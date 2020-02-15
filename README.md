# CURRENTLY NEEDS TESTING!!!

### Install Anaconda3
Download the installer [https://www.anaconda.com/distribution/#linux](https://www.anaconda.com/distribution/#linux). 

Initialize conda for your shell.
```bash
export PATH=~/anaconda3/bin:$PATH
conda init bash
# Restart your shell
```

### Install DeepFaceLab

```bash
conda create -y -n deepfacelab python=3.6.8 cudatoolkit=9.2 cudnn=7.6.4
conda activate deepfacelab
git clone https://github.com/lbfs/DeepFaceLab_Linux.git
cd DeepFaceLab_Linux
python -m pip install -r requirements-cuda.txt
```

## Download CelebA Dataset
Download the latest NVIDIA build from the main repository for Windows. [https://drive.google.com/drive/folders/17a9b9zmLdnAlItifcGSE9ixDIDAT3YxP](https://drive.google.com/drive/folders/17a9b9zmLdnAlItifcGSE9ixDIDAT3YxP)

Extract the build and go into the _internal folder.
Copy both pretrain_CelebA and pretrain_Quick96 to the directory DeepFaceLab_Linux/

