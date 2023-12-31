[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12577732&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Proof

We can prove this through contridiction

Let $A$ and $B$ both be graphs,
Say that $A$ contains fewer nodes than $B$.
Let $f$ be the bijective transformation $f: A \rightarrow B$, since this function is bijective it is both one to one and onto.
Then if we take the map of $A \rightarrow B$ we can see that nodes of $A$ will either map to multiple nodes on $B$ or that there will be unmapped nodes in $B$, both of these situations show that the mapping, $f$, is not one to one, and if it is not one to one it is not bijective, which violates the definition of isomorphism.
$\therefore$ two graphs $A$ and $B$ cannot be isomorphic if they do not contain the same number of nodes.
