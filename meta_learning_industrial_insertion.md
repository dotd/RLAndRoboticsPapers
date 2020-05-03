# Meta-Reinforcement Learning for Robotic Industrial Insertion Tasks

Gerrit Schoettler, Ashvin Nair, Juan Aparicio Ojea,
Sergey Levine, Eugen Solowjow

- [local link](pdfs/Meta-Reinforcement_Learning_for_Robotic_Industrial_Insertion_Tasks.pdf),
- [web link](https://arxiv.org/abs/2004.14404)
- [github.io link + movie](https://pearl-insertion.github.io/)



## Or Summery
- This paper uses a very interesting and efficient off-policy 
context based meta-RL algorithm called [PEARL](https://arxiv.org/abs/1903.08254), to train on a distribution of 
insertion tasks in simulation only, and then adapt them on a real robot in 
less than **20** attempts. 
- The task is performed from a low dimensional 
observation (end effector position) since the **socket is fixed**. 
- I think it is very nice to see meta-RL starting to be applied in real robotic 
tasks, and find these results encouraging
- I do wonder if this technique 
can scale up to pixel observations, as real images will be very different from 
anything a simulation produces.