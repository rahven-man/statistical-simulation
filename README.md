# Statistical Simulation

### Exploring Probability and Statistics Through Mathematics, Computation and Experiments.

**Statistical Simulation** is an ongoing computational exploration of probability theory, statistical reasoning and mathematical phenomena, built around the idea that mathematical concepts become considerably more intuitive when we can experiment with them.

Inspired by lectures from **Harvard's Statistics 110** and other academic learning resources, this repository investigates probability and statistical concepts through mathematical derivations, computational experiments, Monte Carlo simulations and visual analysis.

Rather than treating probability as a collection of formulas to memorize, the objective is to understand the mechanisms behind those formulas, investigate their behaviour under different conditions, and observe how theoretical predictions emerge through repeated experiments.

This is a growing collection of investigations, not a finished course or a static collection of exercises.

---

## The Approach

Every concept presents a different opportunity to investigate how probability behaves.

A theoretical result might suggest that a particular event has a probability of 50.73%. A simulation allows us to generate thousands of independent experiments and examine whether the observed frequency approaches that prediction.

A mathematical paradox might contradict our intuition. A computational experiment allows us to reconstruct the scenario, isolate the underlying mechanism and investigate the conditions responsible for the result.

The repository follows a consistent approach:

**Mathematical Foundation → Computational Implementation → Simulation → Statistical Analysis → Interpretation**

The emphasis is on understanding why a result occurs, not merely reproducing its numerical value.

### What goes into an investigation?

Depending on the problem, an individual notebook may include:

- Mathematical formulation and theoretical derivations.
- Probability models and their underlying assumptions.
- Implementation using Python and scientific computing libraries.
- Monte Carlo experiments and repeated random sampling.
- Comparison between theoretical predictions and simulated observations.
- Statistical uncertainty, convergence and sensitivity analysis.
- Visual exploration of mathematical relationships.
- Practical interpretations and connections to Data Science.

Not every notebook requires every component. The analytical approach is determined by the problem being investigated.

---

## Repository Structure

The repository is organized into thematic blocks. Each block explores a connected set of mathematical ideas, with individual notebooks dedicated to specific problems, experiments or concepts.

```text
statistical-simulation/
│
├── 01_probability_fundamentals/
│   ├── 01_birthday_problem.ipynb
│   ├── 02_matching_problem.ipynb
│   ├── 03_newton_pepys_problem.ipynb
│   ├── 04_disease_testing_problem.ipynb
│   ├── 05_monty_hall_problem.ipynb
│   └── 06_simpsons_paradox.ipynb
│
├── 02_random_variables_and_distributions/
│   └── ...
│
├── 03_sampling_and_limit_theorems/
│   └── ...
│
├── 04_statistical_inference/
│   └── ...
│
└── README.md
```

The structure will evolve as new topics and investigations are introduced.

---

## Block 01 | Probability Fundamentals

**Status: Completed**

The first block establishes the mathematical foundations of probability through classical problems, counterintuitive results and applications of conditional probability.

Rather than approaching these topics exclusively through textbook exercises, the block investigates them through computational experiments.

| No. | Investigation | Mathematical Concepts |
|---|---|---|
| 01 | Birthday Problem | Complementary probability, independence and collision probability |
| 02 | De Montmort's Matching Problem | Permutations, fixed points and inclusion-exclusion |
| 03 | Newton-Pepys Problem | Binomial probability and probability comparisons |
| 04 | Disease Testing Problem | Conditional probability, Bayes' theorem and base-rate fallacy |
| 05 | Monty Hall Problem | Conditional probability, information and decision-making |
| 06 | Simpson's Paradox | Aggregation, confounding, stratification and standardization |

### Selected Investigations

**The Birthday Problem**

How can a group of just 23 people have approximately a 50.73% probability of containing at least one shared birthday? An investigation into collision probability, complementary events and the effect of group size.

**De Montmort's Matching Problem**

A permutation problem involving shuffled cards and fixed points. The investigation explores the probability of at least one match and its connection to the mathematical constant $e$.

**Newton-Pepys Problem**

A historical probability problem comparing three different dice experiments. The notebook investigates why having a higher number of dice does not necessarily produce a higher probability of satisfying the corresponding success condition.

**Disease Testing Problem**

