# Basic Errors
##‘GLIBCXX_3.4.30’ not found
conda environment에서 rclpy를 import할 때 발생함
```bash
conda install -c conda-forge gcc=12.1.0

rm /home/$USER/anaconda3/bin/../lib/libstdc++.so.6
cp /usr/lib/x86_64-linux-gnu/libstdc++.so.6.0.30 /home/$USER/anaconda3/bin/../lib 
ln -s /home/$USER/anaconda3/bin/../lib/libstdc++.so.6.0.30 /home/$USER/anaconda3/bin/../lib/libstdc++.so.6
```
