# VSA-Mamba

**Exploring Extensive Representation Learning in Remote Sensing Change Detection by Vision Super-Alignment and Beyond**

## Framework



## Experiment result



## Inastall

**Please refer to the code repository [ChangeMamba](https://github.com/ChenHongruixuan/ChangeMamba) and install according to the requirements.**

## Pre-trained model

1. Download Pre-trained model ( [SYSU-CD](https://drive.google.com/file/d/1bxf_6j2qiYr935XzZ6Geyj0h6WDCGXmJ/view?usp=sharing) , [WHU-CD](https://drive.google.com/file/d/1xF9JytqDlsz4vmHMA-1Wb9wpf0CNUBnD/view?usp=sharing)，[LEVIER+-CD](https://drive.google.com/file/d/1azqF9H4EKvaGgx31aUo2KApZWZRStaZ8/view?usp=sharing) , [LEVIER-CD](https://drive.google.com/file/d/1en5R-KCjipbwP44CAYJLSWFLB_88YeSU/view?usp=sharing) and place in `./checkpoint/`

2. Download  [Pretrained weight](https://github.com/ChenHongruixuan/ChangeMamba?tab=readme-ov-file#a-pretrained-weight-of-vmamba-encoder)  and place in `./Pretrained_Weight/`

## Data Preparation

1. 

## Train 

```shell
python train.py 
```

```shell
python train.py 
```


## Inference

```bash
python infers.py  --dataset 'WHU-CD'  --model_type MambaBCD_Tiny     --test_dataset_path './test_dataset_path/'  --test_data_list_path    './test_dataset_path/WHUCD/test.txt'  --cfg './configs/vssm1/vssm_tiny_224_0229flex.yaml'    --pretrained_weight_path   ./Pretrained_Weight/vssm_tiny_0230_ckpt_epoch_262.pth    --resume ./checkpoint/WHU-CD_model.pth    --result_saved_path './result/WHU-CD/'
```

## Acknowledgement

This project is build based on [ChangeMamba](https://github.com/ChenHongruixuan/ChangeMamba) and [SIRST-5K](https://github.com/XPixelGroup/DiffBIR). We thank the authors for sharing their code.
