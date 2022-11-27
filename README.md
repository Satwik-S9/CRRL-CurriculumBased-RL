# Curriculum based Reinforcement Learning

> @Authors: Satwik Srivastava, Ashish Jacob Sam
> @Last Modified: 27.11.2022

**NOTE:** <br/>
This repo follows the cleanRL approach of one file doing everything so `curriculum.py` file has all the code that needs to be run. This work is not split into modules. However dependencies need to be installed to run the script.


## How to run the code.
- Download and build dependecies for [cleanrl]().
- Then run 

```bash
# FOR ORDERED CRL WITH USER DEFINED RATIO OF EASY:MEDIUM:HARD CURRICULA
python curriculum.py --track --crl --exp-name EXP_NAME --wandb-project-name PNAME \
--total-timesteps 50000
```
- for random CRRL

```bash
# FOR RANDOM CRL WHERE THE CURRICULUM IS GENERATED RANDOMLY IN ANY ORDER 
python curriculum.py --crl --random-crl --total-timesteps 50000 --track --wandb-project-name PNAME \
--exp-name EXP_NAME
```


