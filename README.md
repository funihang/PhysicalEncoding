# PhysicalEncoding

Physical Encoding Improves OOD Performance in Deep Learning Materials Property Prediction

Nihang Fu, Sadman Sadeed Omee, Jianjun Hu* <br>
Machine Learning and Evolution Laboratory <br>
Department of Computer Science and Engineering <br>
University of South Carolina

## Table of Contents
- [Requirements](#Requirements)

- [Datasets](#Datasets)

- [Pretrained Models](#Pretrained-models)

- [Performance](#Performance)

- [Acknowledgement](#Acknowledgement)

## Requirements

0. Set up virtual environment
```
conda create -n bertos
conda activate bertos
```

1. PyTorch and transformers for computers with Nvidia GPU.
```
conda install pytorch==1.8.0 torchvision==0.9.0 torchaudio==0.8.0 cudatoolkit=11.1 -c pytorch -c conda-forge
conda install -c conda-forge transformers
```
If you only has CPU on your computer, try this:
```
pip install transformers[torch]
```
If you are using Mac M1 chip computer, following [this tutorial](https://jamescalam.medium.com/hugging-face-and-sentence-transformers-on-m1-macs-4b12e40c21ce) or [this one](https://towardsdatascience.com/hugging-face-transformers-on-apple-m1-26f0705874d7) to install pytorch and transformers.

2. Other packagess
```
pip install -r requirements.txt
```  

## Datasets  
Our training process is carried out on our BERTOS datasets. After extracting the data under `datasets` folder, you will get the following four folders `ICSD`, `ICSD_CN`, `ICSD_CN_oxide`, and `ICSD_oxide`.


## Pretrained Models
Our trained models can be downloaded from figshare [BERTOS models](https://figshare.com/articles/online_resource/BERTOS_model/21554823), and you can use it as a test or prediction model.


## Performance

![Performance](performances.png)
Removing `OS`, the datasets under `datasets` folder correspond to the datasets in the figure.

## Acknowledgement
We use the Roost and ALIGNN networks.
```
@article{wolf2019huggingface,  
  title={Huggingface's transformers: State-of-the-art natural language processing},  
  author={Wolf, Thomas and Debut, Lysandre and Sanh, Victor and Chaumond, Julien and Delangue, Clement and Moi, Anthony and Cistac, Pierric and Rault, Tim and Louf, R{\'e}mi and Funtowicz, Morgan and others},  
  journal={arXiv preprint arXiv:1910.03771},  
  year={2019}  
}
```

## Cite our work
```


```

# Contact
If you have any problem, feel free to contact us via [nihang@email.sc.edu](mailto:nihang@email.sc.edu).
