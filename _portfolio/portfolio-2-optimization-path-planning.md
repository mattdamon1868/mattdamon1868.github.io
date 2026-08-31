---
title: "Optimization Path Planning"
excerpt: "Linear programming (duality + simplex) applied to constrained robot path planning."
collection: portfolio
---

This project formulated an optimization problem for robot path planning under competing constraints energy use, weight, and obstacle risk using duality principles and the simplex method within a linear programming framework.

The objective function incorporated energy consumption, weight, distance to the source, and obstacle probability, each with an arbitrary weighting, to evaluate the most efficient path. The original nonlinear problem was linearized to enable analysis via the simplex method and duality principle: the simplex method progresses from vertex to vertex of the feasible region toward an optimal solution, while the duality principle derives a dual (Lagrangian) problem to solve alongside the primal.

The revised objective function is represented as:

J(x) = α·x₁ + β·x₂ + γ·x₃ + δ·x₄

where x₁ is energy, x₂ is robot weight, x₃ is the deviation between the primary and adjusted path (with a penalty gain), and x₄ is the likelihood of an obstacle in the robot's path. This formulation was solved using the Gurobi optimizer library to identify the optimal path within the feasible region defined by the constraints.

The goal of the project was to build a deeper working understanding of linear programming techniques applied to a constrained robotics problem, rather than to find a single "optimal" gain set.

**Skills:** Optimization, duality, Python, Gurobi optimizer library
