# 박석환 | Software · Embedded · Hardware Portfolio

영상처리·센서 데이터 처리, MCU·RTOS 기반 제어, FPGA·SoC 설계 및 검증 프로젝트를 정리한 포트폴리오입니다.
프로젝트별 구현 내용, 코드, 검증 결과는 아래 링크에서 확인할 수 있습니다.

| 분야 | 프로젝트 | 저장소 |
|---|---|---|
| **Software** | 카메라·LiDAR 융합 자율주행 시스템, 특징점 기반 파노라마 스티칭 | [SW 포트폴리오 보기](https://github.com/seokhwanpark02/software_portfolio) |
| **Embedded** | STM32 3-MCU 센서·구동 분산 제어, Zynq 엣지 AI 영상 분류 | [Embedded 포트폴리오 보기](https://github.com/seokhwanpark02/Embedded_Portfolio) |
| **Hardware** | AXI4 DMA·CDC, 3×3 멀티코어 이미지 필터 RTL, Zynq PS–PL GEMM 통합 | [HW 포트폴리오 보기](https://github.com/seokhwanpark02/Hardware-portfolio) |

## Software Projects

| 프로젝트 | 다룬 내용 | 주요 기술 | 상세 내용 |
|---|---|---|---|
| **카메라·LiDAR 융합 자율주행 시스템** | 카메라 마스크의 BEV 변환, 센서 데이터 결합, 경로 CNN과 차량 제어 통합, Replay 기반 문제 재현 및 추론 지연 분석 | Python · ROS 2 · OpenCV · PyTorch · OpenVINO | [프로젝트 보기](https://github.com/seokhwanpark02/software_portfolio/tree/main/autonomous-driving) |
| **특징점 기반 파노라마 스티칭** | NumPy·PIL로 코너 검출, 특징점 매칭, 호모그래피 추정, 역방향 워핑·블렌딩 및 노출 보정 구현 | Python · NumPy · PIL | [프로젝트 보기](https://github.com/seokhwanpark02/software_portfolio/tree/main/panorama-stitching) |

## Embedded Projects

| 프로젝트 | 다룬 내용 | 주요 기술 | 상세 내용 |
|---|---|---|---|
| **STM32 3-MCU 센서·구동 분산 제어** | 센싱·구동, 중앙 판단, 외부 통신을 세 MCU에 분산하고 SPI로 연결. ADC Circular DMA, 히스테리시스, 통신 Timeout 복구 적용 | C · STM32 · ADC/DMA · SPI · Timer PWM | [프로젝트 보기](https://github.com/seokhwanpark02/Embedded_Portfolio/tree/main/stm32-distributed-control) |
| **Zynq 엣지 AI 영상 분류** | 센서 감지부터 영상 분류·구동까지 연결. PS–PL CNN 추론 연동, FreeRTOS 수신·추론 Task 분리, DMA 완료 동기화 | C · FreeRTOS · Zynq · AXI DMA · Vivado/Vitis | [프로젝트 보기](https://github.com/seokhwanpark02/Embedded_Portfolio/tree/main/zynq-edge-ai) |

## Hardware Projects

| 프로젝트 | 다룬 내용 | 주요 기술 | 상세 내용 |
|---|---|---|---|
| **AXI4 DMA·CDC 데이터 전송 엔진** | AXI4-Lite·AXI4 Read·AXI4-Stream 인터페이스, 클록 도메인 간 데이터 전달, 회귀 검증 및 타이밍 분석 | SystemVerilog · SVA · cocotb · Vivado | [프로젝트 보기](https://github.com/seokhwanpark02/Hardware-portfolio/tree/main/axi_dma_cdc) |
| **3×3 멀티코어 이미지 필터 RTL** | 9개 프로세서의 이미지 필터 처리, barrier 동기화, 레퍼런스 기반 출력 대조 및 검증 | SystemVerilog · SVA · C++ · Verilator | [프로젝트 보기](https://github.com/seokhwanpark02/Hardware-portfolio/tree/main/multicore_rtl) |
| **Zynq PS–PL INT16 GEMM 통합** | PS의 PL 가속기 제어, INT16 GEMM 연산 연동, CPU 레퍼런스와 결과 비교 | Python · Zynq · AXI/DMA | [프로젝트 보기](https://github.com/seokhwanpark02/Hardware-portfolio/tree/main/zynq_ps_pl_gemm) |

## 프로젝트에서 다룬 역량

- **영상·센서 처리:** 카메라 좌표 변환, 센서 입력 전처리 및 시간 동기화, 영상 합성
- **실시간 처리와 디버깅:** 최신 프레임 우선 처리, 추론 최적화, 기록 데이터 재생 및 전류 계측
- **임베디드 제어:** MCU 센서 입력·PWM 구동, SPI 통신, RTOS Task, 인터럽트·DMA 활용
- **하드웨어 설계와 통합:** RTL, AXI 인터페이스, CDC, 멀티코어 동기화, PS–PL 연동
- **검증:** 단위 테스트, 레퍼런스 기반 결과 대조, SVA·fault injection, 회귀 검증 및 타이밍 분석
