![](https://lh3.googleusercontent.com/2USBQm0ugfhaNqPYZp33OaHBlrnntJG8Ll-HkT7C5x_Uzg5L6v4GE1DB5idhPZ5HUaesp966jZukwODopH_jYFZ3ce-fR-j9HK0qubYyiiVOI9Yesn9FFPyGHn352kakQuoM9T1S)
# ePIC Boost Miner for GRIN COIN #

#### Please UNDERSTAND and AGREE to the terms in the [EULA](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/EULA.md) before using ePIC Boost Miner for Grin Coin ####
---
## Table of Contents

**[About ePIC Boost Miner](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#about-epic-boost-miner)**  
**[System Requirements](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#system-requirements)**  
**[Performance](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#performance)**  
**[Driver Selection](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#driver-selection)**  
 **[Driver Download and Installation](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#driver-download-and-installation)**  
 - [ROCm](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#instructions-for-installing-rocm-drivers)  
 - [AMDGPU-PRO](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#instructions-for-installing-the-amdgpu-pro-driver)

**[Installing ePIC Boost Miner](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#epic-boost-miner-installation)**  
**[Looking for Mining Pools](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#looking-for-mining-pools)**  
**[Support](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#looking-for-mining-pools)**

---

## About ePIC Boost Miner

ePIC Boost Miner is a GPU Miner specifically designed to give the best performance on Sapphire’s RX 570 16GB Graphics Card when mining Grin Coins.

***Please note that ePIC Boost technology will ONLY work when used with the Sapphire RX 570 16GB Graphics Cards.***

This miner will provide superior performance on Cuckatoo31, compared to cards costing twice as much. Taking advantage of the full 16GB of GPU memory, you can expect a dramatic increase in mining performance over conventional 8GB and 11GB graphics cards -- up to 2x increase on Cuckatoo31. In addition, ePIC Boost will also provide the fastest performance on Cuckaroo29 compared to other miners on AMD cards.

Additionally, ePIC miner's plug-in drivers for ROCm and OCL provide full fidelity or full accuracy when mining Grin. This is an important point to note as Cuckatoo31 requires 14GB of GPU memory to accurately solve a graph cycle. With Sapphire’s 16GB memory, mining performance is up to 40% faster than competing Nvidia GPU’s with only 11GB. These 11GB cards use a memory overflow optimization to solve Cuckatoo31 graphs, but that reduces actual mining performance by 30% in real-world situations. For example, an Nvidia 1080ti will solve at 0.52 gps but in actual mining conditions, pool results show 0.37 GPS or about 30% less.

THE LOWER FIDELITY ON 11GB AND 8GB CARDS WHEN MINING CUCKATOO31 RESULTS IN LESS MINING REWARDS.

**Note: ePIC deducts a 2.5% dev fee from your mining rewards. To help fund the Grin community and support future improvements, ePIC will donate 20% of the collected dev fee back to the community. See [General Funding](https://grin-tech.org/general_funding) for more details. If you do not agree with ePIC’s dev fee policy, you can use other software to mine Grin. Performance may vary significantly when using other mining software.**

If you wish to purchase and/or obtain more info on this GPU, please visit the [Sapphire RX 570 16GB GPU](https://gpuminer.sapphiretech.com/Radeon-RX-570-16GB-Blockchain/) site.

For further information on system requirements, performance, driver selection and installation please refer to the information below.

---

## **System Requirements**
|||
|--:|--|
|**CPU**|Celeron or faster Intel / AMD processor
| **Memory** |8GB system memory|
|**OS**|Ubuntu 18.04.1 installation|
|**Driver**|ROCm or AMDGPU-PRO driver stack *(**MUST USE ONLY ONE OF THE TWO**)*|
|**GPU**|  Sapphire RX570 16GB only|
| **PCIe** | *Gen 2.0 or Gen 3.0 |
|||

###### **The AMDGPU-PRO driver is supported on both PCIe Gen2 and Gen3, while ROCm is only supported on PCIe Gen 3.0 with atomics.*

---

## **Performance**

Your performance will vary depending on your CPU, PCIe slot and GPU driver used. Performance numbers were measured on ePIC test systems using the drivers referenced on this Github.

|||||
|---|:---:|:---:|:---:|
| | **Base** | **Better**  |**Best**|
| **CPU**           | Celeron / Pentium | i3/i5/i7/Ryzen Multithreading |i5/i7/i9/Ryzen Multithreading
| **Bus**    | PCIe 2.0      |  PCIe 3.0 |PCIe 3.0 with [Atomics](https://github.com/RadeonOpenCompute/ROCm_Documentation/blob/master/Installation_Guide/More-about-how-ROCm-uses-PCIe-Atomics.rst)|
| **Cuckaroo29+ Performance**| 1.5 gps      |    1.6 gps |1.9 gps|
| **Cuckatoo31+ Performance** | 0.35 gps      |    0.41 gps |0.45 gps|
|**Mining Fidelity**| 0.99      |    0.99 | 0.99|
| **Driver** | [AMD GPU Pro](https://www.amd.com/en/support/graphics/radeon-500-series/radeon-rx-500-series/radeon-rx-570)     |    [AMD GPU Pro](https://www.amd.com/en/support/graphics/radeon-500-series/radeon-rx-500-series/radeon-rx-570) | [AMD ROCm](https://github.com/RadeonOpenCompute/ROCm)|



***Disclaimers:*** 
 ###### - Performance may vary depending upon your system configuration. Your performance in mining conditions may differ substantially depending on your system, network difficulty, internet connection and other factors. Refer to EULA for additional information.

###### - Features amd performance are subject to change without notice.
  
######  -  WHEN USING CUCKATOO31 WITH 11GB AND 8GB CARDS AND OTHER MINING SOFTWARE, THE LOWER FIDELITY RESULTS IN LESS MINING REWARDS.

---

## Driver Selection

Use the following chart to determine the best driver for your system confirmation. If you are unsure, use the AMD GPU Pro Driver. Best performance can be had if your system supports PCIe Gen3 and Atomics, however that is system dependent.


![](https://lh5.googleusercontent.com/qD_lKkPqnjHKtiL96RQ_fELGKzz6IEV90ooGg07nHqLY5K3ZR9H9LhTMBwwkNZpuarQFvgbeZ_kmTCMU3-Vxv53dna4q5giZSxXj6QY3vdA1JuquC8hwbaQ0xJGdsuwTO4hBKN99)


------------------------------------

## Driver Download and Installation

---

### Instructions for Installing ROCm Drivers ###  

###### :high_brightness:*For AMDGPU-PRO users, [Skip](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#instructions-for-installing-the-amdgpu-pro-driver) to the next section. For additional information on the ROCm Driver please visit the [official page](https://github.com/RadeonOpenCompute/ROCm#ubuntu-support---installing-from-a-debian-repository).*


#### 1. Download the [ROCm Driver](https://github.com/RadeonOpenCompute/ROCm). 

#### 2. Make sure your system is up to date

```sh

sudo apt update

sudo apt dist-upgrade

sudo apt install libnuma-dev

sudo reboot

```

#### 3. Add the ROCm apt repository

```sh

wget -qO - http://repo.radeon.com/rocm/apt/debian/rocm.gpg.key | sudo apt-key add -

echo 'deb [arch=amd64] http://repo.radeon.com/rocm/apt/debian/ xenial main' | sudo tee /etc/apt/sources.list.d/rocm.list

```

#### 4. Install

```sh

sudo apt update

sudo apt install rocm-dkms

```

  

#### 5. Set Your Permissions

```sh

sudo usermod -a -G video $LOGNAME

```

  

#### 6. Finish Install

```sh

sudo reboot

```

  

#### 7. Check Install

```sh

/opt/rocm/bin/rocminfo

/opt/rocm/opencl/bin/x86_64/clinfo

```
#### 8. [Install the ePIC Boost Miner for Grin Coin](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#installing-epic-boost-miner)
  
---

### Instructions for installing the AMDGPU-PRO Driver

###### For additional information on the AMDGPU-PRO Driver please visit the [official page](https://amdgpu-install.readthedocs.io/en/latest/index.html).

  

#### 1. [Download AMDGPU-PRO  Ubuntu driver](https://www.amd.com/en/support/graphics/radeon-500-series/radeon-rx-500-series/radeon-rx-570)



or pull it using curl:

```sh

cd ~/Downloads

curl -L -O --referer https://support.amd.com https://drivers.amd.com/drivers/linux/amdgpu-pro-18.50-725072-ubuntu-18.04.tar.xz

```

  

#### 2. Extracting the Archive

```sh

cd ~/Downloads

tar -Jxvf amdgpu-pro-18.50-725072-ubuntu-18.04.tar.xz

```

  

#### 3. Install

```sh

cd ~/Downloads/amdgpu-pro-18.50-725072-ubuntu-18.04

./amdgpu-pro-install --opencl=legacy

```
#### 4. [Install ePIC Boost Miner for Grin Coin](https://github.com/EPICBOOST/ePIC-Boost-Miner/blob/master/README.md#installing-epic-boost-miner)
  
  ---

## ePIC-Boost-Miner Installation

#### Download and Configuration

  

#### 1. Download

Download miner from the Release tab.

  

#### 2. Extract Archive

```sh

cd <Download directory>

tar xzvf ePIC-Boost-Miner-v1.0.tar.gz

```

#### 3. Edit Configuration File

```sh

cd <ePIC-Boost-Miner directory>

```

Using your favourite editor open ``epic-boost-miner.toml``

  

##### 3(a). Edit Pool

Edit based on your pool information the following fields:

- stratum_server_addr

- stratum_server_login

- stratum_server_password

- stratum_server_tls_enabled

  

If you are looking for a pool to use some suggestions can be found below [Looking for Mining Pools](#Looking-for-Mining-Pools).

  

##### 3(b). Edit Plugin

There are four plugins to choose from:

- cuckatoo_mean_opencl_amdgpu_31

- cuckatoo_mean_opencl_rocm_31

- cuckaroo_mean_opencl_amdgpu_31

- cuckaroo_mean_opencl_rocm_31

  

For each device select which plugin to run (make sure to use the appropriate plugin for your driver)

```sh

[[mining.miner_plugin_config]]

plugin_name = "<plugin name coresponding to one of the choices from the list above>"

[mining.miner_plugin_config.parameters]

device = <device id (if there is only one card in the system it should be 0)>

```

#### 4. Start Miner

```sh

cd <ePIC-Boost-Miner directory>

./ePIC-Boost-Miner

```

  

## Looking for Mining Pools

###### GrinMint : [https://grinmint.com/pages/index.html](https://grinmint.com/pages/index.html)

###### MWGrinPool: [https://www.mwgrinpool.com/](https://www.mwgrinpool.com/)

###### SparkPool: [https://eth.sparkpool.com/](https://eth.sparkpool.com/)

###### F2Pool: [https://www.f2pool.com/](https://www.f2pool.com/)

---

## Stay Tuned!
ePIC is continually working to update and optimize this miner - to push performance and maximize the potential and ROI of your Sapphire RX 570 16GB Graphics Card. 

Please post bugs to this GitHub or email at support@epicblockchain.io and check back here for future enhancements.

### Happy Mining and KEEP GRINNING!

---

###### *OpenCL plugin and OpenCL code copyright (c) 2018 ePIC Blockchain Technologies Inc.*

###### *Miner application contains Open Source Code. Attributions to:*

###### *Equihash Solver provided under MIT License and Copyright (c) 2016 https://github.com/tromp/equihash*

###### *Grin-Miner provided under Apache 2.0 Licence and Copyright (c) 2019 https://github.com/mimblewimble/grin-miner*

