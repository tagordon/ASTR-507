This is the git repository for my thermodynamics class. 
=======
## Particles in a box

The only physical constant in the code is boltzmann's constant, which I've defined such that the mass unit is approximately the 
hydrogen mass, the distance unit is Angstroms, and the time unit is seconds. This part of the code is only used to compute 
the Maxwell distribution function. For the rest of the simulation, the user is free to choose consistent units. )

I check for collisions by computing the distance between two particles. If they are closer than the sum of their radii at 
any timestep, then a collision has occured and their new velocities are computed by applying momentum and energy conservation 
to a two-body collision between hard-sphere particles. 

I used periodic boundary conditions because they conserve momentum. 
