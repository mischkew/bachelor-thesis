# Platener - Generating 2D laser cuttable construction plans from 3D models

## Abstract

We present platener, a web service that converts 3D models originally
designed for 3D printing to a representation that can be fabricated
using a laser cutter.

Designing three-dimensional objects for laser cutting is difficult
today, because it requires users to break down their idea into a set
of two-dimensional parts and to add appropriate joints between these.
Both aspects require substantial engineering knowledge. Our service
eliminates the need for engineering knowledge by offering an
alternative workflow. In this workflow, users model their 3D idea
using a 3D editor of their choice; users then obtain the 2D
representation required for the laser cutter by converting their 3D
model with platener. As a side effect, this workflow allows converting
models from 3D printing model repositories; this is beneficial, as
those repositories already hold many more models as there currently
are models for laser cutting.

platener creates two-dimensional cutting plans as follows. First, it
identifies flat surfaces in the 3D model. Second, it locates laser
cuttable elements by finding plates of appropriate thicknesses as
pairs of parallel surfaces with appropriate distance. Third, the
software generates joints to connect the plates.

The software system is designed primarily with the objective of
converting functional objects, such as mechanical tools and
low-fidelity prototypes. Unlike existing conversion systems, such as
[123DMake](http://www.123dapp.com/make) and
[Brickify](http://brickify.it) it focuses on maintaining the
functional aspect and stability of the input model while still
enabling the benefits of laser cutting, such as the ability to use a
wider choice of materials.
