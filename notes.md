build for machine
https://getmonero.org/resources/user-guides/mine-to-pool.html

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
