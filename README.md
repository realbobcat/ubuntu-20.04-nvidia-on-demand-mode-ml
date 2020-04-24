# ubuntu-20.04-nvidia-on-demand-mode-ml

TensorFlow-GPU/Keras under Ubuntu 20.04 NVIDIA On Demand Mode

## 运行时执行

... ~$ alias nvrun="\_\_NV_PRIME_RENDER_OFFLOAD=1 \_\_GLX_VENDOR_LIBRARY_NAME=nvidia"

... ~$ nvrun conda activate tf2

(tf2) ... ~$ jupyter notebook

<img src='./Screenshot from 2020-04-24 17-47-08.png' align='center' width=600 height=200 />

## 结束时释放显存

先关闭conda，然后运行

... ~$ nvidia-smi

查看显存占用进程

... ~$ kill -9 XXXX

<img src='./Screenshot from 2020-04-24 18-13-57.png' align='center' width=600 height=400 />
