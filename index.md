# Overview

These are activities that students work on during a weekly 50--minute recitation for PHYS 260 at GMU. To maximize time that students spend working on problems, I typically give at most a 10--minute review. Often, my 10--minute overview involves working through an example that is nearly identical to the first problem. If many students are stuck on a part of the problem, I will interrupt the class and have students guide to the answer.

These tutorials were written in collaboration with Jessica Rosenberg over the course of four semesters. The tutorials were revised from semester-to-semester based on observations made while using them.

The length of the tutorials are such that 1--2 students out of 30 will finish completely. 

%**Motivation**

%In the past, I would solve problems at the board for 40 minutes and then give a quiz at the end. The quiz required students to reproduce something that I had expained several times or to reproduce the set--up of a problem. Based on the results of these very simple quizes, few students got much out of my presentation. In addition, often students would ask for help on homework problems after the recitation that were nearly identical to the problem covered in recitation. It was clear from their questions that their notes from, or memory of, my presentation were of little use.

%Prior to working on these, approximately 1/2--2/3 of the students will have attended two 75--minute lectures covering the associated chapter and content.

%The problems on these activities are generally basic and simple. They emphasis the basic calculations required to solve problems rather than concepts. I generally explain the concepts and ask questions about them while the students are solving problems or when I go over a solution.

%However, I find that most students only have time to attempt half of the problems and there are many questions. Based on experience, I assume that after two 75--minute lectures, most students have only knowledge of keywords and associated concepts and are not able to solve problems that require more than identifying the equation to use given variables in the problem statement.

%For my recitations, students turn in their work at the end of class and I hand out solutions. The minimum score for their work is 7/10 points. Scores below a 10 are for students who made little progress and did not ask questions or work with others. I typically indicate wrong answers but do not take points off unless almost everything is very wrong. I also hand out solutions at the end of class and tell students that in order to have any chance of a passing score on the exams, they must have mastered the problems in this tutorial prior to exams. I also encourage them to review by re--solving the tutorial problems again without referring to their previous work or solutions.

# Using

