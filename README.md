## ❤️ 2021 캡스톤디자인프로젝트B : 딥러닝 기반 저비용 주택가 쓰레기 무단 투기 인식 시스템(PIXIE)
<img src="https://user-images.githubusercontent.com/67186222/120105425-c8506f80-c193-11eb-8533-0be46aef75b4.jpg" width="40%">

## 📖 프로젝트 소개
PIXIE는 Raspberry Pi 4를 이용한 딥러닝 기반 저비용 주택가 쓰레기 무단 투기 감시 CCTV입니다.
무단투기 감지 및 영상 자동 저장, 삭제 기능을 탑재하였고, App으로 사용자가 간편하게 영상을 확인할 수 있습니다.

## 😀 개발 배경
 1. 최근 코로나로 인해 폐기물 양이 증가하면서 쓰레기 무단 투기 근절의 필요성이 대두되었다.
 2. 아파트에 비해 관리 및 감시가 소홀한 주택가 쓰레기 무단 투기
 3. 불법 폐기물 작년 8월 기준 39만 6천 톤
 4. 무단 투기 쓰레기 관리 강화 등 폐기물 투기 억제를 위한 대책 마련이 시급해졌다.

## 👨‍👩‍👦 팀원 소개
|학번|이름|
|------|---|
|1876379|정해인|
|1876264|이민영|
|1971030|유현정|

## 📲 System Architecture
![image](https://user-images.githubusercontent.com/67186222/141682460-11b75f69-d0f4-44aa-94a5-d3024348288f.png)


## ⚙️ 진행 상황
  1. HW Raspberry Pi
      - WIFI
      - 영상 녹화 및 DB 저장

  2. SW 알고리즘
      * Object Detection
        - 데이터 크롤링 및 AI Hub 영상 데이터 프레임 추출
        - 사람 & 손 혹은 팔과 함께 있는 물건 라벨링
        - 무단 투기 행위 학습
      
      * Tracking Algorithm
        - 객체 좌표 추출 및 Box Collision
        - 영상 인식 테스트
      
      * OpenPose
        - Coco Model
        - 영상 테스트

  3. App
      - UI & Logo https://www.figma.com/file/F4vtMtcTMxIeKlkhGeQIvE/PIXIE?node-id=0%3A1
      - AWS & Firebase 데이터베이스

  4. 공모전
      * 제4회 KB소프트웨어 경진대회 입상(본선 진행 중)
      * 캡스톤디자인경진대회 은상
  
  5. SW 저작권(심사 중)

## 😀 기술 블로그
- 유현정</br>
[[21-1 캡B] 0. 영상 데이터 프레임 추출](https://whyou-story.tistory.com/34)</br>
[[21-1 캡B] 1. Colab을 이용한 YOLOv5 Custom 학습 및 Inference](https://whyou-story.tistory.com/35)</br>
[[21-2 캡A] 3. 라즈베리파이 초기 세팅 & 4. Docker 명령어 정리](https://whyou-story.tistory.com/45)</

- 정해인</br>
[[2021-1] SSD 알고리즘을 통한 Object Detection](https://study-ai-eun.tistory.com/1)</br>

- 이민영</br>
[Python, OpenPose를 활용하여 인체의 자세 감지하기](https://mignon-cs.tistory.com/2)
