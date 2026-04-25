---
title: "experiencing eureka"
date: 2026-04-24
categories: til
---

i encountered a math question. 

Find the length of the arc of the parabola $x^2 = 4y$ from the vertex to the point $x = 2$, where $x \in \mathbb{R}$ and $y \in \mathbb{R}$.

this seemed so new. i've given enough math/science exams to have had solved a lot of questions. but this i couldn't think how to even proceed. lenght of an arc? how?

but this question was from a paper whose syllabus is high school math. so it meant i knew the tools to solve it.

i went to llms and since i've had multiple threads about math questions, i asked them this - 

>dont tell me the answer or how to solve. basis this thread, do you think i have the tools to solve this. dont even tell me any aproach or name of tool i want to try myself

it said - 

>Yes—you already have the required tools to solve this.

so i got in. i tried finding ways. calculus seemed like the only tool that could help. maybe i could take slices of the arc then integrate. 

i tried using g(x) = f(x) + epsilon. maybe if i find the area between these two curves, itll give me the lenght. but it just comes out to be 2*epsilon.

then i tried making triangles with base dx and finding the equation for hypotenuse and then integrating that. didn't work.

i then looked at trapeziums with points (x,x+dx,f(x),f(x+dx)) and then using the triangle on top to figure out the hypotenuse. it came out to be $dx\left(\frac{\left(\sqrt{dx + 2x\,dx}\right)^2}{4} + 1\right)$. how am i supposed to integrate an expression that has dx inside a square root.

was i even doing the right thing. is this even allowed in calculus?

then i realised instead of using f(x+dx) - f(x) for height, i could use dx*derivative of f. and that was it. i got an expression that i had to integrate. i couldn't do it myself, i've forgotten trig substition, so used the internet for it. 

i had asked the LLM to check my answer and just return whether it is right or wrong. after inputting 3 wrong answers, i input 2.29. it said - 

> You got it! Right on the money.

i stood there in silence staring at those words. 

feels like discovering maths. 

