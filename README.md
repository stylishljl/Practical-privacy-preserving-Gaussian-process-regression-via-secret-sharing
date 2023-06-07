# Practical Privacy-Preserving Gaussian Process Regression via Secret Sharing

This code is used to reproduce the experiments involved in the PP-GP paper. The execution of the code needs to rely on the privacy-preserving machine learning open source framework [Crypten](https://github.com/facebookresearch/crypten). 

## Environment configuration:
To reproduce the experiments in the paper, you need to configure the environment as instructed below.(We recommend using anaconda to create a virtual environment.)
1. Execute `conda create -n your_env_name python=3.7` to create a conda virtual environment;
2. Execute `pip install crypten` to install ''Crypten''.


## implement:
You can follow the instructions in the corresponding file to run the code to reproduce the relevant experimental results.

## Precautions: 
1. When doing multi-machine testing, you need to configure the same environment on two servers according to the above instructions;
2. Crypten may not support recent versions of torch, we recommend installing torchv1.10.2.

## Note:
1. Before conducting the experiment, the parameter "precision_bits:" in line 7 of the "default.yaml" file in Crypten needs to be set to 26.
2. Since the traffic dataset is private to individuals, it is not convenient to open it at present, so we cannot provide the reproduction code of all the experimental results in Table 1. We currently provide code to reproduce experimental results on the diabetes dataset. The traffic data set and related reproduction code will be considered for disclosure after the data disclosure conditions are met in the future.
