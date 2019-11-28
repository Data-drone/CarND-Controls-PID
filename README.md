# Udacity Self Driving Car Nanodegree

# PID Project

This is a write up of the PID Project

# Goals

- Describe Effect of P, I, D
- Describe settings
- Choice of Hyperparams

# Reflection

The PID controller was implemented as per the Python Prototype from the lessons.

### P
I focused first on a pure P controller and as per the lectures, it tends to oscillate wildly when trying to correct for error.

### D
Adding a D value stabilised the oscillations as per the lectures and for this particular course at least produces a stable enough solution to drive most of the course. 

### I
On this particular course and for the steering variable, it seems that whilst I can help a little bit generally P and D alone can keep the car on the course. The addition of I unless it has a really small coefficient can be bad in that it brings oscillation back though tuning together with D can help a bit around sharp corners


# Hyperparmeter tuning

In this case I decided to test manual hyperparameter tuning first. I was able to find a good setting for the car without using twiddle or other algorithms. Student discussion highlighted certain starting points for Kp / Ki and Kd which I followed.