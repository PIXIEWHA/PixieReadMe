<div align="center">
  <h1>딥러닝 기반 저비용 주택가 쓰레기 무단 투기 인식 시스템(PIXIE)</h1>
  <img src="https://user-images.githubusercontent.com/67186222/120105425-c8506f80-c193-11eb-8533-0be46aef75b4.jpg" alt="pixie" width="300px" height="200px">    <img src="https://user-images.githubusercontent.com/67186222/144769445-dba8e1d7-5bfe-40d8-a6df-c95ec628c409.png" alt="pixie" width="200px" height="200px">
  <br />
</div>
<br />

## 목차
1. [**프로젝트 소개**](#1)
1. [**기술 스택**](#2)
1. [**주요 기능**](#3)
1. [**프로젝트 구성도**](#4)
1. [**발표 자료 및 데모 영상**](#5)
1. [**팀원 소개**](#6)
1. [**기간 및 일정**](#7)
1. [**수상 및 성과**](#8)
1. [**실행 방법**](#9)
1. [**기술 블로그**](#10)
<br />

<div id="1"></div>

## 📖 프로젝트 소개
>PIXIE는 Raspberry Pi 4를 이용한 딥러닝 기반 저비용 주택가 쓰레기 무단 투기 감시 CCTV입니다.<br/>
무단투기 감지 및 영상 자동 저장, 삭제 기능을 탑재하였고, App으로 사용자가 간편하게 영상을 확인할 수 있습니다.
<br/>

**개발 배경** 😀
 1. 최근 코로나로 인해 폐기물 양이 증가하면서 쓰레기 무단 투기 근절의 필요성
 2. 아파트에 비해 관리 및 감시가 소홀한 주택가 쓰레기 무단 투기
 3. 불법 폐기물 작년 8월 기준 39만 6천 톤
 4. 무단 투기 쓰레기 관리 강화 등 폐기물 투기 억제를 위한 대책 마련 시급

<br />

<div id="2"></div>

## ⚙️ 기술 스택
![](https://img.shields.io/badge/%20-raspberrypi4-red)
![](https://img.shields.io/badge/%20%20yolo-v5.0-black)
![](https://img.shields.io/badge/%20-deepsort-navy)
![](https://img.shields.io/badge/opencv-v4.5.2-brightgreen)
![](https://img.shields.io/badge/flutter-2.2.0-blue)
![](https://img.shields.io/badge/%20python-3.9.13-black)
![](https://img.shields.io/badge/pytorch-v1.9.0-black)
![](https://img.shields.io/badge/%20django-3.1-black)
![](https://img.shields.io/badge/mysql-8.0.27-informational)
<br/>
![](https://img.shields.io/badge/%20-colab-orange)
![](https://img.shields.io/badge/%20-aws-orange)
![](https://img.shields.io/badge/%20-firebase-skyblue)
![](https://img.shields.io/badge/%20-docker-blue)
![](https://img.shields.io/badge/%20%20-talend%20API%20tester-navy)
<br /><br/>

<div id="3"></div>

## 📲 주요 기능

| <div align="center"/>기능                      | <div align="center"/>내용                                                  |
| :------------------------ | :---------------------------------------------------------------------------------------------------------------------------------- |
| <div align="center"/>HW RaspberryPI|- WIFI<br/>- 영상 녹화 및 Firebase에 업로드|
| <div align="center"/>🔗[**SW 알고리즘(server)**](https://github.com/yhyeonjg/server)|- Object Detection<br/>&nbsp;&nbsp;&nbsp;&nbsp;- 데이터 크롤링 및 AI Hub 영상 데이터 프레임 추출<br/>&nbsp;&nbsp;&nbsp;&nbsp;- 사람 & 손 혹은 팔과 함께 있는 물건 라벨링<br/>&nbsp;&nbsp;&nbsp;&nbsp;- 무단 투기 행위 학습<br/> - Tracking Algorithm<br/>&nbsp;&nbsp;&nbsp;&nbsp;- 객체 좌표 추출 및 Box Collision<br/>&nbsp;&nbsp;&nbsp;&nbsp;- 영상 인식 테스트<br/>- OpenPose<br/>&nbsp;&nbsp;&nbsp;&nbsp;- Coco Model로 사람 관절 인식<br/>&nbsp;&nbsp;&nbsp;&nbsp;- 영상 테스트<br/>&nbsp;&nbsp;&nbsp;&nbsp;- 사람과 물체 ID 좌표를 프레임별로 저장<br/>&nbsp;&nbsp;&nbsp;&nbsp;- 이전 프레임과 비교하여 사람은 있으나 물건 없고, 목-골반 선 < 45도 or 손목-발목 선 < 45도 투기 인식|
| <div align="center"/>🔗[**프론트엔드**](https://github.com/yhyeonjg/frontEnd)|- 라즈베리파이 IP 등록<br/>- Firebase 서버에 있는 무단 투기 영상 확인 및 알림<br/>- URL 복사하여 편리하게 무단 투기 신고|
| <div align="center"/>🔗[**백엔드**](https://github.com/yhyeonjg/backEnd)|- aws에 회원정보 저장<br/>- 라즈베리파이 IP 관리<br/>- Firebase 영상 관리|
      
<br /><br/>

<div id="4"></div>

## 🗄️ 프로젝트 구성도
| <div align="center"/>Architecture|                                                                                                                    
| :------------------------ |
| <div align="center"/><img src="https://user-images.githubusercontent.com/67186222/141682460-11b75f69-d0f4-44aa-94a5-d3024348288f.png" alt="architecture" width="800px" height="700px"/>|

<br /><br/>

<div id="5"></div>

## 📽️ 발표 자료 및 데모 영상
| <div align="center"/>최종 발표| <div align="center">제품 설명서|<div align="center">데모 영상|
| :------------------------ | :--------------------------- |:--------------------------- |
|🔗[**최종 발표**](https://drive.google.com/file/d/1IBnjZ1DAAoEtjlLwZWXu2DJc8TzBNmpJ/view?usp=share_link)|🔗[**제품 설명서**](https://drive.google.com/file/d/1iP_FMtDNcuyShnV-5o1UdswF_vIewaIl/view?usp=share_link)|🔗[**데모 영상**](https://drive.google.com/file/d/1bYeX2mmJJKr1Bi3aQRI-wrcAj_3AOWlf/view?usp=share_link)|

<br />

<div id="6"></div>

## 👨‍👩‍👦 팀원 소개
|학번|이름|개발업무|
|------|---|----|
|1876379|정해인|- 데이터셋 구하기<br/>- 영상 프레임 추출<br/>- 데이터 라벨링 및 어그멘테이션<br/>- Yolo 및 SSD 모델 조사|
|1876264|이민영|- 데이터셋 구하기<br/>- 데이터 라벨링 및 어그멘테이션<br/>- RaspberryPI 조립<br/>- OpenPose 적용|
|1971030|유현정|- 데이터 라벨링 및 영상 프레임 추출<br/>- RaspberryPI 카메라 촬영 및 업로드<br/>- UI 및 Flutter & Django 개발<br/>- DeepSORT 및 OpenPose 적용<br/>- Yolo모델 Custom Training<br/>- AWS, Firebase 등 Integration|
<br/>

<div id="7"></div>

## 📅 기간 및 일정
**2021.3~2022.2**
<br />
<br/>

<div id="8"></div>

## 🏆 수상 및 성과
**1. 제4회 KB소프트웨어 경진대회 특별상**
<br/>

**2. 캡스톤디자인경진대회 은상**
<br/>

**3. SW 저작권 등록**
<br /><br />

<div id="9"></div>

## 💡 실행 방법
### Client 환경
> 🔗[**apk 파일**](https://drive.google.com/file/d/14LaYov-2ddF-LvXdT60Z9SGFr4kFCOee/view?usp=sharing) 실행
<br/>

### 개발환경
**1. 원격 저장소 복제**

```bash
$ git clone https://github.com/yhyeonjg/frontEnd.git
$ git clone https://github.com/yhyeonjg/backEnd.git
$ git clone https://github.com/yhyeonjg/server.git
```
**2. aws 및 firebase, app Key**
> aws 및 firebase, app Key 등록
<br/>

<div id="10"></div>

## 🖥️ 기술 블로그
**유현정**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;🔗[[캡스톤B] 1. 영상 데이터 프레임 추출](https://whyou-story.tistory.com/34)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;🔗[[캡스톤B] 2. Colab을 이용한 YOLOv5 Custom 학습 및 Inference](https://whyou-story.tistory.com/35)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;🔗[[캡스톤A] 4. 라즈베리파이 초기 세팅](https://whyou-story.tistory.com/40)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;🔗[[캡스톤A] 5. Docker 명령어 정리](https://whyou-story.tistory.com/45)
<br/>

**정해인**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;🔗[[2021-1] SSD 알고리즘을 통한 Object Detection](https://study-ai-eun.tistory.com/1)
<br/>

**이민영**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;🔗[Python, OpenPose를 활용하여 인체의 자세 감지하기](https://mignon-cs.tistory.com/2)
<br/>
