# A2C applied to Blood Bowl

The code provided in the repository is an attempt of applying the reinforcement learning algorithm A2C to Blood Bowl. 

The code is structured in a way, that runs parallel environments of Blood Bowl using the code in ``vec_env.py``, where the trajectories collected is used for updating the models parameters after a fixed number of steps. A lot of the configurations for the code can be altered in arguments.py.

## Results

Currently, preliminary results have been acquired on the three smallest/easiest Gym environments in FFAI, which has a board of 4 × 3, 12 × 5, and 16 × 9 squares with 1, 3, and 5 fielded players on each team, respectively. A more comprehensive description of the experiments can be found in the paper: Blood Bowl: A New Board Game Challenge and Competition for AI (https://njustesen.files.wordpress.com/2019/07/justesen2019blood.pdf)

## Rewards
The results mentioned above, uses a different reward function and can be altered from ``vec_env.py``.

## Reproducibility 

**Before getting started:**
* We recommend to use Anaconda with python3.6 or newer.
* Install Pytorch installed (https://pytorch.org/ )
* Install matplotlib
* Install ffai

**The code:**

In order to switch between board sizes, change the variable board_size in ``arguments.py``

**Run**
Simply run the main.py script.
