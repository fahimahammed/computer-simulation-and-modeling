# CSE4132: Computer Simulation and Modeling Lab
Welcome to the Modeling and Simulation Challenges repository, a comprehensive collection of solutions to intriguing problems in the realms of computer simulation and modeling. Geared towards students and enthusiasts in computer science and engineering, this repository offers diverse implementations and insights into various simulation scenarios.

## Included Problems:
### 1. Pure Pursuit Problem:
   
A fighter aircraft sights an enemy bomber aircraft and flies directly toward it, in order to catch up with the bomber and destroy it. The bomber (the target) continues flying (along a specified curve) so the fighter (the pursuer) has to change its direction to keep pointed toward the target. We are interested in determining the attack course of the fighter and in knowing how long it would take for it to catch up with the bomber. Solve this problem under the following conditions. You need to plot the whole path of fighter as well as bomber:

Logic behind the pure pursuit problem of simulation:

    - Bomber Aircraft and a Fighter Aircraft are flying in the same horizontal plane.
    - Fighter aircraft and bomber aircraft both are moving inside the rectangular range. 
    - The fighters and bombers have a velocity given, suppose s = 20 (input from screen).
    - The bomber and the fighter path co-ordinate (i.e., its position as a function of time) are randomizing from 1 to 1000. 
    - When the distance of the bomber and the fighter is less than 900km and greater than 100km, it is assumed that the bomber is shot down or destroyed. Otherwise, the bomber escaped from sight.

#### Sample Output: 
```bash
BOMBER ESCAPES FROM THE SIGHT OF FIGHTER
time=0 xf=642.00 yf=902.00 xb=788.00 yb=709.00 distance=242.00
time=1 xf=654.07 yf=886.05 xb=585.00 yb=997.00 distance=130.69
time=2 xf=643.50 yf=903.03 xb=587.00 yb= 6.00 distance=898.81
time=3 xf=642.24 yf=883.07 xb=11.00 yb=162.00 distance=958.33
The bomber plane escaped from sight at 3 second
```

### 2. Simulation of critical path method:

A furniture making company builds tables that consist of a drawer, four legs, and the top of the table. Building legs takes 11 hours, building the top takes 3 hours, and building the drawer takes 10 hours. After each part is built, each part is painted. The legs take 2 hours, top 1 hour, and the drawer 3 hours. The drawer is then attached to the tabletop (1 hour). After the top and drawer are attached, the four legs can be attached (1 hour). Draw the network diagram from Table 1. Also write program to find the critical Path.

| Activity               | Start Node | End Node | Time |
| ---------------------- | ---------- | -------- | ---- |
| A-Build Legs           | 1          | 2        | 11   |
| B-Build Top            | 1          | 3        | 3    |
| C-Build Drawer         | 1          | 4        | 10   |
| D-Paint Drawer         | 4          | 5        | 3    |
| E-Paint Top            | 3          | 5        | 1    |
| F-Paint Legs           | 2          | 6        | 2    |
| G-Attach Drawer to Top | 5          | 6        | 1    |
| H-Attach Legs          | 6          | 7        | 1    |

- **Input:** From file 
- **Output:** On screen & file

### 3. Simulation of linear congruential generator method: 

Write a program for linear congruential generator method to generate a sequence of random integers between zero and M-1. For example, the following table shows the sequences that result for various choices of a (multiplicative constant), b (additive constant), c (seed), and M (modulus).

| a   | b   | c   | M   | x0  | x1  | x2  | x3  | x4  | x5  | x6  | x7  | x8  | x9  | x10 | x11 | x12 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1   | 3   | 0   | 10  | 0   | 3   | 6   | 9   | 2   | 5   | 8   | 1   | 4   | 7   | 0   | 3   | 6   |
| 2   | 1   | 0   | 10  | 0   | 1   | 3   | 7   | 5   | 1   | 3   | 7   | 5   | 1   | 3   | 7   | 5   |
| 22  | 1   | 0   | 72  | 0   | 1   | 23  | 3   | 67  | 35  | 51  | 43  | 11  | 27  | 19  | 59  | 3   |
| 11  | 37  | 1   | 100 | 1   | 48  | 65  | 52  | 9   | 36  | 33  | 0   | 37  | 44  | 21  | 68  | 85  |
| 8   | 20  | 10  | 100 | 10  | 0   | 20  | 80  | 60  | 0   | 20  | 80  | 60  | 0   | 20  | 80  | 60  |

### 4. Simulation of a Chemical Reactor:

There are two substances A and B. They produce third substance C. The rate of formation of C is proportional to presence of A and B. Write a program to simulate how much of C has been produced as a function of time, ∆t = 0.1. Assume that a = 100g, b = 50g and c = 0g are quantities of A, B and C at time t = 0. Rate constants are also given as follows k1 = 0.008 and k2 = 0.002.

### 5. Simulation of a cubic Bezier curve:

There are four control points P0, P1, P2, and P3 position in 2D space. You have to write a program to construct the spline using Cubic Bezier curve construction approach. Also need to display the output for each new point.

### 6. Forecasting by ARIMA model

- **Identify ARIMA Order (p, d, q):** Plot the Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) to 
- **Model Estimation:** Fit the ARIMA model to the training data using the identified order (p, d, q).
- **Model Evaluation:** Evaluate the model's performance on the testing set. Use MSE, RMSE.
- **Forecasting:** Generate forecasts for future time points using the trained ARIMA model. Visualize the forecasts along with confidence intervals. 


<!-- Contributor: Fahim Ahammed Firoz -->