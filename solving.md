Problem Solving
===============

Humans are great problem solvers. Unfortunately, it is so intuitive that we are not consciously aware of the specifics of the process. This is a shame, as a deeper understanding of of our thought process could lead to techniques to improve decision making and a blueprint for the creation of intelligent machines.

Many scientists and philosophers have attempted to describe the problem-solving process. There were a lot of ideas, but no good way to know if they were correct. Then, in the mid 20th century, machines that could execute logical instructions were finally built - digital electric computers. Up until today, no theory of problem solving, past or present, has been able to run on these machines. I would not say that the theories were *wrong* but it appears that that are, at the very least, incomplete, ambiguous, and/or dependent on other unexplained processes. (Some believe that the reason no general intelligence has been implemented on a computer is that it has possesses sort of magic that makes it not representable in a clear and rigorous manner. This is utter hogwash.)

Even though problem-solving is not well understood, early computer scientists needed to solve problems anyhow. Using computers for rapid and accurate mathematical calculations is valuable, but a human still had to discover which calculations to run. An even bigger difficulty is that traditional mathematics is very good at solving certain types of problems, but completely incapable of solving others. (This isn't something most mathematicians like to publicize.) While working on the Manhattan Project, the amount of shielding needed to protect from neutron radiation ran into this difficulty, so a new technique was proposed: The Monte Carlo Method. Named after a casino, it approximates the solution to complex calculations using multiple random attempts.

When I say "approximates" what I mean is the results of a Monte Carlo calculation have finite precision. Before beginning a calculation, one should determine the minimum amount of precision required. (It's probably less than you think.) Traditional mathematics dislikes this, as their methods can be infinitely precise, but science and engineering have clear limits of precision, so this is not the problem pure mathematicians believe. This doesn't mean that Monte Carlo methods can't be extremely precise, but greater precision takes more time and effort so it is best to know the minimum tolerances the solution requires to keep from needlessly wasting resources.

Monte Carlo methods are a particular type of *stochastic process* which means it utilizes random values.

## Universal Problem Solving

The Monte Carlo method solved a previously unsolvable problem using the brute force of computers. We should be able use similar techniques to solve other problems. Here is a general set of steps that can be used to find the solution to any problem (that I have discovered so far.)

### Step 1: Define the Characteristics of the Solution

With a thorough understanding of the problem, we should know the characteristics of the correct answer, against which we can judge the quality of proposed solutions. I would hope that this step is also a part of traditional, deterministic methods, so that their answer is checked for correctness.

### Step 3: Determine the Solution Space

Using the definition of the solution in step #1, we should be able to determine a range that we are certain the solution lies inside. The smaller this range can be made, the more efficient that calculation.

Though this is not theoretically a necessary step, practical applications require it, as computing machinery have inherent limits in the range and precision of the numbers they represent. It is conceivable that a deep understanding of the solution set and some cleverness could define a solution space so small that it is equal to the answer. Indeed, this describes the process of deterministic math.

### Step 3: Test Possible Solutions

Now, pick some values from inside the solution set, test them, and record the results. How these are chosen is up to you: use a pseudo-random number generator, sample white noise, get a chicken do it, or even eschew randomness altogether and choose values at uniform intervals. Most techniques work, so use whatever seems appropriate to the particular problem.

### Step 4: Decide the Result

At some point - either the predetermined threshold of precision was reached or maybe you just ran out of time - the best solution is chosen. How the final answer is derived from an aggregation of test results can vary, but it is often the result with the highest test score.

### Optional Step 3.5: Adjust the Solution Set

In some types of calculations, we can narrow the range of possible solutions based on our testing results. After a certain number of possible solutions are tested, the scope of the solution set is reduced and a new round of solution testing begins. This is commonly called a "genetic" algorithm because each generation of solution tests inherit scope from the best of their ancestors.
