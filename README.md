# circular-hierarchy

Creates a random hierarchy and displays it using a circular layout. The data generation and visualization are done from scratch (for example, d3-hierarchy is **not** used).

The steps are the following:

- Generate a data hierarchy of random depth and width - `generateRandomHierarchy`
- Recursivly count leaves and depth - `walk1`
- Determine depth and radius from center of each level
- Determine leaf angle and leaf radius
- Recursivley set node angles - `walk2`
- Recursivly determine position of all nodes - `walk3`
- Create the SVG
- Recursively draw the edges (cubic bezier curves) - `drawLines`
- Recursivly draw the nodes (circles) - `drawCircles`

**Screenshots**

![Screenshot](https://raw.github.com/boeric/CircularHierarchy/master/screenshots/Screen%20Shot%201%20Nodes%20and%20Edges.png)
![Screenshot](https://raw.github.com/boeric/CircularHierarchy/master/screenshots/Screen%20Shot%202%20Edges%20Only.png)
