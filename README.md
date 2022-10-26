# MIMO sims

## General
This repo contains a collection of all the massive MIMO simulations created by the Dramco research group. Simulations are written in python.

## Notation / System Model
We consider a MU-MIMO system with $M$ antenna elements serving $K$ single-antenna users. The complex transmit symbol intended for user $k$ is denoted as $s_k$. We assume linear precoding, the symbol for user $k$ at antenna $m$ is precoded using the precoding coefficient $w_{m,k}$. The precoded symbol at antenna $m$ is thus denoted as 
$$x_m = \sum_{k=1}^K w_{m,k}s_k.$$
More compactly, this can be written as
$$\boldsymbol{\mathrm{x}} = \boldsymbol{\mathrm{W}} \boldsymbol{\mathrm{s}}.$$
With $\boldsymbol{\mathrm{x}} \in \mathbb{C}^{M\times1}$ being the precoded symbols, $\boldsymbol{\mathrm{W}} \in \mathbb{C}^{M\times K}$ the precoding matrix and $\boldsymbol{\mathrm{s}} \in \mathbb{C}^{K\times 1}$ the symbol matrix.
After precoding the symbols are amplified (which can be a linear amplification in the simplest case)
$$\boldsymbol{\mathrm{y}} = \phi(\boldsymbol{\mathrm{x}}),$$
where $\phi(\cdot)$ denotes the elementwise nonlinear transformation caused by the power amplifier.
The received signal can then be obtained as
$$\boldsymbol{\mathrm{r}} = \boldsymbol{\mathrm{H}}^{T} \boldsymbol{\mathrm{y}} + \boldsymbol{\mathrm{v}}.$$
With $\boldsymbol{\mathrm{r}}\in \mathbb{C}^{K\times1}$ being the received signal vector, $\boldsymbol{\mathrm{H}} \in \mathbb{C}^{M\times K}$ the channel matrix and $\boldsymbol{\mathrm{v}}\in \mathbb{C}^{K\times1}$ being a vector with addative complex Gaussian noise.

## Repo structure

## To Do
- [x] Define system model
- [ ] Define repo structure
- [ ] Implement some precoders
- [ ] Implement some channel models
- [ ] Implement some equalizers
- [ ] Implement PA models

