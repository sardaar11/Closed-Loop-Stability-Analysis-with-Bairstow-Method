# Project Description

## Overview
This project focuses on finding the roots of the characteristic equation of a closed-loop control system using the Bairstow method. The roots, also known as poles, are essential in determining the stability of the control system. By locating these poles, the stability analysis can be performed to ensure the system behaves as desired under various conditions. Here, the stability of the control loop is checked for different values of $K_c$  and  $\tau_I$

## Stability Analysis with Poles
In control system theory, the stability of a system is determined by the location of its poles in the complex plane. The characteristic equation, derived from the closed-loop transfer function, provides these poles. For a system to be stable, all poles must lie within the left half of the complex plane (i.e., they must have negative real parts). If any pole lies on the right half of the complex plane or on the imaginary axis, the system is considered unstable. This analysis is crucial for designing and validating control systems in engineering applications.

## Bairstow Method
The Bairstow method is an iterative algorithm used to find the roots of a polynomial equation. It is particularly useful for finding both real and complex conjugate roots of polynomials with real coefficients. The method works by assuming a quadratic factor of the polynomial and iteratively refining the coefficients of this factor until the roots are determined with desired accuracy. The main steps are:

1. **Initialization**: Start with an initial guess for the coefficients of the quadratic factor.
2. **Iteration**: 
   - Use the current guess to divide the polynomial and obtain the quotient and remainder.
   - Solve a set of linear equations to update the guess.
3. **Convergence**: Repeat the iteration until the change in the coefficients is smaller than a predefined tolerance.
4. **Root Extraction**: Once the quadratic factor is determined, its roots are extracted, and the polynomial is deflated. The process is then repeated on the deflated polynomial to find all roots.

This project implements the Bairstow method to automate the process of finding the poles of a given characteristic equation, facilitating the stability analysis of the control system.
