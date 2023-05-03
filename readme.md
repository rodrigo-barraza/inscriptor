## Inscriptor
Image captioning for data set annotation. An implementation of diffusers utilizing BLIP2's new **zero-shot instructed vision-to-language generation**.

### Recommended Requirements
24GB VRAM and 48GB RAM

### Install Torch 
#### with pip:
```
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```
#### with conda:
```
conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
```
or install from https://pytorch.org/get-started/locally/

### Examples
*Coming soon*

### How to use
Inside `inscriptor-mass-captioning.ipynb`, point `imagesDirectory` to your local dataset directory. The dataset directory should contain images ( in any of these formats `".jpg", ".png", ".jpeg", ".webp", ".gif"`) and can contain subfolders with their own images. Inscriptor will recursively search for images in the directories. The names of these folders can be used as tokens to add to the caption. For example, if you have a folder named `cat` and another named `dog`, the caption will contain the tokens `cat` and `dog`.