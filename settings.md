# User PC Auto Setup with Ubuntu 22.04
### Environment
```
Ubuntu 22.04 humble
nvidia-driver-525
CUDA 11.8
cuDNN 8.7
```

### Only Ubuntu PC Auto Setup
```bash
wget https://raw.githubusercontent.com/j-wye/j-wye.github.io/main/basic_autoset.sh
bash basic_autoset.sh
source ~/.bashrc
```

### Auto Setup for CUDA, cuDNN v8.7.0 and Anaconda 
```bash
wget https://raw.githubusercontent.com/j-wye/j-wye.github.io/main/additional_autoset.sh
bash additional_autoset.sh
source ~/.bashrc
```
<!-- ### cuDNN v8.7.0 Installation -->
<!-- [Download cuDNN v8.7.0 for CUDA 11.X => Local Installer for Linux x86_64 (Tar)](https://developer.nvidia.com/rdp/cudnn-archive) -->

<!-- ### Conda Environment Settings -->
