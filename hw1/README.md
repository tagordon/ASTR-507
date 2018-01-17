## Particles in a box

I didn't define dimensions for velocity, mass, energy, or length. The user is free to choose consistent dimensions. All particles 
have mass = 1 in whatever dimensions are chosen. For instance, if the user is happy with the particles having masses of one 
gram, they can use cgs units for all quantities. 

I check for collisions by computing the distance between two particles. If they are closer than the sum of their radii at 
any timestep, then a collision has occured and their new velocities are computed by applying momentum and energy conservation 
to a two-body collision between hard-sphere particles. 

Boundaries are periodic - I also implemented hard-wall boundaries but these, of course, do not conserve momentum so I chose 
to use periodic boundaries instead. I could have handled the hard-wall boundary momentum problem in a variety of ways, but 
simply implementing periodic boundaries seemed like a more natural choice. 
