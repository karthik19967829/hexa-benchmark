# HEXA Benchmark

Codebase for the self-supervised goal reaching benchmark introduced in the [LEXA paper](https://github.com/orybkin/lexa) (Discovering and Achieving Goals via World Models, NeurIPS 2021).

<img src="https://github.com/karthik19967829/hexa-benchmark/blob/main/Figure5-1.png" width="1000">


## Setup

Create the conda environment by running : `conda env create -f environment.yml`

Alternatively, you can update an existing conda environment by running : `conda env update -f environment.yml`


Modify the python path   
`export PYTHONPATH=<path to hexa-benchmark>`  

Export the following variables for rendering  
`export MUJOCO_RENDERER=egl; export MUJOCO_GL=egl`

Please follow these [instructions][mujoco_instr] to install mujoco

[mujoco_instr]: https://github.com/openai/mujoco-py#install-mujoco

## Usage 

**WARNING!** The success criteria defined in this benchmark should not be used as a reward for the agent. The criteria were tuned to roughly match human intuition, but produce some false positives, which the agent can exploit if it observes the success variable. 


## Acknowledgements
Our code has been adapted and built on top LEXA Benchmark https://github.com/orybkin/lexa-benchmark
This benchmark is built on top of the following environments: [Adept](https://github.com/google-research/relay-policy-learning), [MetaWorld](https://github.com/rlworkgroup/metaworld), and [DeepMind Control Suite](https://github.com/deepmind/dm_control/tree/master/dm_control/suite).
