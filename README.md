# 데이터 크레이터 캠프\n(Data Creator Camp)
## 일정
25.08.13 ~ 25.09.26
## 세부 사항
빅데이터 센터에서 운영하는 **데이터 캠프**
https://kbig.kr/portal/kbig/keybiz.page

**aihub 데이터셋** : 대기오염 배출원 공간 분포 데이터

이러닝 교육과 함께 미션을 수행하고 미션 결과에 따라 본선 진출

## 주제 
위성 이미지 멀티모달 딥러닝을 이용한 대기오염 배출원 탐지

### mission1
굴뚝 위치 탐지 (Detection)
  이미지와 bbox 박스의 josn 파일을 통해 training, validation 진행
    - json파일
      파일정보 : 
        파일명, 파일크기, 이미지id, 이미지 제공처, 이미지크기, 촬영 해상도, 촬영시간
      영역 정보 :
        영역id, 영역형태, 영역좌표(x, y, 너비, 높이)
    - 목표 : 굴뚝 위치 bbox 값을 예측

### mission2
굴뚝 높이 추정 (Estimation)
  이미지와 높이, bbox의 json 파일을 통해 training, validation 진행
    - json파일
      파일정보 : 
        파일명, 파일크기, 이미지id, 이미지 해상도, 이미지 촬영 해상도, 촬영시간, 이미지 제공처
      영역정보 : 
        영역id, 영역형태, 영역좌표(x,y), 영역속성(높이)
    - 목표 : 굴뚝 높이를 meter 단위로 예측

### mission3
산업단지 영역 분할(Segmentation)
  이미지와 라벨링데이터(세그멘테이션)을 통해 training, validation 진행
    - 목표 : 이미지 내의 산업단지의 영역 분할