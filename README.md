# Robotics System Portfolio

실제 구현 근거가 있는 로봇 프로젝트와, 아직 학습 중인 지식 지도를 분리해 정리하는 포트폴리오 저장소입니다.

완성되지 않은 공부 내용을 프로젝트처럼 포장하지 않고, 하드웨어, 코드, 데모, 문서가 있는 결과물은 프로젝트로 두며 나머지는 학습 기록과 응용 실험 근거로 분류합니다.

## Website

- GitHub Pages: https://yg-gulbi.github.io/robotics-system-portfolio/

## 방향

- 프로젝트는 실제 결과물, 코드, 하드웨어, 데모 근거가 있을 때만 프로젝트로 둡니다.
- 학습 중인 내용은 지식 지도, 실습 계획, 응용 실험 기록으로 분리합니다.
- 기술 수준은 점수보다 근거와 다음 보완점이 함께 보이도록 정리합니다.
- 언어는 읽기, 쓰기, 말하기 기준으로 현재 근거가 있는 만큼만 표시합니다.

## 핵심 기술 스택 요약

| 영역 | 현재 정리 방향 |
| --- | --- |
| Programming | C, C++, Python, MATLAB을 펌웨어, ROS, 실험 자동화, 제어 계산 용도로 구분 |
| Embedded | Arduino, IMU, ODrive, BLDC Motor, RC PWM, 안전 조건을 실제 로봇 근거와 연결 |
| Robotics | ROS, Gazebo, SLAM, Navigation workflow를 simulation과 command layer 관점으로 정리 |
| Control | PID, body angle feedback, speed loop, steering correction, safety layer 중심으로 설명 |
| System/CS | 컴퓨터구조, 운영체제, Linux, 시스템 콜을 학습 기록과 실습 계획으로 정리 |
| AI/RL | Deep Learning, Q-learning, DDPG, Input Shaper 실험을 응용 학습 근거로 분류 |
| Mechanical/3D | CAD, 3D printing, sensor case, board plate, packaging을 하드웨어 설계 근거로 연결 |
| Documentation | README, 결과와 한계, 이력서 요약 문장을 과장 없이 정리 |

자세한 기술 수준은 [tech-stack/skill_matrix.md](tech-stack/skill_matrix.md)에 정리했습니다.

## 대표 프로젝트

| 프로젝트 | 상태 | 요약 |
| --- | --- | --- |
| [self-balancing-robot](projects/self-balancing-robot/README.md) | 실제 하드웨어/코드/데모 근거 보유 | Arduino 기반 2륜 셀프 밸런싱 로봇을 제작하고, ROS/Gazebo workflow와 연결해 정리한 중심 프로젝트 |

원본 프로젝트 저장소:

- [Self-Balancing-Robot-with-Arduino-and-ROS](https://github.com/yg-gulbi/Self-Balancing-Robot-with-Arduino-and-ROS)

## 지식 지도와 응용 학습 기록

| 영역 | 정리 방식 |
| --- | --- |
| [computer-architecture-os](study-notes/computer-architecture-os/README.md) | 컴퓨터구조와 운영체제를 C/Linux 실습으로 확인하기 위한 학습 기록 |
| [control-theory](study-notes/control-theory/README.md) | 균형 로봇의 자세 제어를 이해하기 위한 PID, 상태공간, feedback 개념 정리 |
| [robotics](study-notes/robotics/README.md) | ROS, Gazebo, 센서, SLAM, Navigation을 실제 로봇 workflow와 비교하기 위한 기록 |
| [embedded-system](study-notes/embedded-system/README.md) | Arduino, 센서 입력, 모터 제어, 통신, 실시간 제어 기초 정리 |
| [rl-deep-learning-applied-notes](https://github.com/yg-gulbi/rl-deep-learning-applied-notes) | 강화학습과 딥러닝을 제어 응용 관점으로 정리한 학습/실험 저장소 |
| [3d-modeling-printing-notes](https://github.com/yg-gulbi/3d-modeling-printing-notes) | CAD, assembly, STL/STEP export, 3D printing workflow 정리 저장소 |

## 언어

- [Languages](languages/README.md): 읽기, 쓰기, 말하기 기준의 언어 역량과 날짜별 변화
- [Japanese](languages/japanese.md): JLPT N2를 장기 목표로 둔 일본어 학습 기록
- [English](languages/english.md): 기술 문서 독해와 README 작성 중심의 영어 기록

언어 역량은 현재 자격증이나 점수를 과장하지 않고, 실제 학습 로그와 문서화 근거에 맞춰 보수적으로 표시합니다.

## 현재 보완 중인 내용

- 밸런싱 로봇 프로젝트의 결과, 한계, 안전 계층을 포트폴리오 요약으로 압축
- 운영체제와 시스템 개념을 C/Linux 실습 단위로 정리
- ROS/Gazebo simulation workflow와 실제 로봇 command layer의 차이를 문서화
- 언어 학습 기록을 읽기, 쓰기, 말하기 기준으로 갱신

## 하단 소개 방향

이 포트폴리오는 로보틱스 개발자로서의 기록뿐 아니라, 기록하고 배우는 사람으로서의 모습도 함께 보여줍니다. 언어 학습, 클라이밍, 문장으로 생각을 정리하는 습관은 기술 밖의 시간이지만 문제를 바라보는 방식과 연결됩니다.
