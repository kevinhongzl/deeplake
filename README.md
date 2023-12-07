# Partial-DANN

[![python](https://img.shields.io/badge/Python-3.8.17-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org) [![monai-shieldio](https://img.shields.io/badge/MONAI-1.0.1-5ec2b3.svg?logo=data:image/png;base64,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)](https://github.com/project-monai/monai) [![pytorch](https://img.shields.io/badge/PyTorch-1.12.1-EE4C2C.svg?style=flat&logo=pytorch)](https://pytorch.org) [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-000000.svg)](https://github.com/psf/black)


## Basic usage
```powershell
python main.py 
--root 'C:\Users\User\Desktop\TSM_Project\data\amos22' 
--output checkpoints 
--modality ct 
--batch_size 1 
--lr 0.0001 
--optim AdamW 
--max_iter 10000  
--eval_step 500 
--cache_rate 0.5 
--num_workers 2 
```

#### Fully-labeled dataset
* **Segmentation**
```
python main.py --module segmentation --modality MODALITY --loss dice2
``` 

* **Segmentation with domain adaptation**
```
python main.py --module dann --modality ct+mr --loss dice2
```

#### Partially-labelled dataset
* **Segmentation**
```
python main.py --module segmentation --modality MODALITY --masked --loss LOSS*
``` 
*Loss cannot be `tal` if the modality is `ct+mr`

* **Segmentation with domain adaptation**

One can choose to mask the loaded image (1) before training
```
python main.py --module dann --modality ct+mr --masked --loss LOSS
```
or (2) when calculating loss and during validation
```
python main.py --module dann --modality ct+mr --loss tal
```