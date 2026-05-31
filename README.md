# POD-rDL

## Overview

This repository contains a demo of the POD-DL with residual (POD-rDL). POD-rDL is an extension of the POD-DL , a hybrid model that combines proper orthogonal decomposition (POD) with a neural network (Abadía-Heredia et al., 2022). POD-rDL uses recurrent and fully-connected layers, and it implements skip connections that facilitate deeper models, thus improving the performance predicting turbulent flows compared to the base algorithm.

<p align="center">
  <img width="637" height="418" alt="Image" src="https://github.com/user-attachments/assets/67c5c70d-5c56-459f-83a2-4166ebcdf246" />
</p>

Figure 1. **Sketch of the prediction models**: (a) POD-DL, (b) POD-rDL. The dimension of the output for each layer has been indicated in each block. The symbols *N* and *H* denote the dimensionality, and *T* and *t* the length of the sequence.

## Requirements

- Python
- NumPy
- h5py
- Matplotlib
- PyTorch
- path
- tqdm

## Example dataset

This demo showcases the prediction of POD coefficients pre-computed from the velocity field in a three-dimensional viscoelastic jet. The `data/` repository contains the file `POD_space.h5py`. Trained models are saved in the `model/` directory.

A pretrained model is included in the `model/` directory. The parameters of the models are already set in the `config` class

## Publication

Amor, C., Corrochano, A., Rosti, M. E., & Le Clainche, S. (2026). Reduced-order modeling of a viscoelastic turbulent jet with hybrid machine learning models. *J. Phys.: Conf. Ser.* **3230**, 012001. https://doi.org/10.1088/1742-6596/3230/1/012001.

