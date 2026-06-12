# Skill Matrix

기술 스택은 단순 나열이 아니라 현재 수준, 근거, 다음 보완점을 함께 정리합니다. 프로젝트로 검증된 항목과 학습 중인 항목을 구분해 적습니다.

## 레벨 기준

| Level | 기준 |
| --- | --- |
| 1~2 | 개념을 들어봤거나 아주 기초만 아는 수준 |
| 3~4 | 기본 문법이나 사용법을 따라 할 수 있는 수준 |
| 5~6 | 작은 실습이나 실제 프로젝트 일부에 적용할 수 있는 수준 |
| 7~8 | 문제를 해결하면서 독립적으로 활용할 수 있는 수준 |
| 9~10 | 실무 수준으로 설계, 최적화, 디버깅, 설명까지 가능한 수준 |

## 기술 스택

| Category | Skill | Level | 현재 근거 | 다음 보완점 |
| --- | --- | --- | --- | --- |
| Programming | C | 5/10 | Arduino 펌웨어와 운영체제 실습 계획에 사용 | 포인터, 메모리 구조, 시스템 콜 실습 심화 |
| Programming | C++ | 4/10 | 로봇/임베디드 코드 구조와 ROS C++ 노드 학습 중 | 클래스 기반 구조화와 ROS package 작성 |
| Programming | Python | 6/10 | ROS node, 실험 자동화, 데이터 처리, 학습 코드 정리에 사용 | 객체지향 구조화와 실험 자동화 문서화 |
| Programming | MATLAB | 4/10 | 제어 계산, 딥러닝 예제 변환, RL 실험 코드 학습에 사용 | 제어/학습 실험 결과를 재현 가능한 형태로 정리 |
| Embedded | Arduino | 6/10 | 셀프 밸런싱 로봇의 실제 제어 펌웨어 구현 | 안전 조건, 통신, tuning 과정을 더 읽기 쉽게 정리 |
| Embedded | IMU / Sensor Input | 6/10 | BNO055 기반 body angle, gyro feedback을 균형 제어에 사용 | 보정, 필터링, drift 대응을 별도 문서화 |
| Embedded | ODrive / BLDC Motor | 5/10 | ODrive current command, hub motor feedback, staged tester sketch 정리 | motor bring-up 과정과 fault 대응 정리 |
| Robotics | ROS | 5/10 | topic, launch, Arduino-to-ROS bridge, simulation workflow 경험 | 실제 로봇과 simulation command layer 비교 보강 |
| Robotics | ROS2 | 2/10 | ROS1과의 차이와 전환 방향 학습 중 | 기본 node, launch, topic 구조 실습 |
| Robotics | Gazebo | 4/10 | 밸런싱 로봇 simulation, sensor workflow, navigation capture 정리 | sensor plugin, controller tuning 기록 보강 |
| Robotics | SLAM / Navigation | 3/10 | simulation map generation과 navigation command path 정리 | physical autonomous navigation과의 한계 분리 |
| Control | PID / Feedback Control | 6/10 | body angle feedback, speed loop, steering correction을 실제 로봇에 적용 | 실험 기반 tuning 과정과 증상별 대응 정리 |
| Control | Safety Layer | 6/10 | tilt cutoff, current clamp, RC filtering, engage persistence 구성 | safety boundary와 failure mode 문서화 |
| System/CS | Linux | 4/10 | ROS/Gazebo 환경과 운영체제 실습 환경으로 사용 | process, thread, file descriptor 실습 추가 |
| System/CS | 컴퓨터구조 | 4/10 | 책 1회독 후 핵심 개념 정리 | C/Linux 실습으로 동작 확인 |
| System/CS | 운영체제 | 4/10 | 프로세스, 스레드, 메모리, 파일 시스템 학습 | 시스템 콜 추적과 동기화 실습 |
| AI/RL | Deep Learning | 4/10 | KAIST 예제를 MATLAB으로 옮기며 ANN/CNN/GAN/RNN 계열 복습 | 학습 코드 실행 조건과 결과 요약 정리 |
| AI/RL | Reinforcement Learning | 4/10 | Q-learning, DDPG, reward 설계, Input Shaper 응용 실험 기록 | 로봇 제어 적용 범위와 안전 계층을 더 명확히 분리 |
| Mechanical/3D | CAD / Assembly | 5/10 | 밸런싱 로봇 body, board plate, sensor case, battery mount 정리 | assembly capture와 설계 의도 보강 |
| Mechanical/3D | 3D Printing | 5/10 | STL/STEP export, 출력 가능한 부품, design-to-print workflow 정리 | 실패/수정 기록을 반복 설계 관점으로 추가 |
| Documentation | Git/GitHub | 6/10 | 프로젝트, 학습 기록, 결과와 한계, README 구조 관리 | 커밋 단위와 공개 범위 기준 개선 |
| Documentation | Technical Writing | 5/10 | 한국어/영어 README, portfolio summary, limitations 문서 작성 | 면접용 요약과 긴 기술 문서의 균형 조정 |

## 실제 프로젝트 근거

- [Self-Balancing-Robot-with-Arduino-and-ROS](https://github.com/yg-gulbi/Self-Balancing-Robot-with-Arduino-and-ROS): 실제 하드웨어, firmware, ROS/Gazebo workflow, demo media, 결과와 한계를 포함한 중심 프로젝트

## 학습/응용 근거

- [rl-deep-learning-applied-notes](https://github.com/yg-gulbi/rl-deep-learning-applied-notes): Deep Learning, Q-learning, DDPG, Input Shaper 응용 학습 기록
- [3d-modeling-printing-notes](https://github.com/yg-gulbi/3d-modeling-printing-notes): CAD, assembly, STL/STEP export, 3D printing workflow 기록
- [study-notes](../study-notes/README.md): 운영체제, 제어, 로보틱스, 임베디드 학습 지도
