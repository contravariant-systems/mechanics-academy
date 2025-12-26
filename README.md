# The Canon of Mechanics

*Essential texts across classical mechanics, continuum physics, and their mathematical and computational foundations*

---

## Panoramic Views

Before specialising, certain works illuminate how physics connects as a whole.

**Penrose — The Road to Reality** (1,100 pages) is unmatched for seeing the entire landscape—from complex numbers through twistors to quantum gravity—with genuine mathematical depth throughout. Idiosyncratic and opinionated, but irreplaceable.

**Feynman — Lectures on Physics** remain pedagogically brilliant for physical intuition. They predate the geometric revolution (no symplectic manifolds, no fibre bundles), but Feynman's reasoning is irreplaceable. Volume II on electromagnetism and Volume III on quantum mechanics contain insights found nowhere else.

**Susskind — The Theoretical Minimum** (Stanford lectures, freely available) provides honest, accessible foundations. Valuable for building intuition before Landau, and for teaching others.

Two traditions run through this document: the geometric-theoretical (Landau, Arnol'd, Marsden, Wald) and the computational-applied (Hughes, Simo, Ferziger, Brunton). Both are essential. The geometric tradition reveals *why* things work; the computational tradition reveals *how* to make them work. The rare texts that bridge both—SICM, Marsden's variational integrators, structure-preserving machine learning—are especially valuable.

---

## Foundations & Prerequisites

This document is written for readers with undergraduate mathematics and physics—comfortable with multivariable calculus, linear algebra, ODEs, and classical mechanics at the Kleppner-Kolenkow or Marion-Thornton level. The texts below fill common gaps before tackling the main canon:

**Analysis & Linear Algebra:** Rudin's *Principles of Mathematical Analysis* for rigour. Axler's *Linear Algebra Done Right* or Strang's MIT 18.06 lectures for the essential language. Kreyszig's *Introductory Functional Analysis with Applications* bridges to infinite dimensions.

**Differential Equations:** Arnold's *Ordinary Differential Equations* (the gentler Arnold). For PDEs, **Evans — Partial Differential Equations** (2nd edition) is now standard—systematic, modern, and covers weak solutions essential for computational work. Strauss provides a more applied alternative.

**Probability & Stochastic Processes:** Grimmett & Stirzaker for foundations. Gardiner's *Stochastic Methods* for physics applications.

**Intermediate physics:** Griffiths' *Electrodynamics* and *Quantum Mechanics* before Landau or Jackson. These are genuinely good books, not just stepping stones.

Many canonical texts have affordable editions: Dover reprints (Lanczos, Den Hartog, Hughes, Taylor), free PDFs from authors (Tong, Carroll gr-qc/9712019, Lubliner, Cannas da Silva), and institutional access. The expensive Springer hardbacks often appear in university libraries.

---

## How to Begin

This is a canon, not a syllabus. Pick one entry point and commit to it for a month before reassessing.

A useful rhythm at any level: **one spine text + one problem source + one lecture series + one computational companion**.

**Concept-first** — if you want physical intuition and momentum.
Spine: Feynman I or Susskind. Problems: Kleppner-Kolenkow selectively. Lectures: MIT 8.01 or Shankar. Bridge to formalism: Taylor → Tong's Classical Dynamics notes.
*First month: 8-10 lectures, 20-30 problems, weekly one-paragraph reflection on which symmetry or conserved quantity you actually used.*

**Geometry-first** — if you want structure (symplectic forms, Noether, manifolds) early.
Spine: Schuller → Arnol'd. Problems: Taylor (coordinate-free problems). Lectures: Schuller videos, Tong notes alongside Arnol'd. Bridge: Tong's GR or QFT notes.
*First month: Schuller's core arc, first serious Arnol'd chapter, one system (pendulum or rigid body) implemented symbolically.*

**Computation-first** — if you want to make ideas run and keep yourself honest.
Spine: Tong or Taylor. Companion: SICM as executable text. Bridge: Barba (CFD Python) or Bathe (FEM).
*First month: derive one system (Lagrangian → equations), integrate it two ways (symplectic vs. non-symplectic), write one paragraph on what invariants drift and why.*

---

## Mathematical Foundations

### Geometry for Physics

**Arnol'd — Mathematical Methods of Classical Mechanics** is the geometric foundation for theoretical physics. Constructs mechanics from differential geometry: manifolds, tangent bundles, symplectic structures, Lie groups. Everything else builds on this language.

**Schuller — Lectures on the Geometric Anatomy of Theoretical Physics** (28 lectures, YouTube) builds the mathematical machinery from propositional logic through topology, manifolds, bundles, and connections. The ideal preparation for Arnol'd. Simon Rea's transcribed notes provide written accompaniment.

**Nakahara — Geometry, Topology and Physics** bridges formalism to physics: gauge theories, anomalies, topological invariants.

**Cannas da Silva — Lectures on Symplectic Geometry** (freely available) provides the symplectic manifold theory essential for Hamiltonian mechanics.

For full mathematical rigour: **Lee's "Introduction to Smooth Manifolds"** and **"Riemannian Manifolds"**. For bridging to applications: **Frankel's "The Geometry of Physics"**.

### Analysis for Mechanics

**Evans — Partial Differential Equations** is the modern standard. Sobolev spaces, weak solutions, regularity — the language of modern computational mechanics.

**Temam — Navier-Stokes Equations** provides the functional analysis foundations for fluid mechanics. Existence, uniqueness, regularity for the central equations.

**Brezis — Functional Analysis, Sobolev Spaces and Partial Differential Equations** bridges analysis and PDEs elegantly.

For existence theory in elasticity: Ciarlet (see Continuum Mechanics). For spectral theory: Reed & Simon (see Quantum Mechanics).

---

## Classical Mechanics

### Foundations

**Landau & Lifshitz — Mechanics (Vol. 1)** derives everything from symmetry and least action in 170 pages. Teaches you to *think* like a theoretical physicist. The gap-filling it demands is part of the education. *If you read one book on classical mechanics, this is the one.*

**Arnol'd — Mathematical Methods of Classical Mechanics** is the geometric reformulation. Phase space as symplectic manifold. Liouville integrability. KAM theory. Where Landau is physics-first, Arnol'd is geometry-first. Both are essential, and they illuminate each other.

**Goldstein — Classical Mechanics** (2nd edition preferred) is the comprehensive graduate course. More accessible than Landau, more thorough than most. Has trained generations.

**Sussman & Wisdom — Structure and Interpretation of Classical Mechanics** is unique: executable mathematics where every equation is working Scheme code. Forces computational honesty about what notation actually means. Bridges the geometric and computational traditions more directly than any other text.

**Lanczos — The Variational Principles of Mechanics** provides unmatched philosophical depth on *why* variational methods work.

**Lectures:** MIT 8.01 (Lewin) for Newtonian foundations. David Tong's *Classical Dynamics* notes for the bridge to analytical mechanics.

### Advanced Geometric Mechanics

**Abraham & Marsden — Foundations of Mechanics** (800+ pages) is the geometric mechanics bible. More comprehensive than Marsden-Ratiu.

**Marsden & Ratiu — Introduction to Mechanics and Symmetry** develops momentum maps, Poisson reduction, Lie group actions. Their treatment of variational integrators—discretising the Lagrangian rather than the equations—is essential for long-term simulations.

**José & Saletan — Classical Dynamics: A Contemporary Approach** bridges Goldstein's physics-first style with Arnol'd's geometry-first approach.

**Spivak — Physics for Mathematicians: Mechanics I** is obsessively rigorous, asking what a reference frame *precisely is*.

### Dynamical Systems & Control

**Strogatz — Nonlinear Dynamics and Chaos** (3rd edition) combines exceptional clarity with rigorous treatment of bifurcations, strange attractors, and chaos. The definitive introduction.

**Guckenheimer & Holmes — Nonlinear Oscillations, Dynamical Systems, and Bifurcations of Vector Fields** is the mathematical treatment. Center manifolds, normal forms, Melnikov methods. Where Strogatz builds intuition, this builds machinery.

**Wiggins — Introduction to Applied Nonlinear Dynamical Systems and Chaos** (2nd edition) bridges Strogatz and Guckenheimer-Holmes. Comprehensive with extensive examples.

**Khalil — Nonlinear Systems** (3rd edition) is the standard for control-oriented dynamical systems. Lyapunov stability, input-output methods, feedback linearisation.

**Sontag — Mathematical Control Theory** (free PDF from author) provides the deterministic foundations with mathematical rigour.

**Lectures:** MIT 12.006J (chaos), Steve Brunton's YouTube series on data-driven dynamical systems and control.

### Problems

**Kotkin & Serbo — Exploring Classical Mechanics** offers 350+ problems with full solutions corresponding to Landau and Goldstein. Essential for mastery.

---

## Continuum Mechanics — Solids

### Foundations

**Truesdell & Noll — The Non-Linear Field Theories of Mechanics** (Handbuch der Physik) establishes the axiomatic foundations of rational mechanics. All serious work builds on this framework. Not a first book, but the book you eventually need.

**Gurtin — An Introduction to Continuum Mechanics** provides elegant, concise first principles. *The clean starting point for continuum mechanics.*

**Gurtin, Fried & Anand — The Mechanics and Thermodynamics of Continua** offers comprehensive modern treatment including crystal plasticity and gradient theories.

### Elasticity

**Marsden & Hughes — Mathematical Foundations of Elasticity** is the definitive geometric treatment using differential geometry and functional analysis. Bridges engineer tensor notation with mathematician bundle language. Dover reprint available.

**Ogden — Non-Linear Elastic Deformations** is finite elasticity done meticulously. Stability, bifurcation, incompressibility. The reference for rubber, soft tissue, large deformations.

**Ciarlet — Mathematical Elasticity** (3 volumes) provides rigorous existence theorems and asymptotic justification of plate and shell theories. The mathematical bible.

**Antman — Nonlinear Problems of Elasticity** develops geometrically exact Cosserat theories for rods and shells with rigorous bifurcation analysis. Contains unsolved research problems. The frontier.

**Holzapfel — Nonlinear Solid Mechanics** adds computational focus with the best treatment of tangent stiffness matrices for FEA. Essential for biomechanics.

**Lectures:** Rohan Abeyaratne's MIT notes (400+ pages, free) provide worked examples in finite elasticity.

### Plasticity & Fracture

**Simo & Hughes — Computational Inelasticity** is the definitive reference for return mapping algorithms, finite-strain plasticity, consistent tangent operators. Bridges theory to code.

**Lubliner — Plasticity Theory** (freely available from Berkeley) provides comprehensive classical treatment.

**Anderson — Fracture Mechanics** (4th edition) is the standard text, adopted at 150+ universities. Linear elastic fracture mechanics through ductile failure.

**Freund — Dynamic Fracture Mechanics** covers crack propagation dynamics.

---

## Continuum Mechanics — Fluids

### Foundations

**Batchelor — An Introduction to Fluid Dynamics** is THE book. Elegant mathematical development emphasising physical mechanisms. Every derivation meticulous. The standard against which others are measured.

**Landau & Lifshitz — Fluid Mechanics (Vol. 6)** complements Batchelor with characteristic compression and insight.

**Acheson — Elementary Fluid Dynamics** is an excellent intermediate text, more accessible than Batchelor.

**Lectures:** David Tong's *Fluid Mechanics* notes (~240 pages) derive Navier-Stokes from first principles through boundary layers and turbulence.

### Viscous & Boundary Layer Flow

**Schlichting & Gersten — Boundary-Layer Theory** (9th edition) is legendary. The definitive treatment of viscous flow near surfaces.

**White — Viscous Fluid Flow** serves as the standard graduate engineering text.

### Turbulence

**Pope — Turbulent Flows** is the modern standard. Fundamentals through DNS, LES, PDF methods. Rigorous yet readable.

**Tennekes & Lumley — A First Course in Turbulence** is the classic physical introduction using dimensional analysis. Complements Pope.

**Frisch — Turbulence: The Legacy of Kolmogorov** offers the theoretical physics perspective with mathematical rigour.

### Compressible Flow

**Liepmann & Roshko — Elements of Gasdynamics** is the Caltech classic. Timeless treatment of shocks, expansions, nozzle flow.

**Anderson — Modern Compressible Flow** provides comprehensive modern treatment with applications.

### Stability & MHD

**Chandrasekhar — Hydrodynamic and Hydromagnetic Stability** is stability theory done definitively. Thermal convection, rotating flows, magnetic fields.

**Drazin & Reid — Hydrodynamic Stability** (2nd edition) covers linear stability theory comprehensively.

**Davidson — Introduction to Magnetohydrodynamics** provides modern accessible MHD treatment.

### Rheology

**Bird, Armstrong & Hassager — Dynamics of Polymeric Liquids** (2 volumes) is the definitive reference for non-Newtonian fluids.

### Computational

**Lorena Barba — CFD Python: 12 Steps to Navier-Stokes** (Jupyter notebooks, free) teaches implementation through building a solver. The pedagogical model for computational tutorials.

**OpenFOAM** documentation and tutorials provide industrial-strength CFD. **FEniCS/FEniCSx** for finite elements with automatic differentiation. **JAX-Fluids** and **PhiFlow** for differentiable fluid simulation.

---

## Thermodynamics & Statistical Mechanics

### Thermodynamics

**Callen — Thermodynamics and an Introduction to Thermostatistics** is axiomatic thermodynamics via four postulates. The ideal preparation for statistical mechanics.

### Statistical Mechanics

**Landau & Lifshitz — Statistical Physics (Vol. 5)** develops ensemble formalism without ergodic hypotheses. Derives thermodynamics as consequence of statistics.

**Landau & Lifshitz — Statistical Physics Part 2 (Vol. 9)** covers quantum fluids and condensed matter.

**Landau & Lifshitz — Physical Kinetics (Vol. 10)** completes the treatment with transport and non-equilibrium.

**Chandler — Introduction to Modern Statistical Mechanics** covers Monte Carlo, renormalisation, modern computational methods.

**Lectures:** Mehran Kardar's MIT 8.333/8.334 (video on OCW) covers statistical mechanics with full rigour. David Tong's *Statistical Physics* and *Kinetic Theory* notes are exceptional.

### Non-Equilibrium

**de Groot & Mazur — Non-Equilibrium Thermodynamics** is the definitive treatment of linear irreversible thermodynamics and Onsager relations.

**Zwanzig — Nonequilibrium Statistical Mechanics** presents projection operator formalism with exceptional clarity.

### Transport

**Bird, Stewart & Lightfoot — Transport Phenomena** ("BSL") is the definitive treatment of momentum, heat, and mass transport.

### Problems

**Kubo — Statistical Mechanics: Problems with Solutions** provides essential problem sets for mastery.

---

## Quantum Mechanics

### Foundations

**Landau & Lifshitz — Quantum Mechanics (Vol. 3)** achieves legendary concision with profound physical insight. Demands mathematical maturity.

**Dirac — The Principles of Quantum Mechanics** presents the conceptual architecture from its creator. How to think about quantum mechanics.

**Sakurai — Modern Quantum Mechanics** (3rd edition) is the standard graduate text. Balanced rigour and physical intuition. *If you want one modern graduate QM book, this is it.*

**Cohen-Tannoudji — Quantum Mechanics** (2 volumes) offers encyclopedic completeness with extensive complements. More reference than textbook, but invaluable.

**Lectures:** MIT 8.04/8.05/8.06 (Zwiebach) provides the complete sequence with video. Perimeter Institute's PSI courses go deeper.

### Mathematical Foundations

**Reed & Simon — Methods of Modern Mathematical Physics** (4 volumes) is the mathematical foundation done rigorously. Functional analysis, operators, scattering theory.

**von Neumann — Mathematical Foundations of Quantum Mechanics** (2018 corrected edition) established the Hilbert space framework.

**Hall — Quantum Theory for Mathematicians** is a modern bridge between physics and mathematics cultures.

**Takhtajan — Quantum Mechanics for Mathematicians** treats path integrals, Grassmann variables, and supersymmetry rigorously.

### Scattering & Path Integrals

**Taylor — Scattering Theory** (Dover) is the clearest pedagogical treatment of scattering.

**Feynman & Hibbs — Quantum Mechanics and Path Integrals** (emended edition) transmits insight from the inventor.

**Zinn-Justin — Path Integrals in Quantum Mechanics** provides rigorous treatment connecting to statistical mechanics and field theory. His larger *Quantum Field Theory and Critical Phenomena* is encyclopedic.

**Kleinert — Path Integrals in Quantum Mechanics, Statistics, Polymer Physics, and Financial Markets** (5th edition, 1500+ pages) is comprehensive to the point of excess—but contains things found nowhere else.

### Quantum Information

**Nielsen & Chuang — Quantum Computation and Quantum Information** is the undisputed bible with 58,000+ citations.

**Preskill — Quantum Information Lecture Notes** (Caltech, free) provides comprehensive graduate coverage.

### Problems

**Zettili — Quantum Mechanics: Concepts and Applications** contains ~700 problems, many solved. Essential for calculation fluency.

---

## Quantum Field Theory

### Foundations

**Weinberg — The Quantum Theory of Fields** (3 volumes) builds QFT from relativistic invariance and cluster decomposition. Dense, uncompromising, definitive.

**Peskin & Schroeder — An Introduction to Quantum Field Theory** is the standard course text emphasising calculations. Where most physicists learn QFT.

**Schwartz — Quantum Field Theory and the Standard Model** integrates effective field theory throughout. Modern approach.

**Lectures:** David Tong's *Quantum Field Theory* notes with Perimeter Institute videos. Sidney Coleman's Harvard lectures (video available). TASI summer school for current topics.

### Mathematical

**Streater & Wightman — PCT, Spin and Statistics, and All That** establishes the axiomatic Wightman framework.

**Folland — Quantum Field Theory: A Tourist Guide for Mathematicians** presents QFT as practiced by physicists, identifying mathematical gaps carefully.

**Haag — Local Quantum Physics** founds algebraic QFT.

### Advanced

**Duncan — The Conceptual Framework of Quantum Field Theory** (782 pages) fills conceptual gaps other texts neglect.

**Burgess — Introduction to Effective Field Theory** is the first comprehensive EFT textbook.

---

## General Relativity

### Foundations

**Misner, Thorne & Wheeler — Gravitation** (1,279 pages) is encyclopedic with two tracks through the material. Physical intuition emphasised. Taught a generation. Not for the faint-hearted, but irreplaceable.

**Wald — General Relativity** provides mathematical rigour and modern geometric methods. Where MTW emphasises intuition, Wald emphasises precision. Together they cover everything.

**Carroll — Spacetime and Geometry** is the best first graduate course, combining accessibility with rigour. *Start here.* His lecture notes (gr-qc/9712019) are freely available.

**Weinberg — Gravitation and Cosmology** offers the field-theoretic perspective. Gravity as spin-2 field.

**Lectures:** David Tong's *General Relativity* notes. Susskind's Stanford lectures for intuitive foundations. eigenchris (YouTube) for visual tensor calculus.

### Advanced

**Hawking & Ellis — The Large Scale Structure of Space-Time** covers global methods, singularity theorems, causal structure. The mathematical physics of spacetime.

**Poisson — A Relativist's Toolkit** provides practical computational tools. Best Hamiltonian formulation treatment.

### Gravitational Waves & Cosmology

**Maggiore — Gravitational Waves** (2 volumes) is definitive: theory through detection to astrophysical sources.

**Dodelson — Modern Cosmology** (2nd edition) covers CMB physics and large-scale structure.

### Problems

**Lightman, Press, Price & Teukolsky — Problem Book in Relativity and Gravitation** contains 475 problems with solutions. Essential.

---

## Condensed Matter Physics

### Foundations

**Ashcroft & Mermin — Solid State Physics** remains the standard graduate introduction after 50 years. Crystal structure, electronic bands, phonons, magnetism. Essential vocabulary for anyone touching materials.

**Chaikin & Lubensky — Principles of Condensed Matter Physics** is the other essential text, emphasising soft matter and phase transitions from a statistical mechanics perspective. Liquid crystals, polymers, membranes alongside traditional solid state. Where Ashcroft-Mermin is about electrons, this is about everything else.

### Field Theory Methods

**Altland & Simons — Condensed Matter Field Theory** (2nd edition) is the modern treatment using path integrals and field-theoretic methods. Superconductivity, magnetism, disordered systems, topology.

**Fradkin — Field Theories of Condensed Matter Physics** (2nd edition) covers topological phases, quantum Hall, and modern developments.

**Abrikosov, Gorkov & Dzyaloshinski — Methods of Quantum Field Theory in Statistical Physics** ("AGD") is the classic many-body Green's function approach. Dated but foundational.

### Many-Body Theory

**Mahan — Many-Particle Physics** (3rd edition) is comprehensive: Green's functions, diagrams, transport, superconductivity.

**Coleman — Introduction to Many-Body Physics** (Cambridge) provides modern perspective with exceptional clarity on renormalisation group and heavy fermions.

### Lectures

David Tong's *Statistical Field Theory* notes cover critical phenomena. MIT 8.511 (condensed matter) provides course materials. Perimeter PSI has advanced courses.

---

## Computational Mechanics

### Numerical Foundations

**Trefethen & Bau — Numerical Linear Algebra** is the essential foundation. SVD, conditioning, iterative methods — elegant and rigorous. Anyone writing simulation code needs this.

**Trefethen — Approximation Theory and Approximation Practice** (free PDF, extended edition) explains why spectral methods work. Chebyshev polynomials as the computational physicist's secret weapon.

**Higham — Accuracy and Stability of Numerical Algorithms** (2nd edition) is the definitive reference on floating-point and numerical stability. Consult when things go wrong.

**Boyd — Chebyshev and Fourier Spectral Methods** (free PDF from author) provides comprehensive spectral methods for PDEs.

**LeVeque — Finite Difference Methods for Ordinary and Partial Differential Equations** and **Finite Volume Methods for Hyperbolic Problems** are clear, careful treatments with code.

### Finite Elements

**Hughes — The Finite Element Method** (Dover) provides systematic development of weak forms and variational formulations from Stanford/Caltech courses. *Start here for FEM.*

**Zienkiewicz, Taylor & Zhu — The Finite Element Method** (3 volumes, 8th edition) is the comprehensive reference from the field's founder. More encyclopedic than Hughes; use as reference.

**Brenner & Scott — The Mathematical Theory of Finite Element Methods** provides rigorous functional analysis foundations. The mathematics behind convergence.

**Ern & Guermond — Theory and Practice of Finite Elements** bridges mathematical rigour and practical implementation.

**Lectures:** Klaus-Jürgen Bathe's MIT OCW course (RES.2-002) teaches FEM through video—legendary clarity. His textbook *Finite Element Procedures* (2nd edition, 2014) provides the written companion.

### Computational Fluids

**Ferziger, Perić & Street — Computational Methods for Fluid Dynamics** (4th edition) is the standard CFD text with sample codes.

**Moukalled, Mangani & Darwish — The Finite Volume Method in Computational Fluid Dynamics** provides modern treatment with OpenFOAM orientation.

### Molecular Dynamics

**Frenkel & Smit — Understanding Molecular Simulation** explains the physics behind MD and Monte Carlo algorithms.

**Rapaport — The Art of Molecular Dynamics Simulation** provides complete programs and implementation details.

### Multibody Dynamics & Robotics

**Featherstone — Rigid Body Dynamics Algorithms** is THE reference for O(N) recursive algorithms. Spatial vector algebra unifying linear and angular quantities. Essential for robotics and simulation.

**Lynch & Park — Modern Robotics** (textbook free, Coursera, YouTube) bridges geometric mechanics to working code using SE(3) and product of exponentials.

### Multiscale

**Tadmor & Miller — Modeling Materials** is the first integrated atomistic-continuum presentation. Exceptional pedagogical clarity—"crystal clear" from quantum mechanics through quasicontinuum methods.

### Modern Computational Methods

**Karniadakis et al. — Physics-Informed Neural Networks** (PINN) literature—the original papers and DeepXDE documentation establish foundations for embedding physical laws in neural networks.

**Brunton & Kutz — Data-Driven Science and Engineering** bridges dynamical systems, machine learning, and control. Sparse regression, DMD, Koopman operators. Free PDF and YouTube lectures.

**Raissi, Perdikaris & Karniadakis** — foundational PINN papers (Journal of Computational Physics, 2019) for physics-constrained learning.

The **JAX ecosystem** (Google) enables differentiable physics: automatic differentiation through ODE/PDE solvers, GPU acceleration, composable transformations. JAX + Flax/Equinox is becoming standard for research. Julia's **DifferentialEquations.jl** and **SciML** ecosystem offer similar capabilities with different tradeoffs.

For structure-preserving machine learning: **Greydanus** (Hamiltonian Neural Networks), **Cranmer** (Lagrangian Neural Networks), **Chen** (Neural ODEs).

**Lectures:** Steve Brunton's YouTube channel covers data-driven methods extensively. MIT 18.337 (Parallel Computing and Scientific Machine Learning).

---

## Applied Mechanics

### Vibrations

**Den Hartog — Mechanical Vibrations** (Dover) is the MIT classic. 233 problems. Standard for 80+ years.

**Meirovitch — Fundamentals of Vibrations** provides rigorous graduate treatment.

**Ewins — Modal Testing** is the standard for experimental modal analysis.

### Acoustics

**Pierce — Acoustics** is wave propagation done with mathematical rigour.

**Morse & Ingard — Theoretical Acoustics** provides comprehensive theoretical treatment.

### Machine Design

**Shigley — Mechanical Engineering Design** (11th edition) is the "holy grail" of machine design for 50+ years.

**Roark — Formulas for Stress and Strain** contains 5,000+ formulas. The desk reference every structural engineer owns.

**Norton — Design of Machinery** (6th edition) covers mechanism synthesis with 82 video lectures.

### Vehicle & Aerospace

**Gillespie — Fundamentals of Vehicle Dynamics** (SAE) is the "most significant vehicle dynamics book of our time."

**Milliken & Milliken — Race Car Vehicle Dynamics** provides comprehensive treatment of high-performance vehicle behaviour.

**Anderson — Fundamentals of Aerodynamics** is the standard aerospace text.

**Zipfel — Modeling and Simulation of Aerospace Vehicle Dynamics** (4th edition) uses tensor methods with open-source C++ code.

**Lectures:** NASA JPL's *Basics of Space Flight* (free online) trains actual mission engineers.

---

## Biomechanics

**Fung — Biomechanics trilogy** (Mechanical Properties of Living Tissues, Biodynamics of Circulation, Biomechanics of Motion) established the field. From the father of biomechanics.

**Humphrey & O'Rourke — An Introduction to Biomechanics** (3rd edition, 2024) provides modern unified continuum treatment of biosolids and biofluids.

**Winter — Biomechanics and Motor Control of Human Movement** (5th edition, 2023) is the seminal technical text for motion analysis.

**Cowin — Bone Mechanics Handbook** is definitive for hard tissue, from cell biology through poroelasticity.

**Lighthill — Mathematical Biofluiddynamics** (SIAM) covers biological fluid mechanics from the pioneer.

**Holzapfel & Ogden — CISM volumes** on cardiovascular and biological tissue mechanics represent the research frontier.

**Lectures:** MIT 20.310J covers molecular through tissue scale biomechanics.

---

## Micro- & Nanoscale Mechanics

### Micromechanics

**Nemat-Nasser & Hori — Micromechanics** is the definitive treatise on homogenisation with rigorous variational methods.

**Mura — Micromechanics of Defects in Solids** establishes the foundational eigenstrain/Eshelby approach.

**Aboudi — Micromechanics of Composite Materials** (with NASA MATLAB codes) provides computational implementation.

### Nanomechanics & MEMS

**Senturia — Microsystem Design** is the MEMS bible from MIT's pioneer. Fabrication, mechanics, heat flow, system dynamics.

**Cleland — Foundations of Nanomechanics** uniquely treats quantum mechanical aspects of mechanical systems.

**Freund & Suresh — Thin Film Materials** is "a masterpiece" (Hutchinson, Nix) on mechanics of thin films.

### Multiscale

**Tadmor & Miller — Modeling Materials** bridges atomistic and continuum seamlessly.

**Lectures:** MIT 6.777J MEMS provides complete course materials.

---

## Geomechanics & Geophysics

### Soil Mechanics

**Schofield & Wroth — Critical State Soil Mechanics** is the Cambridge foundation.

**Muir Wood — Soil Behaviour and Critical State Soil Mechanics** is the definitive modern treatment with strong mathematical foundation.

### Rock Mechanics

**Jaeger, Cook & Zimmerman — Fundamentals of Rock Mechanics** (4th edition) has been authoritative since 1969.

### Seismology & Earthquakes

**Aki & Richards — Quantitative Seismology** is "The Bible" of theoretical seismology. Wave propagation and source mechanics.

**Scholz — The Mechanics of Earthquakes and Faulting** (3rd edition) provides unified treatment of brittle tectonics including rate-state friction.

### Geophysical Fluid Dynamics

**Vallis — Atmospheric and Oceanic Fluid Dynamics** (2nd edition, 900+ pages) is "The Great Book of the field."

**Pedlosky — Geophysical Fluid Dynamics** is the classic treatment.

**Lectures:** Woods Hole GFD Summer School archives lectures by world experts.

---

## Astrophysical & Planetary Mechanics

### Celestial Mechanics

**Murray & Dermott — Solar System Dynamics** is the benchmark with Mathematica software. Two-body through chaos.

**Danby — Fundamentals of Celestial Mechanics** provides rigorous classical treatment.

### Galactic Dynamics

**Binney & Tremaine — Galactic Dynamics** (2nd edition) — "We will all study from it and come to know it better than the Bible" (Bahcall). Potential theory, stellar orbits, disk dynamics, dark matter. 200+ problems.

**Heggie & Hut — The Gravitational Million-Body Problem** covers collisional dynamics and N-body methods.

### Stellar Structure

**Kippenhahn, Weigert & Weiss — Stellar Structure and Evolution** (2nd edition) covers stellar interior physics.

### Astrodynamics

**Bate, Mueller & White — Fundamentals of Astrodynamics** (USAF Academy, 2nd edition 2020) is the standard text.

**Vallado — Fundamentals of Astrodynamics and Applications** provides comprehensive modern treatment.

**Lectures:** NASA JPL's *Basics of Space Flight* trains mission engineers. MIT 16.346 covers spacecraft navigation.

---

## The Landau-Lifshitz Course

The ten volumes of the *Course of Theoretical Physics* constitute the most elegant unified treatment of physics ever written:

1. **Mechanics**
2. **The Classical Theory of Fields**
3. **Quantum Mechanics**
4. **Quantum Electrodynamics** (with Berestetskii & Pitaevskii)
5. **Statistical Physics, Part 1**
6. **Fluid Mechanics**
7. **Theory of Elasticity**
8. **Electrodynamics of Continuous Media**
9. **Statistical Physics, Part 2**
10. **Physical Kinetics**

Working through the complete course is one of the great self-education projects in physics.

---

## Open Lecture Courses

The revolution in open educational resources means world-class instruction is now freely available. These are the essential video lectures and notes.

### Cambridge — David Tong

The backbone of free theoretical physics education. Comprehensive lecture notes with problem sheets, many with accompanying video (Perimeter PSI recordings).

| Course | Level | Notes |
|--------|-------|-------|
| Classical Dynamics | Undergraduate | Lagrangian/Hamiltonian mechanics |
| Statistical Physics | Undergraduate | Ensembles through phase transitions |
| Kinetic Theory | Graduate | Boltzmann equation, transport |
| Statistical Field Theory | Graduate | Renormalisation group, critical phenomena |
| Quantum Field Theory | Graduate | Full course with PSI video |
| Gauge Theory | Graduate | Yang-Mills, instantons, monopoles |
| General Relativity | Graduate | Differential geometry through black holes |
| Cosmology | Undergraduate | Expanding universe, structure formation |
| String Theory | Graduate | Bosonic string, CFT basics |
| Particle Physics / Standard Model | Various | From pop-science to full mathematical treatment |
| Fluid Mechanics | Undergraduate | Navier-Stokes through turbulence |
| Quantum Hall Effect | Advanced | Chern-Simons, edge states |

Available at: damtp.cam.ac.uk/user/tong/teaching.html

### MIT OpenCourseWare

The original and still essential. Key physics courses with full video:

| Course | Instructor | Notes |
|--------|------------|-------|
| **8.01 Classical Mechanics** | Walter Lewin | Legendary demonstrations, physical intuition |
| **8.02 Electricity & Magnetism** | Walter Lewin | The definitive introductory E&M course |
| **8.03 Vibrations & Waves** | Walter Lewin | Completes the Lewin trilogy |
| **8.04/8.05/8.06 Quantum Physics I-III** | Barton Zwiebach | Complete undergraduate QM sequence |
| **8.033 Relativity** | — | Special relativity |
| **8.09 Classical Mechanics III** | — | Graduate analytical mechanics |
| **8.321/8.322 Quantum Theory I-II** | — | Graduate quantum mechanics |
| **8.323/8.324/8.325 QFT I-II-III** | — | Graduate QFT sequence |
| **8.333/8.334 Statistical Mechanics I-II** | Mehran Kardar | Particles and Fields — exceptional |
| **8.962 General Relativity** | Scott Hughes | 2020 recordings, gravitational waves emphasis |
| **RES.2-002 Finite Element Procedures** | Klaus-Jürgen Bathe | The legendary FEM course |
| **2.25 Advanced Fluid Mechanics** | — | Graduate fluids |

### Yale Open Courses — Ramamurti Shankar

**Fundamentals of Physics I & II** — Shankar is a master teacher. These undergraduate courses (PHYS 200/201) have been viewed over 20 million times. Covers mechanics, thermodynamics, waves, E&M, optics, and quantum mechanics. Companion textbooks available. Praised by Susskind as "excellent for teaching and learning introductory physics."

Available at: oyc.yale.edu/physics

### NPTEL / IIT — V. Balakrishnan

**Classical Physics** (38 lectures, IIT Madras) — One of the best lecture series in existence. Covers Newtonian mechanics through Hamiltonian dynamics, chaos, statistical mechanics, and special relativity with both physical intuition and mathematical rigor. Balakrishnan's teaching style is legendary.

**Quantum Physics** (31 lectures) — Linear algebra foundations through advanced quantum mechanics.

**Selected Topics in Mathematical Physics** — Deeper mathematical methods.

**Topics in Nonlinear Dynamics** — Dynamical systems and chaos.

**Physical Applications of Stochastic Processes** — Langevin, Fokker-Planck, and applications.

Combined views exceed 6 million. Available on NPTEL YouTube channel.

### Stanford — Leonard Susskind

**The Theoretical Minimum** series provides honest foundations without sacrificing correctness:

- Classical Mechanics
- Quantum Mechanics  
- Special Relativity & Classical Field Theory
- General Relativity
- Cosmology
- Statistical Mechanics
- Quantum Field Theory (Advanced)
- String Theory

Companion books available. Ideal preparation before Landau or as teaching resource.

### Frederic Schuller

**Lectures on the Geometric Anatomy of Theoretical Physics** (28 lectures) — Builds mathematical physics from propositional logic through topology, manifolds, bundles, connections, and gauge theory. Exceptional rigor. Simon Rea's transcribed notes available.

**International Winter School on Gravity and Light** (24 lectures, 2015) — "Unequivocally the best, most lucid, and well-constructed lecture series on General Relativity" (Ernest Yeung). Develops GR from first principles with full mathematical precision. LaTeX notes available.

**Lectures on Quantum Theory** — Rigorous quantum mechanics from scratch with Rigged Hilbert spaces. Joint notes by Simon Rea and Richie Dadhley.

### Tobias Osborne (Hannover)

**Symplectic Geometry & Classical Mechanics** (Winter 2017-18) — Geometric mechanics for those with differential geometry background. Connects symplectic structure to Hamiltonian dynamics. Notes by multiple transcribers available.

**Quantum Field Theory** — Full course with transcribed notes on GitHub.

**Advanced Quantum Theory** — Many-particle QM, scattering, relativistic QM.

**Quantum Information Theory** — Comprehensive graduate treatment.

### University of Washington — Steve Brunton

**Data-Driven Science and Engineering** (YouTube, ~200 videos) — The essential modern course bridging dynamical systems, machine learning, and control. Covers SVD, DMD, sparse regression, Koopman operators, reduced-order models, physics-informed learning. Brunton's ability to explain sophisticated mathematics visually is exceptional. Companion textbook free online.

**Control Bootcamp** — Comprehensive modern control theory with MATLAB/Python.

### University of Michigan — Krishna Garikipati

**Lectures on Continuum Physics** (~130 segments) — Comprehensive treatment emphasizing both solids and fluids equally. Mathematical rigor with physical props. Covers kinematics, kinetics, constitutive relations, thermomechanics, variational principles, mass transport. "I know of no other way to do continuum physics" than mathematically.

**Introduction to Finite Element Methods** (~50 hours) — From functional analysis foundations to implementation. Develops competent FEM code developers.

Both available on YouTube and Open Michigan.

### Harvard — Sidney Coleman

**Physics 253: Quantum Field Theory** (1975-76) — Coleman was "the master teacher of quantum field theory." Video quality reflects the era, but Coleman's legendary wit and insight remain. Brian Hill's handwritten notes (now LaTeX transcribed, arXiv:1110.5013) accompany the lectures. The book *Lectures of Sidney Coleman on Quantum Field Theory* (2019) captures the course.

"Sidney Coleman's course on quantum field theory was one of the most memorable and enjoyable experiences of my physics education." — Sean Carroll

### Perimeter Institute PSI

The Perimeter Scholars International program makes graduate-level courses freely available:

- Quantum Field Theory (multiple instructors including Tong)
- Condensed Matter
- Quantum Information
- Cosmology  
- String Theory
- Statistical Mechanics

Research-level courses from leading practitioners.

### Additional Essential Resources

| Resource | Coverage |
|----------|----------|
| **ICTP Diploma Programme** | Full graduate physics curriculum, streaming lectures |
| **Woods Hole GFD Summer School** | Geophysical fluid dynamics, world experts |
| **TASI Summer Schools** | Particle physics and string theory, annual topics |
| **Les Houches** | Advanced summer school proceedings |
| **eigenchris (YouTube)** | Visual tensor calculus and differential geometry |
| **3Blue1Brown** | Mathematical visualisation (linear algebra, calculus) |

### Continuum & Computational Mechanics

| Course | Institution | Instructor |
|--------|-------------|------------|
| Continuum Physics | Michigan | Garikipati |
| Intro to FEM | Michigan | Garikipati |
| FEM for Solids & Structures | MIT | Bathe |
| Computational Continuum Mechanics | NPTEL/IIT Guwahati | Gautam |
| Applied Mechanics of Solids | — | Bower (online text) |
| CFD Python: 12 Steps to Navier-Stokes | — | Lorena Barba |

### Robotics & Dynamics

**Modern Robotics** (Lynch & Park) — Free textbook, Coursera specialisation, YouTube playlist. Product of exponentials, SE(3) kinematics, dynamics, control. Bridges geometric mechanics to working code.

---

## Study Pathways

No one masters all of this. These pathways offer coherent routes through the material—choose based on your goals, go deep, and return when ready to branch out.

**The Geometric Path** (mathematical physics, 2-3 years)
Schuller (Geometric Anatomy) → Arnol'd → Cannas da Silva → Marsden-Ratiu → Marsden-Hughes → Wald
*For those who want the mathematical structures underlying physics. You'll emerge thinking in manifolds and seeing symmetry everywhere.*

**The Landau Path** (theoretical physics, 3-5 years)
Landau-Lifshitz Vols. 1, 2, 3, 5, 6, 7, 9, 10 — the complete course
*The classical education in theoretical physics. Demands discipline. Rewards it.*

**The Executable Path** (computational mechanics, 1-2 years)
SICM → Marsden (variational integrators) → Featherstone → Lynch-Park
*For those who believe code is understanding. You'll be able to simulate what others can only write equations for.*

**The Computational Path** (simulation, 2-3 years)
Trefethen-Bau → Hughes (FEM) → Simo-Hughes (Plasticity) → Ferziger-Perić (CFD) → Frenkel-Smit (MD)
*The working tools of computational science. From numerical foundations to production simulation.*

**The Modern Computational Path** (differentiable physics, 1 year)
Brunton-Kutz → JAX/Julia ecosystem → PINNs → structure-preserving ML
*Where classical simulation meets machine learning. The current frontier.*

**The Dynamical Systems Path** (applied mathematics, 1-2 years)
Strogatz → Guckenheimer-Holmes → Wiggins → Khalil
*Nonlinear dynamics and control. Essential for anyone working with complex systems.*

**The Condensed Matter Path** (many-body physics, 2-3 years)
Ashcroft-Mermin → Altland-Simons → Coleman (Many-Body) → Fradkin
*From electrons in solids to topological phases. Where quantum meets materials.*

**Problem Mastery** (ongoing)
Kotkin-Serbo (Classical) → Zettili (QM) → Lightman et al. (GR) → Kubo (Statistical)
*Reading is not understanding. Work problems.*

---

*These texts define their fields. No one reads them all—choose your path, go deep, and trust that the others will be here when you need them. The lectures are freely available to anyone with the dedication to work through them.*
