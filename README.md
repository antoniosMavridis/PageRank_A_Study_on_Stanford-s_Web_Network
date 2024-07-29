# PageRank: A Study on Stanford's Web Network
An in-depth exploration of Stanford University's web network using Stanweb.dat. This project computes the PageRank vector through various methods, including the power method and Gauss-Seidel iteration. It also investigates the influence of link farms and other factors on PageRank distribution.

## Overview

In this technical report, we will analyze and explore various aspects of the connectivity matrix for
the webpages of Stanford University, provided in the file Stanweb.dat. Our primary focus will be on
calculating the PageRank vector using different methods and parameters.

To begin, we will first find the PageRank vector $π$ using the power method. For both methods, we will consider
$α = 0.85$ as the damping factor and a stopping criterion of $τ = 10^{−8}$. Additionally, we will
define a vector α that has a value of $1$ if it corresponds to a node with no outgoing links, and $0$
otherwise. We will compare the results obtained from both methods and determine if they are
the same. Furthermore, we will assess the speed of each method, with the Gauss-Seidel method
employed for the iterative solution of the system

Moving forward, we will repeat the previous task but with $α = 0.99$. We will evaluate the convergence speed and investigate whether the ranking of the first 50 nodes has changed.
Next, we will delve into the behavior of the convergence of the components of $π$ when using the
power method. We will examine whether all components converge at the same speed to their limits.
If not, we will analyze which components converge faster: those corresponding to important nodes
or those related to non-important nodes. We will also compare this behavior to the convergence
observed when finding π through the solution of the linear system.

In the later part of the report, we will explore the design of link farms and their impact on PageRank
calculations. We will consider a web graph containing a large number of pages labeled from $1$ to
$n$. We will introduce a new web page, $X$, which has neither in-links nor out-links. We will analyze
how the addition of this new page affects the PageRank of the older pages. Using the stationary
equations, we will calculate the new PageRank vector ($π$) of the older pages and determine the
PageRank of page $X$ ($x$) in terms of a variable $r$.

Furthermore, we will introduce another page, $Y$, with no in-links, that links to page $X$. We will
investigate the resulting PageRanks of all the $n + 2$ pages, including $X$. We will assess whether
the PageRank of $X$ improves with this new addition.
Continuing our exploration, we will create a third page, $Z$, and analyze how to set up the links
among the three pages ($X$, $Y$, and $Z$) to maximize the PageRank of $X$.

Additionally, we will examine the impact of adding links from page $X$ to older, popular pages. We
will investigate whether this improves the PageRank of $X$ and determine if the answer changes
when adding links from pages $Y$ or $Z$ to older, popular pages.

Finally, we will outline possible steps that can be taken to further increase the PageRank of page
$X$. While no formal proofs are required, we will summarize our thoughts based on the previous
sections. For extra credit, we will provide a proof for the optimal structure of a link farm with $m$
nodes to optimize the PageRank of page $X$.
Through this report, we aim to gain a comprehensive understanding of the connectivity matrix
and its influence on the PageRank algorithm, while exploring various strategies to enhance the
PageRank of a given webpage.

### Additional Information

The repository also includes a `Report.pdf` that briefly explains our approach and methodology used to solve the problem.
