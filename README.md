# Voronoi-Halfspace

# Overview

This project provides a mathematical and computational approach to finding the Voronoi half-space that separates two points in Euclidean space. The half-space represents the set of all points that are closer to one point than the another and is defined in the form:

        { x ∈ R^n | c^Tx <= d }
        
where c is the normal vector and d is the threshold value.

# Problem Statement

Given two distinct points a,b ∈ R^n, the goal is to find the half-space that contains all points closer to a than to b. Mathematically, we define the region as :

        S = {x ∈ R^n | ||x - a||2 <= ||x - b||2}

Using algebraic manipulation, this can be rewritten in the linear form as :

        2(b - a)^Tx <= b^Tb - a^Ta

This confirms that the set of points forms a half-space, which is a convex region.

# Methodology

<ins> (a) Compute the Normal Vector </ins>

The normal vector for the half-space equation is given by :

        c = 2(b - a)

<ins> (b) Compute the Threshold Value </ins>

The thrshold value is given by :

        d = b^Tb - a^Ta

<ins> (c) Implementation in Python </ins>

1. Define two points a and b in R^n.

2. Compute the normal vector c using the formula given above.

3. Compute the threshold value d using the formula given above.

4. Display the final half-space equation.

# Dependencies

1. Python 3

2. NumPy

3. Pandas

# Usage

1. Run the provided Python script in any Python environment.

2. Modify the values of a and b to compute different half-spaces.

3. The output will display the normal vector, threshold and half-space equation.

# Conclusion

This project successfully determines the Voronoi half-space separating two points using mathematical derivation and Python computation. The result confirms that the set of points forms a convex half-space, as expected.
