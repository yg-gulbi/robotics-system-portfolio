# Control Theory

## 학습 목적

제어공학은 단순 공식 암기가 아니라 실제 균형 로봇이 어떻게 넘어지지 않고 움직이는지 이해하기 위한 도구로 정리합니다.

## 현재 범위

- PID 제어
- 상태공간의 기본 개념
- body angle feedback
- speed loop
- steering correction
- safety layer

## 포트폴리오 연결

셀프 밸런싱 로봇에서는 body angle과 angular velocity를 기반으로 자세를 잡고, throttle 입력은 speed loop를 통해 balance-compatible한 움직임으로 바뀝니다. steering correction은 좌우 모터 전류 차이를 만들고, tilt cutoff와 current clamp는 위험한 상태가 모터 명령으로 이어지지 않게 합니다.

## 현재 이해한 점

- 균형 로봇은 body angle feedback만으로 끝나지 않고 speed loop, steering correction, safety layer가 함께 필요합니다.
- 실제 하드웨어에서는 센서 노이즈, RC PWM drift, motor feedback 이상값 때문에 filtering과 safety boundary가 중요합니다.
- 상위 명령은 직접 모터 명령이 아니라 motion intent로 다루는 편이 안전합니다.

## 다음 보완점

- PID tuning 과정과 증상별 대응 표 정리
- IMU filtering과 보정 기록 추가
- speed loop와 steering correction의 역할을 그림으로 요약
- simulation controller와 physical controller의 차이 정리

## 관련 프로젝트

- [self-balancing-robot](../../projects/self-balancing-robot/README.md)

## 한 줄 요약

제어공학 개념을 균형 로봇의 body feedback, speed loop, steering correction, safety layer와 연결해 정리하는 학습 자료입니다.
