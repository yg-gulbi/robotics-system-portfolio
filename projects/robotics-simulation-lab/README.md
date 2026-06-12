# Robotics Simulation Lab

## 분류

이 문서는 완성된 프로젝트가 아니라 ROS/Gazebo 기반 시뮬레이션과 실제 로봇 workflow를 비교하기 위한 학습/실험 기록입니다.

## 학습 목적

실제 로봇 하드웨어만으로 모든 실험을 반복하기는 어렵습니다. 시뮬레이션 환경에서 로봇 모델, 센서, 제어 노드, navigation command path를 먼저 확인하면 실제 하드웨어 실험의 시행착오를 줄일 수 있습니다.

## 목표

- ROS 토픽과 노드 구조 이해
- Gazebo 로봇 모델링 실습
- 센서 토픽 흐름 확인
- 제어 노드 실험
- 실제 밸런싱 로봇의 command layer와 비교
- simulation result와 physical result의 경계 분리

## 사용 기술

- ROS
- Gazebo
- Python
- C++
- Linux

## 실습 흐름

```text
Gazebo Robot Model
  -> Sensor Topic
  -> ROS Node
  -> Command Layer
  -> Simulation Result
  -> Physical Robot Comparison
```

## 현재 상태

기본 구조와 관련 개념을 정리하는 단계입니다. 실제 하드웨어 결과가 있는 중심 프로젝트와 분리해, simulation workflow를 이해하기 위한 보조 기록으로 둡니다.

## 다음 보완점

- 로봇 모델과 launch 구조 정리
- 센서 플러그인 실습
- 제어 노드 실험 결과 정리
- ROS2 전환 학습
- 실제 로봇 command layer와의 비교표 작성

## 포트폴리오 요약

ROS/Gazebo 기반 로봇 모델링, 센서 토픽, 제어 노드, navigation workflow를 실제 로봇 프로젝트와 비교하기 위한 학습/실험 기록입니다.
