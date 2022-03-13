# Nonlinear-controller-backstepping-design
3rd order strict feedback nonlinear system, controller desined using backstepping method
In MATLAB, a mathematical model is composed by main.m, backstepping.m, systemdynamics.m. The main idea is that: 
1）	Set 20 initial value of state variables (x_1,x_2,x_3)as random number from -1 to 1
2）	In each integration step, calculate u by state variables according backstepping design result as manipulated input for
 next step. 
3）	With each manual determined parameters set (k_1,k_2,k_3), there are 20 random initial samples, each calculated with 
6000 steps, derivative step is set to be 1e-3.
 4）               Plot.m the state variables, state variables’ derivative and manipulated input in a figure of 9 sub plots. With subplot
 (3,3,1) ({t,x}_1); subplot (3,3,2) ({t,x}_2); subplot (3,3,3) ({t,x}_3); subplot (3,3,4) (t,\dot{x_1}); subplot (3,3,5) (t,\dot{x_2}); 
subplot (3,3,6) (t,\dot{x_3}) subplot (3,3,1) (x_1,x_2,x_3) ; subplot (3,3,2) (\dot{x_1},\dot{x_2},\dot{x_3}); subplot (3,3,3) (t,u).
