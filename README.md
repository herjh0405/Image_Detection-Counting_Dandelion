# 🌼 [NIMS] Image Detection - Counting Dandelion
---
## 개요

국가수리과학 연구소 산업수학 아카데미 (2020/11/05 - 2020/11/08)
* 딥러닝을 이용하여 개화한 민들레 꽃의 갯수를 세는 프로그램 구축
  * 라벨링부터 모델 구현까지 작업
  * Detectron2의 faster_rcnn, retinanet 두 가지 모델 비교

---
## 개발 환경
**[서버 사양]** 서버 : Colab
> * CPU 1, 메모리 12GiB, CUDA Version: 11.2
> * Ubuntu 18.04.5 LTS

**[개발 환경]**
> * 파이썬 : Python 3.7.10
> * 파이썬 라이브러리
>   * torch 1.7.1+cu101
>   * detectron2 0.3
>   * opencv 4.1.2

**[데이터 출처]**
> * NIMS 제공 [data](https://github.com/herjh0405/Image_Detection-Counting_Dandelion/blob/master/dandelion.zip)
>   * 4-5월 한 달간 일정한 시간대에 같은 각도로 촬영한 민들레 꽃 데이터
> * 라벨링 사이트 [link](http://www.robots.ox.ac.uk/~vgg/software/via/via.html)
>   * Bounding Box : 직사각형

---
## 결과 비교
* 왼쪽 사진이 Faster_rcnn_R_101_FPN_3x, 오른쪽 사진이 Retinanet_R_101_FPN_3x의 결과이다.
  * LR=0.0025, Max_Iter=500, BATCH_SIZE=128 조건하에 시행하였고 Faster_rcnn이 더 좋은 효과를 보임

<div class="imgCollage"> 
 <span style='max-width:30%;'> <img src = "https://user-images.githubusercontent.com/54921730/109373991-82b2ab00-78f5-11eb-836f-3a1e6220a117.png" width=500 max-width=50% height = 350/> </span> 
 <span style='max-width:30%;'> <img src = "https://user-images.githubusercontent.com/54921730/109375334-4e43ec80-78ff-11eb-93e3-34d3993fcaf6.png" width=500 max-width=50% height = 350/> </span> 
</div>

---
## 결과 시각화 

* 새로운 사진이 주어졌을 때 민들레 꽃을 높은 확률로 Detection해냄을 알 수 있다.

<img src = "https://user-images.githubusercontent.com/54921730/109375209-518aa880-78fe-11eb-87b2-70f6a2200122.png" width = 1000 max-width=100% height = auto/>



