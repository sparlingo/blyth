# Model Thinking

## Week 1

## Week 2

## Week 3

## Week 4

### Tipping Points

#### Percolation Models

#### Contagion Models: Diffusion

#### Contagion Models: SIS

#### Classifying Tips

#### Measuring Tips

### Economic Growth

*Why Nations Fail*

Botswana vs Zimbabwe example: Botswana has grown quickly, Zimbabwe is stagnant

#### Exponential Growth

Economies tend do grow quickly when societies are at a low level of development, and then the growth rate tends to slow (catch up growth is easy). 

#### Solow Growth Model

$L_t$ = labor at time t; $K_t$ = capital at time t; $A_t$ = tech at time t; $O_t$ = Output

$O_t = A_t K_t^\beta L_t^{1-\beta}$

Growth requires creative destruction (Schumpeter). 

Piketty's Capital: The Power of a simple model

Returns to capital are greater than overall economic growth, so the rich get richer.

#### Questions

1. Which of the following is explained by a tipping point?

   a) residential segregation

   b) new home sales plummet 60%

   c) power outages through the eastern US

   d) Last year 2 bunnies, this year there are 40

2. In a building with 70 residents, a rumor spreads through a diffiusion process. When is diffusion greater: 15 people know the rumour, or 50?

3. A virus has a R0 of 9. What is the percentage that should be vaccinated?

4. In our disease model (SIS), R0 must be less than 1 in order to ensure that a disease will not spread. In this model, R0 is an example of what type of tipping point?

   Contextual or Direct?

5. There are 4 possible outcomes: one with probability 1/6, one 1/3, and two with 1/4. Calculate the diversity index. 

6. In order to attain a long-run equilibrium in the Basic Growth Model, which of the following must be true?

   a) Investment and output must be equal

   b) Savings rate and output must be equal

   c) Savings rate and depreciation must be equal

   d) Investment and depreciation must be equal

7. A country has a production function such that output equals $40*\sqrt K$ where k equals the amount of capital. If this country has 36 units of capital, what is its output?

8. If output equals $30 \sqrt K$ the savings rate equals 20% and equilibrium output equals 1200, what is the depreciation rate?

   a) 20%

   b) 5%

   c) 10%

   d) 15%

9. If output equals $40 \sqrt K$ the savings rate equals 10% and the depreciate rate is 20%, what is sthe long run equilibrium level of output?

## Week 5

### Problem Solving and Innovation

### Perspectives

Local Optima: an action in any direction will lead to a less good immediate outcome

Rugged landscape: many local peaks

Mt. Fuji landscape: only one global peak

### Heuristics

Do the Opposite: this is an example of a hueristic that might be attempted in order to innovate, eg: have the customer set the price rather than the typical way

Big Rocks First: put the big rocks in first when doing something

### Teams

Better at solving problems because people use different heuristics, and are diverse and hence able to overcome obstacles. Using a toaster as an example, iterative improvements of one product type can be considered as a type of team as well. 



### Recombination

How many ways can we combine things together. Many new things are really just mash-ups of old solutions to other problems, look at the post-it note as an example. If the glue is too sticky it won't work, if it's not sticky enough it won't work. You have to try different glues to get the right conditions. 

### Markov Processes

Many things can be thought of as Markov Processes, they must have:

1) finite number of states

2) ability to get from any state to any other

3) fixed transition probablity

Following is an example of a markov process, modeling a classroom of students who can be either alert or bored

#### Scenario 1: 100 Alert students

|        | A(t) | B(t) |
| ------ | ---- | ---- |
| A(t+1) | 0.8  | 0.25 |
| B(t+1) | 0.2  | 0.75 |

The matrix above gives the probability that there will be a state change during any period. In the case that all students begin alert, multiply the above matrix by the second column below:

| Alert | 1    |
| ----- | ---- |
| Bored | 0    |

Step through the example above for many periods to get the value for any particular time period

### Markov Model of Democratization

Let's say that 20% of dictatorships become democracies in each period, and 5% of democracies become dictatorships in each period. 

| 0.95 | 0.2  |
| ---- | ---- |
| 0.05 | 0.8  |

Expanding the model to free, partly free, and not free: 

| 0.9  | 0.1  | .05  |
| ---- | ---- | ---- |
| .05  | 0.8  | .15  |
| 0    | 0.1  | 0.8  |

multipled by:

| p     |
| ----- |
| q     |
| 1-p-q |

### Markov Convergence Theorem

4 necessary conditions for MCT to apply:

1) Finite states, 2) Fixed transition probablities 3) there is a path from one state to any other 4) not a simple cycle

This is a tricky theorem to apply to the real world, since in this model history doesn't matter and initial conditions don't matter. 