The source files for all activities are available at [Overleaf]((https://www.overleaf.com/read/btssfxsjgyzr) and [GitHub](https://github.com/rweigel/phys260); all files are available in a [zip](https://github.com/rweigel/phys260/archive/refs/heads/master.zip) file.

In each subdirectory at https://github.com/rweigel/phys260 there is a file named `README.md` with notes written after class and after reviewing student work.

The master document is the `.md` file, which is converted to `.html` and `.tex`. The `.pdf` files are based on the `.html` file. The `.tex` files are auto--generated from the `.md` files and a `.pdf` created with the `.tex` file may look different than the one stored in the repository.

If you have corrections, comments, or suggestions please [submit an issue](https://github.com/rweigel/phys260/issues) or email `rweigel@gmu.edu`. 

The figures were created using [MathCha](https://www.mathcha.io/). To edit a figure using MathCha, open the MathCha links in the comments in the `.md` or `.tex` file with a web browser. The `.tikz` files can also be edited using a [tikz editor](https://www.google.com/search?q=tikz+editor).

# Modules

## Vector Review

* Given a diagram showing a vector with a known magnitude and direction, find components in unit vector notation. Deal with the fact that horizontal component is not always $\cos$ of angle given.
* Given a diagram showing vector components, find magnitude and direction.
* Given a diagram showing two vectors with known magnitudes and directions, find components in unit vector notation. Then find net vector magnitude and direction.

## Electric Force Between Point Charges (Coulomb's Law)

* Background material:
  * PowerPoint: []()
  * Reading: [Section 21.3 of Young and Freedman 2015, 14th Edition](https://drive.google.com/file/d/1JS_pBuNEwXdz9IzpSBFPJffgVacZmqN7/view?usp=sharing_remove_)
  * Videos
    * [Solving 2-- and 3--charge problems in 1-D](https://www.youtube.com/watch?v=kCp5yYjo9zE): Very basic, and long (35 minutes)
    * [3--charge problem](https://www.youtube.com/watch?v=t6S-PX14Pu4): Charges at points of equilateral triangle
    * [4--charge problem](https://www.youtube.com/watch?v=t6S-PX14Pu4): Charges at corners of square.

* Activity: Using Coulomb's law to find the electric force magnitude and direction between two charges (without $\rhat$ notation)
  * Documents:
| [pdf](Electric_Force/Electric_Force.pdf)
| [pdf solns](Electric_Force/Electric_Force-solutions.pdf)
| [html](Electric_Force/Electric_Force.html)
| [instructor notes](Electric_Force/README.html)
|
  * Source Files:
| [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr)
| [Github](https://github.com/rweigel/phys260/tree/master/Electric_Force)
|

* Demonstrations:
  * [Estimating charge using balloons](https://youtu.be/K-8nCXY-iSI?t=29) -- Balloons are charged and hung from a strings attached to a common point on the ceiling. Their charge is estimated using the distance between the balloons.
  * [Comparing Coulomb's law to experimental results](https://www.youtube.com/watch?v=B5LVoU_a08c) -- An experiment measuring the forces between two charged spheres using an experimental set--up similar to Coulomb's.

## Electric Field

* Background material:
  * Videos
    * [Electric Field Definition](https://www.youtube.com/watch?v=_4VC3IHbuW8) -- Includes details on how the electric field is related to electric force.
  * Reading: [Section 21.4 of Young and Freedman 2015, 14th Edition](https://drive.google.com/file/d/1JS_pBuNEwXdz9IzpSBFPJffgVacZmqN7/view?usp=sharing_remove_)

* Activity
Computing the electric field due to one and three point charges (without $\rhat$ notation)
  * Documents:
| [pdf](Electric_Field/Electric_Field.pdf)
| [pdf solns](Electric_Field/Electric_Field-solutions.pdf)
| [html](Electric_Field/Electric_Field.html)
| [instructor notes](Electric_Field/README.html)
|
  * Source Files:
| [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr)
| [Github](https://github.com/rweigel/phys260/tree/master/Electric_Field)
|

* Visualizations
  * [3-D visualizations of vector fields](https://www.youtube.com/watch?v=rB83DpBJQsE&t=185s). Although the video covers advanced vector calculus, is has several vector field visuals that can be used when explaining how to imagine vector fields.
  * [2-D visualization of vector field due to two charges](https://www.geogebra.org/m/MAsvESCX) -- This interactive online Geogebra application can be used to demonstrate superposition and the fact that the electric field points in the same direction as the force on a test charge. A good review is to hide the test charge and ask students to predict the direction the force will be on it.
  * [PhEt Charges and Fields Simulation](https://phet.colorado.edu/sims/html/charges-and-fields/latest/charges-and-fields_all.html) -- Similar to the Geogebra example above.

## The $\rhat$ Unit Vector

* Activity: Find electric field using $\rhat$ notation.
  * Documents:
| [pdf](rhat/rhat.pdf)
| [pdf solns](rhat/rhat.pdf)
| [html](rhat/rhat.html)
| [instructor notes](rhat/README.html)
|
  * Source Files:
| [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr)
| [Github](https://github.com/rweigel/phys260/tree/master/rhat)
|

## Superposition and Symmetry

* Activity: Find electric force and field due to multiple charges
  * Documents:
| [pdf](Superposition_and_Symmetry/Superposition_and_Symmetry.pdf)
| [pdf solns](Superposition_and_Symmetry/Superposition_and_Symmetry.pdf)
| [html](Superposition_and_Symmetry/Superposition_and_Symmetry.html)
| [instructor notes](Superposition_and_Symmetry/README.html)
|
  * Source Files:
| [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr)
| [Github](https://github.com/rweigel/phys260/tree/master/Superposition_and_Symmetry)
|

## Continuous Charge Distributions

* [Instructor Notes](https://github.com/rweigel/phys260/tree/master/Continuous_Charge_Distributions/README.md) 
* Documents: | [pdf](Continuous_Charge_Distributions/Continuous_Charge_Distributions.pdf) | [pdf solns](Continuous_Charge_Distributions/Continuous_Charge_Distributions-solutions.pdf) |
* Source: | [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr) | [Github](https://github.com/rweigel/phys260/tree/master/Continuous_Charge_Distributions) | [Markdown](Continuous_Charge_Distributions/Continuous_Charge_Distributions.md) | 
* Covered in [Section 21.5](https://drive.google.com/file/d/1JS_pBuNEwXdz9IzpSBFPJffgVacZmqN7/view?usp=sharing_remove_) of Young and Freedman 2015, 14th Edition and [Section 1.5](https://openpress.usask.ca/physics155/chapter/1-5-calculating-electric-fields-of-charge-distributions/) of Introduction to Electricity, Magnetism, and Circuits by Ling et al.

## Electric Flux

* [Instructor Notes](https://github.com/rweigel/phys260/tree/master/Electric_Flux/README.md) 
* Documents: | [pdf](Electric_Flux/Electric_Flux.pdf) | [pdf solns](Electric_Flux/Electric_Flux-solutions.pdf) |
* Source: | [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr) | [Github](https://github.com/rweigel/phys260/tree/master/Electric_Flux) | [Markdown](Electric_Flux/Electric_Flux.md) | 

## Enclosed Charge

* [Instructor Notes](https://github.com/rweigel/phys260/tree/master/Enclosed_Charge/README.md) 
* Documents: | [pdf](Enclosed_Charge/Enclosed_Charge.pdf) | [pdf solns](Enclosed_Charge/Enclosed_Charge-solutions.pdf) |
* Source: | [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr) | [Github](https://github.com/rweigel/phys260/tree/master/Enclosed_Charge) | [Markdown](Enclosed_Charge/Enclosed_Charge.md) | 

## Electric Potential

* [Instructor Notes](https://github.com/rweigel/phys260/tree/master/Electric_Potential/README.md) 
* Documents: | [pdf](Electric_Potential/Electric_Potential.pdf) | [pdf solns](Electric_Potential/Electric_Potential-solutions.pdf) |
* Source: | [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr) | [Github](https://github.com/rweigel/phys260/tree/master/Electric_Potential) | [Markdown](Electric_Potential/Electric_Potential.md) | 

## Capacitance

* [Instructor Notes](https://github.com/rweigel/phys260/tree/master/Capacitance/README.md) 
* Document: | [pdf](Capacitance/Capacitance.pdf) | [pdf solns](Capacitance/Capacitance-solutions.pdf) |
* Source: | [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr) | [Github](https://github.com/rweigel/phys260/tree/master/Capacitance) | [Markdown](Capacitance/Capacitance.md) |

## Kirchhoff's Circuit Laws

* [Instructor Notes](https://github.com/rweigel/phys260/tree/master/Kirchhoffs_Laws/README.md) 
* Document: | [pdf](Kirchhoffs_Laws/Kirchhoffs_Laws.pdf) | [pdf solns](Kirchhoffs_Laws/Kirchhoffs_Laws-solutions.pdf) |
* Source: | [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr) | [Github](https://github.com/rweigel/phys260/tree/master/Kirchhoffs_Laws) | [Markdown](Kirchhoffs_Laws/Kirchhoffs_Laws.md) | 
* See also [Section 10.5 of University Physics Volume 2 by Ling et al.](https://pressbooks.online.ucf.edu/osuniversityphysics2/chapter/kirchhoffs-rules/)

## RC Circuits

* [Instructor Notes](https://github.com/rweigel/phys260/tree/master/RC_Circuits/README.md) 
* Document: | [pdf](RC_Circuits/RC_Circuits.pdf) | [pdf solns](RC_Circuits/RC_Circuits-solutions.pdf) |
* Source: | [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr) | [Github](https://github.com/rweigel/phys260/tree/master/RC_Circuits) | [Markdown](RC_Circuits/RC_Circuits.md) | 

## Lorentz Force Law

* [Instructor Notes](https://github.com/rweigel/phys260/tree/master/Lorentz_Force/README.md) 
* Document: | [pdf](Lorentz_Force/Lorentz_Force.pdf) | [pdf solns](Lorentz_Force/Lorentz_Force-solutions.pdf) |
* Source: | [Overleaf](https://www.overleaf.com/read/btssfxsjgyzr) | [Github](https://github.com/rweigel/phys260/tree/master/Lorentz_Force) | [Markdown](Lorentz_Force/Lorentz_Force.md) | 

## Lorentz Force Law on Wires

* [Instructor Notes](https://github.com/rweigel/phys260/tree/master/Lorentz_Force_Wires/README.md) 
* Document:
[pdf](Lorentz_Force_Wires/Lorentz_Force_Wires.pdf)
|
[pdf solns](Lorentz_Force_Wires/Lorentz_Force_Wires-solutions.pdf)

* Source:
[Overleaf](https://www.overleaf.com/read/btssfxsjgyzr)
|
[Github](https://github.com/rweigel/phys260/tree/master/Lorentz_Force_Wires)
|
[Markdown](Lorentz_Force_Wires/Lorentz_Force_Wires.md) | 
