# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Answer
Two graphs $A$ and $B$ do not have to be completely connected to be isomorphic. Connected means "undirected, and a path between any two vertices" the path between any two verticies is important here.
Two graphs are isomorphic if they "have the same structure", a given example from this example states $G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

To test this we can do a square and an hourglass, represented by S and H respectively. Graph Square is represented by S where $S = (VS, ES)$ and $VS = [1,2,3,4]$ and $ES = [(1,2),(1,3),(2,4),(3,4)]$
Likewise, Graph Hourglass is represented by H where $H = (VH, EH)$ where $VH = [1,2,3,4]$ and $EH = [(1,2),(1,4),(2,3),(3,4)$. To prove S and H are isomorphic, we just need to swap vertices 1 and 2 in SH, when we swap those, so $VH = [2,1,3,4]$ and $EH = [(1,2),(2,4),(1,3),(3,4)]$ which now contains all the same edges as ES, proving the two graphs are isomorphic.

Now to test on a simple example of an unconnected graph, A, where A is visually represented by a triangle and a square, unconnected, which we can represent as $A = (VA, EA)$ where $VA = [1,2,3,4,5,6,7]$ and $EA = [(1,2),(1,3),(2,3),(4,5),(4,6),(5,7),(6,7)] and B, consisting of a triangle and an hourglass, unconnected, which can be represented as $B = (VB, EB)$ where $VB = [1,2,3,4,5,6,7]$ and $EB = [(1,2),(1,3),(2,3),(4,5),(4,7),(5,6),(6,7)]. To prove these two are isomorphic, we swap verticies 4 and 5 in B, giving us $VB = [1,2,3,5,4,6,7]$ and $EB = [(1,2),(1,3),(2,3),(4,5),(4,6),(5,7),(6,7)$ so now EB = EA, proving that these two graphs are isomorphic. There is no need for connectivity for two graphs to be isomorphic.

Isomorphisms only need to maintain the adjacency, no matter the swaps, the adjacencies are maintained. What matters is that the disconnects must be the same between graphs. For example the triangle and square can't be connected by one edge but then not in the hourglass example. The isomorphisms must be able to be represented by only a simple swap.

### Sources and Plagarism Statement
Used this to help understand isomorphisms and connectivity [GeeksforGeeks] (https://www.geeksforgeeks.org/graph-isomorphisms-connectivity/#)
Used slides from class to help with definitions.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
