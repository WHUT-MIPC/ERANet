# <p align=center>  Real-Time Multi-Scene Visibility Enhancement for Promoting Navigational Safety of Vessels Under Complex Weather Conditions</p>

<div align="center">



</div>

---
>**Real-Time Multi-Scene Visibility Enhancement for Promoting Navigational Safety of Vessels Under Complex Weather Conditions**<br>  Ryan Wen Liu, Yuxu Lu *, Yuan Gao, Yu Guo, Wenqi Ren, Fenghua Zhu, and Fei-Yue Wang (* indicates corresponding author) <br> 
>Under Review

> **Abstract:** *The visible-light camera, which is capable of environment perception and navigation assistance, has emerged as an essential imaging sensor for marine surface vessels in intelligent waterborne transportation systems (IWTS). However, the visual imaging quality inevitably suffers from several kinds of degradations (e.g., limited visibility, low contrast, and color distortion, etc.) under complex weather conditions (e.g., haze, rain and low-lightness). The degraded visual information will accordingly result in inaccurate environment perception and delayed operations for navigational risk. To promote the navigational safety of vessels, many computational methods have been presented to perform visual quality enhancement under poor weather conditions. However, most of these methods are essentially \textit{specific-purpose} implementation strategies, only available for one specific weather type. To overcome this limitation, we propose to develop a \textit{general-purpose} multi-scene visibility enhancement method, i.e., edge reparameterization- and attention-guided neural network (ERANet), to adaptively restore the degraded images captured under different weather conditions. In particular, our ERANet simultaneously exploits the channel attention, spatial attention, and reparameterization technology to enhance the visual quality while maintaining low computational cost. Extensive experiments conducted on standard and IWTS-related datasets have demonstrated that our ERANet could outperform several representative visibility enhancement methods in terms of both imaging quality and computational efficiency. The superior performance of IWTS-related object detection and scene segmentation could also be steadily obtained after ERANet-based visibility enhancement under different weather conditions. The source code is freely available at \url{https://github.com/LouisYuxuLu/ERANet}.*
<hr />

## Requirement

- Python 3.7
- Pytorch 1.12.0

## Motivation
![Image](images/Motivation.jpg)

## Network Architecture
![Image](images/Network.jpg)

## Test
* Place the pre-training weight in the `checkpoint` folder.[README.md](..%2F..%2F..%2FEnhancement%2FDehazing%20method%2FCNN%20method%2FTOENet-main%2FREADME.md)
* For the dehazing task, place test hazy images in the `input/hazy` folder. Modify the `Type==2`,  the `line 55` of `test.py`.
* For the deraining task, place test rainy images in the `input/rainy` folder. Modify the `Type==0`,  the `line 55` of `test.py`.
* For the low-light enhancement task, place test low-light images in the `input/low` folder. Modify the `Type==2`,  the `line 55` of `test.py`.
* Run `test.py`
* The results are saved in `output/hazy` folder (dehazing), `output/rainy` folder (deraining), `output/low` folder (low-light enhancement).

## Dehazing Results
![Image](images/haze.jpg)

## Deraining Results
![Image](images/rain.jpg)

## Low-light Enhancement Results
![Image](images/low.jpg)

## Citation

```
Continue Update