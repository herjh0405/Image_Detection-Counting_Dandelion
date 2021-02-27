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
* Faster_Rcnn Resinanet

<div class="imgCollage"> 
 
 <html lang="ko">
	<head>
		<meta charset="utf-8">
		<title>CSS</title>
		<style>
			.jb-wrap {
				width: 40%;
				margin: 10px auto;
				border: 1px solid #000000;
			}
			.jb-wrap img {
				width: 100%;
				vertical-align: middle;
			}
			.jb-text {
				padding: 5px 10px;
				background-color: yellow;
				text-align: center;
			}
		</style>
	</head>
	<body>
		<div class="jb-wrap">
			<div class="jb-image"><img src="https://user-images.githubusercontent.com/54921730/109373991-82b2ab00-78f5-11eb-836f-3a1e6220a117.png" alt=""></div>
			<div class="jb-text">
				<p>Faster_Rcnn</p>
			</div>
		</div>
	</body>
</html>
 <span style="width: 40%"> <img src = "https://user-images.githubusercontent.com/54921730/109373991-82b2ab00-78f5-11eb-836f-3a1e6220a117.png" width = 450 max-width=40% height = 350/> </span> 
 <span style="display: inline-blockl height:20px; width:100px;"> VS </span>        
 <span style="width: 40%"> <img src = "https://user-images.githubusercontent.com/54921730/109374207-f0aba200-78f6-11eb-914e-1c1ba4c6a88e.png" width = 450 max-width=40% height = 350/> </span> 
</div>



