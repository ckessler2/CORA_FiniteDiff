# CORA_FiniteDiff

[CORA](https://github.com/TUMcps/CORA) is a general-purpose reachability toolkit written in MATLAB, capable of verifying continuous nonlinear dynamic systems through reachability analysis.

To verify a given model, CORA derives and solves Jacobian and Hessian matrices, but my model of interest ([Li 2022](https://doi.org/10.1017/jfm.2022.89)) is too complex for analytical derivations. My solution is to estimate partial derivatives using finite difference approximations, for which I have written two scripts.
