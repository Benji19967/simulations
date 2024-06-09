# Experimenting with physics simulations

## Mathematics Background (walk before you run!)

- Mathematics Models in the Physical Sciences by Boas.
    - Great for ODEs and PDEs, which are everywhere in Physics. 
    - Great overview and introduction before going deeper into specific areas.
    - Solve problems of the topics already familiar! (Chapter 1-6, 8 which cover Calculus)
        - Pencil and paper at hand!
    - Then: Chapter 7, 8 and first four sections of Chapter 13. 
    - "You should not feel satisfied with your study of a chapter until you can solve a reasonable number of these problems."
    - Answer book: https://personal.utdallas.edu/~pervin/ENGR3300/answer_book.pdf

## Online Courses

- Computational Physics by 	Kristjan Haule at Rutgers University (2023)
    - https://www.physics.rutgers.edu/grad/509/
    - Uses mostly Python (scipy and numpy) and C++ (with pybind11) to speed up code. 

- Introduction to Computational Physics by Richard Fitzpatrick at UT Austin (2014) 
    - https://farside.ph.utexas.edu/teaching/329/329.pdf
    - Uses the C programming language.
    - Programs are self-contained and written from scratch--good for understanding. 

- Introduction to Computational Physics at ETHZ (2011-2017)
    - https://ethz.ch/content/dam/ethz/special-interest/baug/ifb/ifb-dam/homepage-IfB/Education/bsc_courses/bsc-intro-comphys/documents/CompPhysScript-2017.pdf
    - Computational physics plays an important role in the following fields:
        • Computational Fluid Dynamics (CFD): solve and analyze problems that
        involve fluid flows
        • Classical Phase Transition: percolation, critical phenomena
        • Solid State Physics (Quantum Mechanics)
        • High Energy Physics / Particle Physics: in particular Lattice Quantum
        Chromodynamics (“Lattice QCD”)
        • Astrophysics: many-body simulations of stars, galaxies etc.
        • Geophysics and Solid Mechanics: earthquake simulations, fracture, rupture,
        crack propagation etc.
        • Agent Models (interdisciplinary): complex networks in biology, economy,
        social sciences and many others
    

## Languages

It might be worth it to investigate pros and cons of the following languages and 
what they are best suited for. 

- Python
- C++
- Julia
- Rust (getting some traction in computational biology, see https://rust-bio.github.io/)

## Ideas

1. Generate the position of a particle moving in a straight line in time
2. Generate the position of a particle thrown in a gravitational field in time (parabola)
3. Figure out when the particle hits the ground (root finding)
4. Figure out what angle you should throw it at to make it go the farthest for a fixed speed (optimization)
5. Use a differential equation to factor in air resistance

Do the above for both:
- Writing your own root finding, optimization, and diffeq solvers
    - Try out different methods and examine their precision and stability
- Use prepackaged routines (numpy)

Whenever you write a program, keep in mind:

- What sensitivity are you needing? What sensitivity are you giving the computer in terms of number size (double, long, ...)?
- Is this routine stable under these circumstances?
- What memory and time will be required for the final results?
- What's the physics expected to come out of this situation? Does it match with what the computer is telling me?
- Can I take a quick way out?

### Advanced Ideas

- Patrick Diamond (PhD MIT, UCSD Physics Professor) answer on Quora
    - Contains MANY suggestions!
    - https://qr.ae/psUUAv
