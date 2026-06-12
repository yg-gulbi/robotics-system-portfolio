# Self Balancing Robot

## 프로젝트 개요

2륜 셀프 밸런싱 로봇을 직접 제작하고, Arduino 기반 실시간 자세 제어와 ROS/Gazebo workflow를 함께 정리한 중심 프로젝트입니다.

원본 저장소:

- [Self-Balancing-Robot-with-Arduino-and-ROS](https://github.com/yg-gulbi/Self-Balancing-Robot-with-Arduino-and-ROS)

## 문제 정의

2륜 로봇은 정적으로 불안정하기 때문에 IMU, wheel feedback, RC 입력, 모터 명령, 안전 조건이 하나의 신뢰 가능한 루프로 연결되어야 합니다. 상위 명령이 모터로 바로 전달되면 작은 센서 노이즈나 잘못된 입력도 넘어짐으로 이어질 수 있으므로, low-level balance loop와 safety layer를 분리해 다루는 것이 중요했습니다.

## 실제 결과

| 항목 | 결과 |
| --- | --- |
| 실제 균형 유지 | 약 1시간 standing balance |
| 실제 주행 | 10m 복도 주행 |
| 장애물 주행 | 간단한 실내 장애물 코스 수행 |
| ROS/Gazebo | simulation, SLAM map generation, navigation command path 문서화 |
| Arduino-to-ROS | `/imu`, `/odom`, `cmd_vel` 흐름을 bridge sketch와 실험 기록으로 보존 |

## 목표와 범위

- IMU 기반 body angle과 gyro feedback으로 자세 안정화
- RC PWM 입력을 filtering, deadband, engage persistence로 안정화
- ODrive current command와 BLDC hub motor feedback 연결
- tilt cutoff와 current clamp로 safety boundary 구성
- ROS/Gazebo simulation과 실제 Arduino control path의 차이 정리
- physical full autonomous navigation은 완료 결과가 아니라 future work로 분리

## 사용 기술

- Arduino Mega 2560
- C/C++
- BNO055 IMU
- ODrive 3.6
- BLDC hub motor
- RC receiver / PWM input
- PID / body angle feedback
- ROS / Gazebo
- Linux
- CAD / 3D printing

## 시스템 구조

```text
RC or ROS-side intent
  -> Arduino safety checks
  -> body angle feedback
  -> speed loop
  -> steering correction
  -> current clamp
  -> ODrive
  -> BLDC motors
  -> robot motion
```

ROS/Gazebo는 실제 로봇의 command structure, simulation workflow, SLAM/navigation 실험을 설명하는 보조 축으로 정리합니다.

## 구현 내용

- IMU 기반 body angle, angular velocity feedback 처리
- RC throttle, steering, engage PWM filtering
- tilt cutoff와 current clamp를 통한 안전 조건 적용
- ODrive current command 기반 모터 제어
- ROS/Gazebo simulation, navigation command routing, SLAM workflow 구성
- CAD/3D printing 기반 sensor case, board plate, battery mount 정리

## 결과와 한계

이 프로젝트의 강한 근거는 실제 balancing과 RC driving입니다. ROS/Gazebo 쪽은 simulation navigation과 SLAM workflow를 완료된 software-side 결과로 다루고, 실제 로봇의 end-to-end autonomous navigation은 아직 future work로 분리합니다.

## 배운 점

- 균형 로봇은 제어식 하나보다 센서, 통신, 모터, 안전 조건이 함께 맞아야 안정화됩니다.
- RC 입력과 모터 feedback은 노이즈와 이상값을 전제로 다뤄야 합니다.
- 상위 navigation 명령은 직접 모터 권한이 아니라 motion intent로 다루는 것이 안전합니다.
- 공개 포트폴리오에서는 completed result, simulation result, future work를 분리해야 과장이 줄어듭니다.

## 다음 보완점

- tuning 과정과 증상별 대응을 더 짧은 표로 정리
- IMU 보정과 filtering 근거 보강
- ROS/Gazebo workflow와 실제 robot control loop의 차이를 그림으로 요약
- 3D printed part의 설계 의도와 assembly 근거 연결

## 포트폴리오 요약

Arduino 기반 2륜 셀프 밸런싱 로봇을 직접 제작하며 IMU feedback, RC 신호 처리, ODrive current command, safety layer, ROS/Gazebo workflow를 통합하고 문서화한 프로젝트입니다.
