# popsynth_inference_pipeline
Pipeline code for the popsynth inference 

## Pipeline Steps:
1. Generate simulation data _d_ given _π_TRUNC(θ)_
2. Given some observed data _d_obs_ Train a surrogate for _LnL(d_obs | θ)_
3. Use an acquisition function based on _LnL_ uncertainty / Truncate _π_TRUNC(θ)_ based on regions low probability
4. Repeat till P(θ|d_obs) converged / _LnL_ uncertainty is below some threshold
