---
layout:     post
title:      Hackintosh EFI For ASUS B250M-PLUS i5-7500 RX580
subtitle:   Hackintosh EFI
date:       2020-05-22
author:     ZSY
header-img: img/home-bg-o.jpg
catalog: true
tags:
    - 博客
    - Github Pages
---

## 前言

个人自用EFI文件，近期闲鱼收了一张Rx580，参考了大量的文章和其他前辈的EFI，做了整合和修改，在此感谢。

## 更新

- 2020-12-15
 	- 更新至BIG SUR 11.1
 	- 更换引导程序至OC 0.6.4

- 2020-05-25
	- 键盘、鼠标、网卡蓝牙接口内建
	- USB接口定制
	- 删除部分无用文件
	- 更新Clover 5118

- 2020-05-22
    - 初次上传

## 配置

 - CPU: i5-7500
 - 内存：金士顿 DDR4 2400MHz 8GB x 2
 - 硬盘：
      - 三星 SSD 860 EVO 250GB SATA
      - 三星 SSD 850 EVO M.2 250GB 
      - 西数机械蓝盘 1TB 
 - 风扇：酷冷至尊 暴雪T400i 
 - 显卡：蓝宝石 RX580 8G 2304SP
 - 网卡：Bcm94360CS2 + PCIE转接卡
 - 显示器：
    - 三星26.9英寸2K 144Hz 1800R曲面[已开启HIDPI]

## Bios设置
（参考以下常规选项进行设置）

### Disable
- Fast Boot
- Secure Boot
- Serial/COM Port
- Parallel Port
- VT-d
- CSM
- Thunderbolt
- Intel SGX
- Intel Platform Trust
- CFG Lock 

### Enable
- VT-x
- Above 4G decoding
- Hyper-Threading
- Execute Disable Bit
- EHCI/XHCI Hand-off
- OS type: Windows 8.1/10 UEFI Mode
- DVMT Pre-Allocated(iGPU Memory): 64MB
- SATA Mode: AHCI

## 工作状态

### 正常工作：

- 1.声卡 
- 2.网卡 
- 3.蓝牙 
- 4.Airdrop  
- 5.接力 
- 6.App store  
- 7.睡眠  
- 8.H.264、HEVC硬件解码、编码、视频处理
- 9.SATA SSD Trim（终端输入：sudo trimforce enable）

## 使用说明

- 需重新生成三码

## 致谢

 - [acidanthera](https://github.com/acidanthera)
 - [daliansky](https://github.com/daliansky/)
 - [Mrliu12123](http://bbs.pcbeta.com/viewthread-1851046-1-1.html)





















