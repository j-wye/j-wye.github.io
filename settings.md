# User PC Auto Setup with Ubuntu 22.04
### Environment
```
Ubuntu 22.04 humble
nvidia-driver-525
CUDA 11.8
cuDNN 8.7
```

### Auto Setup for all of CUDA, cuDNN v8.7.0 and Anaconda
```bash
wget https://raw.githubusercontent.com/j-wye/j-wye.github.io/main/autoset.sh
bash autoset.sh
source ~/.bashrc
```

### Only Ubuntu PC Auto Setup (include Chrome and Anaconda download)
```bash
wget https://raw.githubusercontent.com/j-wye/j-wye.github.io/main/basic_autoset.sh
bash basic_autoset.sh
source ~/.bashrc
```

### Check your cuDNN version and Installation
First, you have to check your [GPU and CUDA compatibility](https://www.wikiwand.com/en/CUDA#GPUs_supported)

And then

[Download cuDNN](https://developer.nvidia.com/rdp/cudnn-archive)

### Conda Environment Settings
[Check Anaconda Version which you want and copy](https://repo.anaconda.com/archive/) and follows:
```bash
axel https://repo.anaconda.com/archive/${copy version full name.sh}
bash ${copy version full name.sh}
source ~/.bashrc
```