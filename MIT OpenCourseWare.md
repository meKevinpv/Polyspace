Status: #Doing 
Tags: #Programming #Algorithms #Lecturenotes
Links: [Lecture](https://www.youtube.com/watch?v=ZA-tUyM_y7s)
MOC: 
___
# MIT OpenCourseWare
Goals of the course:
- Solving computational problems
- Prove correctness
- Argue efficiency
- Communication of these ideas

### Defenition of a problem
````mermaid
graph LR

a[input]
b[solution]
a-->|Routes|b
````
The goal of algorithms is to solve general problems with arbitrarily sized inputs.
**You can prove this is true by:**
1. Testing the base statement, meaning the smallest possible input it can be tested against.
1. Testing against the largest (k) inputs within scope and seeing if every output state can be reached.
This concept is called *Inductive test*

### Asymptotic analysis
To test weather an algorithm is efficient we use *Asymptotic analysis*, which is a method to describe behaviour at the mathematical limits (in this case in terms of input).

n *Size of input*
O *Upper bounds of input*
Ω (Omega) *Lower bounds of input*
Θ (Theta) *Bound from above and below*

Results of Asymptotic time efficient (generally):
1. Θ(**i**) > Constant time
1. Θ(log**n**)
1. Θ(**n**) > Linear time
1. Θ(**n**log**n**)
1. Θ(**n**^2)
1. Θ(**n**^c) > Polynomial time

>Fun little sidenote: Old computers used to run a maximum WORD size, the ammount of bits that go from memory in 1 adress to the cpu, of 32 bits, nowadays that is 64 bits. This functionally meant that memory had to be partitioned in 4GB chunks because that is *2(io states) to the power of 32*, doing that same calculation nowadays with 64 bit systems that would come up to about 20 exabyes. For context this is double the **total** storage of Google worldwide.

*End of Lecture 1*

[Lecture 2, Data Strucutres and Dynamic Arrays](https://youtu.be/CHhwJjR0mZA)
