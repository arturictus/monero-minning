build for machine
https://getmonero.org/resources/user-guides/mine-to-pool.html

- install NVIDIA DRIVERS
http://christopher5106.github.io/nvidia/2016/12/30/commands-nvidia-install-ubuntu-16-04.html

- install CUDA
- compile

```
apt-get install libmicrohttpd-dev libssl-dev cmake build-essential
git clone https://github.com/fireice-uk/xmr-stak.git

mkdir build-$(gcc -dumpmachine)
cd $_
cmake ../
make -j$(nproc)
<!-- cp ../config.txt bin/ -->
cd bin
```
run the miner:

```
cd bin
nohup ./xmr-stak &
```

- check cards
```
nvidia-smi
```

- todo
fix MEMORY ALLOC FAILED: mmap failed (big pages)
