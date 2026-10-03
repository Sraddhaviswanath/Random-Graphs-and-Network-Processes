# Random Graphs and Network Processes

A computational investigation of Erdős–Rényi random graphs, combining mathematical theory with simulation to study graph structure, connectivity, shortest paths, and random-walk exploration.

## Project Overview

This project investigates structural and dynamical properties of the Erdős–Rényi random graph model \(G(n,p)\).

The main focus is on understanding how the edge probability \(p\) influences the behaviour of a random graph. Mathematical results from random graph theory are compared with computational simulations generated using Python and NetworkX.

The project examines:

* degree distributions
* connected components
* giant-component formation
* connectivity thresholds
* shortest-path distances
* random-walk exploration

## Research Question

**How does the edge probability \(p\) influence the structure and exploration of an Erdős–Rényi random graph?**

## Mathematical Background

In the Erdős–Rényi model \(G(n,p)\), each possible edge between two vertices is included independently with probability \(p\).

For a graph with \(n\) vertices, the degree \(D\) of a fixed vertex follows a binomial distribution:

$$
D \sim \mathrm{Binomial}(n-1,p).
$$

The expected degree is

$$
E[D]=(n-1)p.
$$

The project also investigates two important theoretical scales in random graph theory:

### Giant-component threshold

A giant connected component emerges around

$$
p \approx \frac{1}{n}.
$$

### Connectivity threshold

Full graph connectivity occurs around

$$
p \approx \frac{\log n}{n}.
$$

The simulations investigate these transitions for finite graphs and compare the observed behaviour with these theoretical predictions.

## Methodology

The computational experiments use:

* Python
* NetworkX
* NumPy
* Matplotlib

Random graphs are generated for different values of \(p\), with repeated simulations used to examine variation caused by randomness.

For the main experiments, graphs with

$$
n=100
$$

vertices are studied using multiple independent simulations.

The project combines:

1. theoretical calculations;
2. random graph generation;
3. repeated simulations;
4. numerical summaries;
5. visualisations;
6. interpretation of simulation results.

## Main Investigations

### 1. Degree Distribution

The observed degree distribution of a simulated graph is compared with the theoretical binomial distribution predicted by the Erdős–Rényi model.

The average degree is also examined over repeated simulations and compared with

$$
E[D]=(n-1)p.
$$

### 2. Connected Components

The project investigates how the sizes and number of connected components change as \(p\) increases.

Particular attention is given to the size of the largest connected component.

### 3. Giant-Component Formation

Simulations around the theoretical scale

$$
p \approx \frac{1}{n}
$$

are used to investigate the emergence of a giant component.

For \(n=100\), this scale is approximately

$$
p=0.01.
$$

### 4. Full Connectivity

The probability that the entire graph is connected is investigated for different values of \(p\).

The results are compared with the theoretical connectivity scale

$$
p \approx \frac{\log n}{n}.
$$

### 5. Shortest Paths

Average shortest-path lengths are measured within the largest connected component.

The simulations investigate how increasing edge density affects distances between vertices.

### 6. Random-Walk Exploration

Random walks are simulated on the largest connected component.

The number of unique vertices visited during a fixed number of steps is used as a measure of network exploration.

## Key Findings

The simulations show several consistent patterns.

* Increasing \(p\) increases the expected degree of vertices.
* The largest connected component grows rapidly as \(p\) increases.
* A giant component can emerge before the entire graph becomes connected.
* Full connectivity becomes increasingly likely around the scale \(\log(n)/n\).
* Average shortest-path lengths generally decrease as the graph becomes denser.
* Random walks can explore more unique vertices as the edge probability increases.

These results illustrate how a single probabilistic parameter can produce substantial changes in the structure and behaviour of a random network.

## Limitations

The simulations use graphs with \(n=100\) vertices and a finite number of repetitions. Therefore, the observed transitions can differ from the asymptotic behaviour predicted by random graph theory.

The random-walk experiments also depend on the particular graph generated and the starting vertex.

## Future Work

Possible extensions include:

* increasing the number of vertices;
* increasing the number of simulations;
* investigating larger ranges of \(p\);
* studying how the observed thresholds change with \(n\);
* comparing Erdős–Rényi graphs with other random graph models;
* investigating additional structural properties;
* exploring probabilistic and structural questions related to graph reconstruction.

## Repository Contents

`Random_Graphs_and_Network_Processes_.ipynb`

The Jupyter/Google Colab notebook contains the mathematical explanations, simulations, numerical results, visualisations, and interpretations developed throughout the project.

## Tools

**Python | NetworkX | NumPy | Matplotlib | Jupyter/Google Colab**

## Author

**Sraddha Viswanath**

MSc Mathematics | MSc Data Science

This project was developed as a research-oriented computational study of random graphs and network processes.
