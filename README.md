# Shallow Waves Simulation System
## Introduction
In this case, we can see the shallow waves effects on the surface and a two-way coupling result between cubes and water.

The pool is incompressible and has a clear boundaries.

The task is based on Unity.

## Hydrodynamics
To simplify the problem, we use height field to represent the waves based on Euler grid and only use pressure to update the velocity field.

Viscosity is expressed by a coefficient acting on the momentum part and the coefficient before controlling the pressure is constant to guarantee incompressibility.

We choose to use a Neumann method to guarantee a closed boundary.

## Coupling
Two rigid cubes can create waves on the surface and float on the water due to buoyancy.

We calculate a virtual height in order to update the height using an existing formula and acts inversely to create block buoyancy.

## Interaction
User can press 'r' to randomly generate waves and drag the left cube by mose to see the two-way coupling effects.

## Effects





https://user-images.githubusercontent.com/53171201/209751438-7665606f-2644-4a89-804b-16a79558bd52.mov



