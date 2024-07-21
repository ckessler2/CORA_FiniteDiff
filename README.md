# CORA_FiniteDiff

[CORA](https://github.com/TUMcps/CORA) is a general-purpose reachability toolkit written in MATLAB, capable of verifying continuous nonlinear dynamic systems through reachability analysis.

To verify a given model, CORA derives and solves Jacobian and Hessian matrices, but my model of interest ([Li 2022](https://doi.org/10.1017/jfm.2022.89)) is too complex for analytical derivations. My solution is to estimate partial derivatives using finite difference approximations (FDAs), for which I have written two scripts.

If reliable, this could enable CORA to be used with any dynamic model no matter how complex - the examples and benchmark systems are all relatively simple models. As evidence of my method working as intended, I have implemented it in two existing CORA examples - [Tank](https://github.com/TUMcps/CORA/blob/master/examples/contDynamics/nonlinearSys/example_nonlinear_reach_01_tank.m) and [Quad](https://github.com/TUMcps/CORA/blob/master/examples/contDynamics/neurNetContrSys/benchmark_neuralNet_reach_09_QUAD.m).

### Limitations

* Only implemented for 1st and 2nd order derivatives (Jacobian and Hessian)
* Derivative approximation accuracy depends on the size of perturbation (delta), defined in the FDA scripts

### How to use 

* Only implemented for 1st and 2nd order derivatives (Jacobian and Hessian)
* Derivative approximation accuracy depends on the size of perturbation (delta), defined in the FDA scripts

<hr style="height: 1px;">

### Tank Result

<img src="https://github.com/ckessler2/CORA_FiniteDiff/blob/main/CORA_FiniteDiff_Tank.jpg">

### Quad Result

asd
