
# Email

In the directory Enclosed_Charge at https://www.overleaf.com/read/btssfxsjgyzr, there is an activity that I plan on using Monday (pdfs attached). If you want to make edits, the .tex version has a switch at the top to hide the solutions.

I used to cover the enclosed charge briefly when I covered Gauss's law until I realized that many students weren't able to compute the enclosed charge part (unless they remembered the answer). Instructors, including myself, and textbooks tend to spend the most time on the flux part of Gauss's law. This activity covers many parts that students need practice on (both at the freshman and junior level, I've found):

1. Plotting piecewise functions (the motivation for them plotting points is because many get stuck and I tell them to plot a few points first to give themself a hint)
2. Manipulating variables instead of numbers
3. Identifying how Q enclosed scales with the radius of the Gaussian volume (or other dimensions) and using this to check their plot and answers
4. Computing charge densities
5. Recalling formulas for volumes and areas (many don't know or recall that if they know the circumference of a circle, they can figure out the surface area of a cylinder and if they know the area of the circle, they can figure out its volume)

For the few students who have an easy time with these problems, I ask them to

1. draw the field lines for the charged object,
2. identify the conditions on the Gaussian volume such that the computation of flux through its surface is easy, and
3. compute the flux

I plan on spending 10 minutes doing one of the problems with the addition of doing 1.-3. above so they know the motivation for computing Q enclosed.

Bob

# Comments Before

ro -> rw

I always emphasize to students that final results should be in terms of the "given" variables of the problem when it is an algebraic problem. So, I would like to see questions 4. and 5. of each section ask explicitly for answers in terms of Q, not lambda or rho or sigma. I see the reason for doing it in terms of density in the earlier parts, but I think at some point they need to plug in the "givens": R, H, etc.

> Previously, I had them plotting Q_enclosed in terms of the variables given, but switched to using densities to lead them to the form of Q_enclosed that is used to compute the usual textbook formulas, which are typically given in terms of densities ... except for the case you mention below and outside a solid sphere.

In a similar vein, I don't see the need to ask for charge in terms of sigma in part 3 of section 5. I would rather have them realize that Q_encl is simply the total charge of the sphere when you are outside the sphere. I think telliing them they need to do an extra step might be more confusing than helpful. Maybe in this question we could just leave off the part that tells them what the answer should be in terms of, and then instructors could ask if they understand how to get it "the other way"?

> The motivation for asking for sigma was to ensure that they could compute a sigma. But it is awkward given they most likely see a formula in terms of Q and not sigma.
>
>Perhaps I could break the parallelism and in this problem give the charge density and ask for answers in terms of net charge. Or, note that this problem is a special case in the sense that we don't write E in terms of a charge density. Same for the solid sphere when outside.
>
>I'll put this discussion in my notes for consideration for revision next time. These are all good points that ideally should be addressed.

# Comments after

rw
1. ✓ Have a stand-alone section at the start for computing charge density given Q on all surfaces and volumes given.

2. Start problems with a density given.

3. Move two cylinder problems to the end. They appear in the more difficult Gauss' law problems, and students got stuck. I had to stop them and give answers so they had time for the other problems. (Even after my explanation and the answers, I noticed students still trying to answer them.) Add a discussion for the cylindrical shell problem about how it can be solved given a linear or surface charge density. The solid cylinder problem could be solved given a linear or volume charge density, but I don't recall ever seeing a problem where its linear density was given.

4. Add to the notes a definition of linear, surface, and volume charge density when the charge is uniformly distributed. I'm reluctant to give formulas for areas and volumes because it lets them think they don't need to know it without reference.

5. Students who had difficulty plotting the curve also had difficulty in writing down the value at various points. I'm not sure what to do about that. There could be a sentence that says "if the formula does not depend on r, ...". But the students who didn't realize this understood so little that I'm not sure it will help.

6. Add a question after the spherical shell and solid sphere problem that states "if the total charge is Q in both cases, is Q_enclosed for r>R the same?" Ideally, there would be a follow-up that makes the point that if Q is uniformly distributed on a shell, thick shell, solid sphere, or on an infinitesimal sphere, E will be the same outside. I'm still trying to think about how to address the issue about this you raised earlier.

7. I may add a question at the end that gives a non-uniform density for a solid sphere to make the point that the total charge/ total length, total charge/total area, and total charge/total volume formulas only work apply if the charge is uniformly distributed. Probably I'll give the integral formula for Q and show it gives the correct result for constant rho and then ask them to use it for rho that depends on r.

8. State that "charge enclosed" means the same thing as "charge inside of"

9. Some students were tripped up by the fact that I switched from having the Gaussian volume larger than the charged object for the cylinder problems to smaller for the sphere problems. I had not noticed it. I'm not sure if it is something to leave as-is, so they get in the habit of reading the problem statement, or to change so they don't get tripped up (because there is already enough to get tripped up on when trying the first time).

10. I usually have about 5 students that continue working for 5-10 minutes after the period ends. For this activity, there was more. I wonder if this is because they liked the problems, the exam is coming up, or they were the few students that only got an 8 or 9 out of 10 on the previous activity.

About 1/4 of the students required a significant amount of explanation for why a small sphere inside of a shell has no charge inside of it. I tried about four different explanations ... the only one that seemed to work is "if your hair is charge and I put a marble inside your skull, how much hair is inside the marble?". Probably I should bring visual aids next time, especially for the charged cylindrical shell, which stumped even more students.

----
ro

I thought it went really well in my classes and I liked the progression of the problems as is. I edited my version to ask for answers in terms of Q in the last step (while keeping it in terms of density in the previous steps). See attached.

I agree that the idea of doing a cylindrical shape in terms of surface charge density OR linear charge density is confusing to them and requires some discussion, especially because the book problems mostly use linear density. (Personally, I would just stick with surface charge density to avoid the confusion.) Not sure what to do about that because it would make it even longer.

My only other recommended change is in part 2, Line of Charge, it should be stated as r= L/100, etc, rather than h/100. I had a lot of groups that thought r= h/100 meant that h=100r and therefore changed when we changed the radius. Putting it in terms of L (the way the others are in terms of the physical radius, R) should help with that.

I found it very eye-opening that these "easy" Gauss problems required so much struggle from the students. I always feel that I have to give them a "hard" Gauss problem, eg. nested spheres, to make the problem non-trivial. Clearly these cases are non-trivial for the students. Thanks for developing this!  It was really worthwhile.

In Part 7, it should be stated that $r < L/2$ (not $r<L$), so that the diameter is not larger than $L$. (A student caught that one!)
