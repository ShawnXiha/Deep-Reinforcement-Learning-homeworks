[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Project 1: Navigation

### Introduction of the task

In project, I will train an agent to navigate (and collect bananas!) in a large, square world.  

![Trained Agent][image1]

#### rewards

- **`+1`** - a yellow banana collected
- **`-1`** - a blue banana collected

#### state space

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:

#### actions

- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

#### goal 

get an average score of +13 over 100 consecutive episodes.


### setup environment 

#### install pytorch

As I have a online Server with cuda10 toolkit, I build my pytorch environment by:

```bash
conda create --name drlnd python=3.6
source activate drlnd
conda install pytorch torchvision cuda100 -c pytorch

```
#### ml-agent

```bash
git clone https://github.com/Unity-Technologies/ml-agents.git
pip3 install -e .
```

#### download environment

I use [headless banana environment](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) as I am using online Server


### 