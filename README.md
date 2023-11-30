# quantum-gflownets



TODO:
- [X] test without masking. Result: Failed to learn
- [ ] test with beta 1/T
- [ ] replace softmax with sharpened logits logits x 1\T (lower sharpens)
- [X] try scaling rewards by 2. Result: frowny faces had too high a reward and learned to only generate frowny faces.
- [X] try fixing logZ to correct value. Result: Learned to maximally generate smiley faces but failed to learn proper proportions. Learning mimicked optimized logZ. 
- [ ] update srun to sbatch for persistent job
- [X] try changing alternating init to 1 instead of -1. Result: poor convergence
- [X] reverse rewards. Still produces all smileys showing that reward is not being used.
- [X]  add more layers. Result: no significant change
- [X] investigate order of actions. Result: model not learning
- [X] heavier clip penalty for negative rewards
- [X] update over more epochs. Keep. Better convergence
- [X] try without amsgrad. Result: keep false
- [X] try reward combo of 2 and 4. Works great but still not getting distribution. just maximizing


What is running?
-  reverse reward

What is working?
- works for both smile and frown. 
- maximizes instead of proportional rewards