# Robot Learning of Shifting Objects for Grasping in Cluttered Environments

- [https://arxiv.org/pdf/1907.11035.pdf](https://arxiv.org/pdf/1907.11035.pdf)

- [https://github.com/pantor/learning-shifting-for-grasping](https://github.com/pantor/learning-shifting-for-grasping)

## Differences in Setup
1. Gripper with force sensor
1. Ensenso depth camera

## Research Contribution
1. Presenting an algorithm for learning the optimal pose of manipulation primitives 
like:
    - clamping 
    - shifting 
1. Learning non-prehensible actions that explicitly
increase the grasping probability. 
    - Making one skill (shifting) directly dependent on another (grasping) 
    removes the need of sparse rewards, leading to more data-efficient learning. 
1. Applying to the industrial task of bin picking, (ability to empty bins completely)


## pre-grasping Manipulations 
- Sliding 
- Pushing 
- Rolling

## Work Structure 
1. Vision-based algorithm for learning a rewarding pose for applying object 
manipulation primitives (5 in total: 3 for grasping at different gripper widths, 
3 for shifting). 
1. Learning grasping by estimating the grasp probability at a given pose. 
1. Deriving:
    1. Grasping-dependent reward function
    1. Training procedure for shifting
    - This way, sparse rewards of the grasp success can be bypassed for more 
    data-efficient learning of shifting. 
1. Presenting a robotic system (Fig. 1) which learns the industrial task of 
bin picking. 
    - The system is able to empty bins completely 
    - achieves arbitrary grasp rates at the expense of picks per hour (PPH)
1. Evaluating the system’s ability of grasping novel objects from 
non-graspable positions

## Training
Data collection:
- Grasping: 25,000 Grasps in 100 hours, i.e., grasp every 14.4 seconds.
- Shifting: 2500 attempts in 9 hours, i.e., shift every 12.96 seconds. 

Advantage: separating leads to data efficient recording.

Exploration techniques:
- Maximizing self-information $$ p(a) \approx $$
- Minimizing uncertainty of prediction  
- Minimizing uncertainty of outcome