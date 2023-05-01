Download Link: https://assignmentchef.com/product/solved-cecs328-lab7
<br>
<strong>Programming assignment 7. </strong>

<strong>Due date: </strong>Monday, November 30, 2020 at 11:59pm







<strong>Note</strong>: you can have different names for vertices: {a b c d e ..} = {v1 v2 v3 v4 ..} = {1 2 3 4 ..}




In this program you are required to implement BFS.

First, you can create the below graph and print the resulting adjacency matrix/list. Or create a random graph.

<strong><u>Part A.</u></strong>

<ol>

 <li>Request the user to determine the starting vertex (<em>a</em>) for <strong>BFS</strong> algorithm</li>

 <li>Call <em>BFS</em> function to find the vertices reachable from vertex <em>u</em> and print the <em>shortest paths</em> and their <em>lengths/distances</em>.</li>

</ol>




<strong><u>Part B.</u></strong>

In this part you are required to determine if a random undirected graph is <u>bipartite</u> or not. You can use the below graph to test.




Here, we work with three colors for the vertices: <em>gray</em> (not visited), [<em>blue, red</em>] (<strong><u>opposite colors</u></strong>)

<ol>

 <li>Print the resulting adjacency matrix/list.</li>

 <li>Implement 2 functions: <em>Explore</em> and <em>Is_bipartite </em></li>

 <li>In <strong><em>Explore</em></strong> function,

  <ol>

   <li>For each vertex (v) initialize <em>color = “gray”. </em></li>

   <li>Start from the first vertex, color it <em>“blue” </em>and call <em>Is_bipartite</em> on that.</li>

   <li>Next, go to the next unexplored vertex (having <em>gray</em> color), color it <em>“blue” </em>and call <em>Is_bipartite</em></li>

   <li>Repeat <em>step c.</em> until every vertex is explored/colored or a not bipartite graph is detected.</li>

  </ol></li>

 <li>Now to implement our second function (<strong><em>Is_bipartite</em></strong>), you need to change your BFS function in part A. a. Keep popping each vertex from <em>Q</em>. (call it <strong>u</strong>)

  <ol>

   <li>Go to the adjacency list of <strong>u</strong>, (adj(u)), and for <u>each neighbor</u> (<strong>v</strong>):</li>

   <li>If <strong><em>v</em></strong>. <em>color</em> == “<em>gray</em>”, assign an opposite color to <strong>v</strong> and push it into the <em>Q</em>. (<strong><u>Example</u></strong>: <strong><em>u</em></strong><em>.color</em> is <em>blue</em>, and <strong><em>v</em></strong><em>.color</em> is <em>gray</em> ➔ we set <strong><em>v</em></strong><em>.color</em> = “<em>red</em>”)</li>

   <li>Else if <strong><em>v</em></strong><em>.color</em> == <strong><em>u</em></strong><em>.color</em>: Stop the entire code and print “<strong>NOT bipartite</strong>”.</li>

  </ol></li>

 <li>Print the color of all the vertices.</li>

</ol>