A Bayesian investigation into diagnostic testing. Despite a test having 95% sensitivity and 95% specificity, a positive result can correspond to a much lower probability of actually having the disease when prevalence is low.

**The Monty Hall Problem**

Three doors, one car and two goats. A computational investigation of why switching produces a winning probability of $2/3$, compared with $1/3$ for staying, under the classical host rules.

**Simpson's Paradox**

An investigation into how a statistical trend can reverse when observations are aggregated across groups with different compositions. The notebook explores subgroup comparisons, direct standardization and the implications for observational data analysis.

---

## The Roadmap

Probability and statistics are broad subjects, and this repository is intended to grow alongside the mathematical concepts being explored.

The following blocks outline the intended direction of the project. Their contents may evolve as the investigations progress.

### Block 02 | Random Variables and Probability Distributions

**Status: Planned**

Moving from individual probability events to mathematical representations of uncertain quantities.

Expected areas of investigation:

- Discrete and continuous random variables.
- Probability mass functions and probability density functions.
- Cumulative distribution functions.
- Expected value and variance.
- Bernoulli and Binomial distributions.
- Geometric and Poisson distributions.
- Uniform and Exponential distributions.
- Normal distribution and its properties.
- Joint distributions and covariance.

The emphasis will be on understanding distributions through repeated sampling, simulated experiments and visual analysis.

### Block 03 | Sampling and Limit Theorems

**Status: Planned**

Investigating how random samples behave and why large-sample statistical methods work.

Expected areas of investigation:

- Sampling distributions.
- Law of Large Numbers.
- Central Limit Theorem.
- Convergence in probability.
- Convergence in distribution.
- Sampling variability.
- Standard errors and sample-size effects.

### Block 04 | Statistical Inference

**Status: Planned**

Using probability models to draw conclusions about populations from observed samples.

Expected areas of investigation:

- Point estimation.
- Confidence intervals.
- Hypothesis testing.
- Null and alternative hypotheses.
- p-values.
- Type I and Type II errors.
- Statistical power.
- Correlation and causal interpretation.
- A/B testing and experimental design.

Additional topics and blocks may be introduced as the project develops.

---

## Technology and Tools

The repository uses Python and its scientific computing ecosystem to translate mathematical ideas into executable experiments.

| Tool | Purpose |
|---|---|
| Python | Primary programming language |
| NumPy | Numerical computation and random sampling |
| Pandas | Data manipulation and statistical summaries |
| Matplotlib | Visualization and graphical analysis |
| SciPy | Probability distributions and statistical functions |
| Jupyter Notebook | Interactive mathematical investigations |

The choice of libraries depends on the requirements of each experiment. The objective is to use computational tools where they contribute to understanding, rather than introducing dependencies without a clear purpose.

---

## Reproducibility

Randomized experiments are designed to be reproducible wherever practical.

Random number generators with explicitly defined seeds are used when consistent results are important.

Theoretical calculations are retained alongside simulation results so that computational estimates can be evaluated against their mathematical expectations.

Simulation results are treated as estimates subject to random variation, not as exact replacements for theoretical probabilities.

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/rahven-man/statistical-simulation.git

cd statistical-simulation
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```powershell
.venv\Scripts\activate
```

### 3. Install the dependencies

```bash
pip install numpy pandas matplotlib scipy seaborn ipykernel jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Alternatively, open the repository in VS Code and execute the notebooks using its Jupyter extension.

---

## What This Repository Is About

Probability is often introduced through formulas, definitions and carefully constructed textbook problems. Those provide the mathematical foundation, but they do not always reveal how probability behaves when we repeatedly experiment with it.

This repository takes a computational approach to that gap.

A theoretical probability is something we can calculate. A simulation is something we can observe. Statistical analysis helps us understand the relationship between the two.

Some experiments confirm intuition. Others challenge it. A few reveal that the intuition itself was based on an incomplete understanding of the problem.

The goal is to build a stronger understanding of probability and statistics by moving repeatedly between mathematical reasoning and computational evidence.

**The repository is a work in progress. The first block, Probability Fundamentals, is complete. Further blocks covering random variables, probability distributions, statistical inference and related concepts are under development.**

---

**Repository:** [rahven-man/statistical-simulation](https://github.com/rahven-man/statistical-simulation)

**Maintainer:** [Rahven](https://github.com/rahven-man)