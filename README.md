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
