# 3D Curve Print

For this project I wanted to create an artistic/fun 3d curve, make two copies of it so the resulting three 3d curves form a chain, and then create a 3d print of this object.  

My objective was to get experience designing B-spline curves and surfaces, improve my understanding of 3d geometry, understand the concept of curves on a surfaces (ConS), and get hands on experience with 3d printing.  The first step was to design and plot a 2d B-spline curve.  I wanted to create something that I could give to my girlfriend as a gift after 3D printing, so I decided to make a curve in the shape of a turtle because she studies marine biology.  This proved to very difficult because I had to research exactly how different control points and knots affected a B-spline curve and experiment until I was able to design one continuous curve in the shape of a turtle.  Then I formatted the control points by centering them around the origin and scale/translating them so that they exist in the domain of a Bezier surface.  Then I plotted the curve, control points, and the curve polygon.  The next step was to design a Bezier surface patch.  I defined a function for the equation of the surface, defined the number of control points in each row/column of the control net, defined the control points and centered them around the origin, and defined a control net by using the surface equation to generate z-values for control points.  The next step was to plot the B-spline curve as a ConS (curve on surface) with the surface.  I defined a function to evaluate points on the curve, a function to get a point on the surface at a given (u,v) parameter pair, and created a plot of the surface, control net, curve-on-surface, and points.  The next I created a plot of the ConS without the surface and used the tube function to give it some thickness.  Then I defined a function to evaluate points on the ConS and translated the ConS twice to create a plot of three curves chained together.  After this, I exported the ConS as an STL file and used Cura to make a 3D print of the curves.  
