Problem:  
We study the steady motion of a collection of N = 3000 identical spheres, sheared between two parallel bumpy planes, in the absence of gravity. The two bumpy boundaries move at constant relative velocity in the direction tangent to the planes themselves. The planes are made bumpy by gluing Nw = 240 spheres in a regular hexagonal fashion, at close contact and aligned with the direction of the flow. The spheres glued at the walls have the same diameter (d=1) and mechanical properties of the moving spheres. We take x and z to be the flow and shearing directions, respectively, and neglect variations in the transversal direction y. We focus on constant-volume conditions, so that the number of particles and the vertical distance between the walls, H, are kept constant during shearing. Periodic boundary conditions are employed in the x- and y-directions.  
Details of the problem can be found at: https://on-dem.atlassian.net/wiki/spaces/Index/pages/244744204/Granular+shear+flows+between+bumpy+walls+case

Initial geometrical configuration:  
find it into folder: InitialGeometricalConfiguration
the file GranularShearFlow.restart sets the geometrical info of the simulation: position and radius of each particle.  
The total number of particles is 3480.  
Particles from id 0 to id 479 are those glued at the walls.

Output files format:  
find examples of the output files format into the folder: outputs_example

NOTE: to perform the coarse-graining, we use the post-processing tool "MercuryCG" provided with the open-source DEM code MercuryDPM. The "discrete" output files must be compatible with the MercuryCG, so that, at each time step, two type of files must be generated (see http://docs.mercurydpm.org/Trunk/db/da1/VisualisingYourResults.html):
1) .data file: this is composed by a series of N subsequent lines, each providing information for one particle within the system.
2) .fstat file: this is composed by a series of Nc lines corresponding to each of the Nc particle contacts within the system at the current instant in time.

