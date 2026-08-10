---
title: "Research"
permalink: /research/
author_profile: true
---

My current research focuses on the soil behaviours and large deformation numerical modelling in computational mechanics.

## 1. Soil behaviours
Like water, soils can exhibit solid-like, fluid-like, and gas-like behaviors. For example, they may behave like a fluid on beaches or in deserts, act as a solid when serving as foundations for buildings, or exhibit gas-like behavior in sandstorms. Our research focuses on these multifaceted and complex behaviors, as well as on unified mathematical models that describe soils across these multiple states.

Key topics include:

- Phase transition constitutive model
- Granular rheology
- Kinetic theory
- Solid-fluid phase transition model

### Solid-fluid phase transition model
**Solid-fluid phase transition** behavior is observed across three distinct stages of landslides: (a) Initiation: transitions from solid-like to fluid-like states; (b) Propagation: moving as a fluid-like state; (c) Sedimentation: regains solid-like behavior. Neither the soil mechanics-based nor fluid mechanics-based models can effectively depict the whole phase transition process. In this regard, we develop a constitutive model for the solid-fluid phase transition of soils.

![Phase transition](/images/Phase_transition.png)
(Phase transition in landslides)

## 2. Computational mechanics
Real-world geohazards (e.g., landslides and soil surface erosion) usually has the large-deformation, large-scale, and multi-physics characteristic. Hence, we use the continuum-based numerical model to develop an efficient numerical platform.

Key topics include:
- Numerical method: Finite Element Method (FVM), Material Point Method (MPM), Lattice Boltzmann Method (LBM), Coupled-Eulerian-Lagrangian (CEL), and **new methods: ???**
- Hybrid numerical model: FVM-MPM, LBM-MPM

### Multiphysics MPM model
We establish two-phase two-point MPM frameworks for simulating soil-water coupling problems (e.g., granular flows, submarine landslides, soil surface erosion). Two sets of Lagrangian material points are used to discretize the soil-solid and fluid phases, while the Eulerian grid is employed to enable an effective soil-water coupling scheme.

![Huangtian landslide simulation](/images/Huangtian.gif)
(Real-world Huangtian landslide-tsunami)

### CFD by MPM
MPM is widely used for free-surface flows, but its performance for viscous incompressible flow past a cylinder has not been systematically assessed. This work develops a cut-cell MPM tailored for viscous incompressible flow past a cylinder. A fractional-step explicit-implicit algorithm is employed, with an explicit stage for the intermediate velocity and an implicit stage for incompressible pressure and final velocity. Irregular boundaries on orthogonal grids are represented using a cut-cell method, while the viscous term is discretized via particle viscous stresses rather than grid stresses.

![flow_past_cylinder simulation](/images/Flow_cylinder.gif)
(Flow past a cylinder)

## 3. AI-based application
We also integrate the finite element method (FEM) with machine learning (ML) to address foundation bearing capacity problems.

