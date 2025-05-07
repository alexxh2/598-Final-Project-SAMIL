# SAMIL
Code for the paper Detecting Heart Disease from Multi-View Ultrasound Images via Supervised Attention Multiple Instance Learning (MLHC'23)

# Setup
### Prepare datasets
The AS diagnosis task in this study uses the view_and_diagnosis_labeled_set from TMED2 
- Step1. Download TMED2, please visit https://TMED.cs.tufts.edu and follow the instruction.
- Step2. Put the labeled and unlabeled image for the same study under same folder

### Install Anaconda
Follow the instructions here: https://conda.io/projects/conda/en/latest/user-guide/install/index.html

### Environment
pytorch 1.11.0

# Running experiments
### Define the environment variable
```export ROOT_DIR="paths to this repo" ```
(e.g.,  '/ab/cd/SAMIL')

```export DATA_INFO_DIR="path to the data_info/ folder" ```
(e.g.,  '/ab/cd/SAMIL/data_info')

```export DATA_DIR="path to the actual data ```
(e.g.,  '/ab/cd/SAMIL/Echo_data/view_and_diagnosis_labeled_set/')

```export CHECKPOINT_DIR="path to where pretrained view classifier and MOCO pretrained weights```
(e.g.,  '/ab/cd/SAMIL/model_checkpoints/')

### Running
Running SAMIL with study-level pretraining, go to [runs/SAMIL](runs/SAMIL)
``` bash launch_experiment.sh run_here ```

