<h2 align="center">
Foraminiferal spatiotemporal missing data completion via temporal knowledge graph embedding
</h2>

<!-- <p align="center">
  <img src="https://img.shields.io/badge/ACL-2023-brightgreen">
  <a href = 'https://aclanthology.org/2023.acl-long.862.pdf' target='_blank'><img src="http://img.shields.io/badge/Paper-PDF-red.svg"></a>
  <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg">
  <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?e&logo=PyTorch&logoColor=white">
</p> -->


<p align="center">
Codes for the paper Foraminiferal spatiotemporal missing data completion via temporal knowledge graph embedding.
</p>


## 


### Installation
Create a conda environment with pytorch and scikit-learn :
```
conda create --name fstkgc_env python=3.8
source activate fstkgc_env
conda install --file requirements.txt -c pytorch
```


### Datasets

```
python process_paleo.py
```

This will create the files required to compute the filtered metrics.

### Reproducing results of FSTKGC

In order to reproduce the results of FSTKGC on the four datasets in the paper,  run the following commands

```
python  learner.py --dataset 100_envAcom    --emb_reg 0.01 --time_reg 0.0001
```

### Acknowledgement
We refer to the code of [TeAST](https://github.com/dellixx/TeAST). Thanks for their great contributions!
