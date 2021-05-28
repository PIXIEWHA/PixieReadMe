## ❤️ 2021-1 캡스톤디자인프로젝트B : 쓰레기 무단 투기 감시 시스템(PIXIE)

로고


## 📖 프로젝트 소개
PIXIE는 Raspberry Pi 4를 이용한 딥러닝 영상 처리 기반 쓰레기 무단 투기 감시 CCTV입니다.
무단투기 감지 및 영상 자동 저장, 삭제 기능을 탑재하였고, App으로 사용자가 간편하게 영상을 확인할 수 있습니다.

## 😀 개발 배경
 1. 최근 코로나로 인해 폐기물 양이 증가하면서 쓰레기 무단 투기 근절의 필요성이 대두되었다.
 2. 불법 폐기물 작년 8월 기준 39만 6천 톤
 3. 불법폐기물 추적 및 관리 강화 등 폐기물 투기 억제를 위한 대책 마련이 시급해졌다.

## 👨‍👩‍👦 팀원 소개
|학번|이름|
|------|---|
|1876379|정해인|
|1876264|이민영|
|1971030|유현정|

## 📁 Requirement Specification
![image](https://user-images.githubusercontent.com/67186222/119847320-d90ba600-bf45-11eb-84c9-e648fb23d688.png)

## 📲 System Architecture
![image](https://user-images.githubusercontent.com/67186222/117320715-759ed300-aec7-11eb-8abe-a3721b39b437.png)

## ⚙️ 진행 상황
  1. HW Raspberry Pi
      - WIFI
      - 영상 연동

  2. SW 알고리즘
      * YOLO 알고리즘/SSD 알고리즘
        - 모델 학습 코드 실행
        - 데이터 크롤링 및 AI Hub 영상 데이터 프레임 추출
        - 쓰레기 및 사람 & 쓰레기 무단 투기 행위 학습
        - 객체 좌표 추출
        - 실시간 영상 인식 테스트

  3. App
      - UI & Logo https://www.figma.com/file/F4vtMtcTMxIeKlkhGeQIvE/PIXIE?node-id=0%3A1
      - aws 데이터베이스

  4. 공모전, SW 저작권, 특허

## 😀 기술 블로그
- 유현정</br>
[[21-1 캡B] 0. 영상 데이터 프레임 추출](https://whyou-story.tistory.com/34)</br>
[[21-1 캡B] 1. Colab을 이용한 YOLOv5 Custom 학습 및 Inference](https://whyou-story.tistory.com/35)</br>

- 정해인</br>
[[2021-1] SSD 알고리즘을 통한 Object Detection](https://study-ai-eun.tistory.com/1)
