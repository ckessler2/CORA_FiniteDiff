# CORA_FiniteDiff

[CORA](https://github.com/TUMcps/CORA) is a general-purpose reachability toolkit written in MATLAB, capable of verifying continuous nonlinear dynamic systems.

CORA includes deriving and solving Jacobian and Hessian matrices to verify a given model, but my model of interest is too complex for analytical derivations. My solution is to estimate partial derivatives using finite difference approximations, for which I have written two scripts.
