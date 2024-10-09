# 2주차: 시스템 관리 및 운영 개론

## 1. 시스템 관리의 개념 (슬라이드 1)
### 시스템 관리란 무엇인가?
시스템 관리는 컴퓨터 시스템, 서버, 네트워크 장치 등의 안정적인 운영을 보장하는 프로세스입니다. 시스템 관리자는 시스템의 성능을 유지하고, 보안과 데이터 무결성을 보장하며, 시스템 장애를 예방하고 해결하는 역할을 합니다.

- **시스템 관리 주요 목표**:
  1. 시스템의 가용성 보장
  2. 시스템 성능 최적화
  3. 보안 관리
  4. 문제 해결 및 장애 복구

## 2. 운영체제의 역할과 기능 (슬라이드 2)
운영체제는 컴퓨터 하드웨어와 소프트웨어를 관리하고, 사용자와 컴퓨터 간의 상호작용을 제어하는 중요한 소프트웨어입니다.

- **운영체제의 주요 기능**:
  1. **프로세스 관리**: 프로그램 실행을 제어하고, 여러 프로그램이 동시에 실행될 때 CPU 자원을 할당합니다.
  2. **메모리 관리**: 메모리 자원을 효율적으로 분배하고, 프로그램 간의 메모리 충돌을 방지합니다.
  3. **파일 시스템 관리**: 파일과 디렉터리를 생성, 삭제, 조회, 저장하는 기능을 제공합니다.
  4. **네트워크 관리**: 데이터의 송수신을 제어하고 네트워크 연결을 관리합니다.

## 3. 프로세스 및 메모리 관리 (슬라이드 3)
### 프로세스 관리
프로세스는 실행 중인 프로그램을 의미하며, 운영체제는 CPU 시간을 적절히 분배하여 여러 프로세스가 동시에 실행될 수 있도록 관리합니다.

- **프로세스 상태**: 실행, 대기, 종료 등의 상태로 나뉘며, 각 상태 간의 전환을 운영체제가 제어합니다.

### 메모리 관리
운영체제는 메모리를 효율적으로 사용하기 위해 각 프로세스에 메모리를 할당하고, 프로그램이 충돌하지 않도록 메모리 접근을 관리합니다.

- **페이징(Paging)**: 물리적 메모리를 고정된 크기의 페이지로 나누어 관리하는 방식
- **가상 메모리**: 물리적 메모리보다 큰 프로그램을 실행할 수 있도록 지원하는 기술

## 4. 디스크 관리 및 파일 시스템 (슬라이드 4)
디스크는 데이터를 저장하는 장치이며, 운영체제는 파일 시스템을 통해 데이터를 관리합니다.

- **파일 시스템의 역할**: 데이터를 효율적으로 저장하고 검색할 수 있도록 파일을 디렉터리 구조로 관리합니다.
- **주요 파일 시스템**: NTFS, FAT32, ext4 등
- **디스크 관리 도구**: fdisk, mkfs, df, du 등을 사용하여 디스크 파티션, 포맷, 용량 등을 관리합니다.

## 5. 네트워크 설정 및 관리 (슬라이드 5)
### 네트워크 설정 기본
네트워크는 컴퓨터 간의 데이터 전송을 가능하게 하며, 운영체제는 네트워크 인터페이스와 연결을 관리합니다.

- **IP 설정**: 고정 IP 또는 DHCP를 사용하여 네트워크 설정
- **DNS 설정**: 도메인 이름을 IP 주소로 변환하는 서비스
- **방화벽 설정**: 네트워크 트래픽을 제어하여 시스템을 보호하는 기능

## 6. 사용자 및 권한 관리 (슬라이드 6)
운영체제는 여러 사용자가 동일한 시스템을 사용하더라도 서로의 작업에 영향을 주지 않도록 계정과 권한을 관리합니다.

- **사용자 계정 생성 및 삭제**: `useradd`, `userdel` 명령어로 계정을 관리합니다.
- **사용자 권한 관리**: 각 사용자에게 적절한 파일 접근 권한을 설정하여 보안을 유지합니다.

## 7. 시스템 로그 관리 (슬라이드 7)
시스템 로그는 시스템의 상태 및 활동을 기록한 파일입니다. 시스템 로그를 분석하면 시스템의 문제를 파악하고 해결할 수 있습니다.

- **로그 파일 확인**: `/var/log` 디렉터리에서 시스템 로그 파일 확인
- **로그 관리 도구**: `syslog`, `journalctl` 명령어를 사용하여 로그를 관리하고 분석합니다.

## 8. 성능 모니터링 도구 (슬라이드 8)
시스템 성능을 유지하기 위해 운영체제는 다양한 모니터링 도구를 제공합니다.

- **Linux 성능 모니터링**: `top`, `htop`, `vmstat`, `iostat` 등의 명령어로 CPU, 메모리, 디스크 사용량 모니터링
- **Windows 성능 모니터링**: 작업 관리자를 통해 성능을 모니터링하거나, 성능 모니터(perfmon)를 통해 세부 지표를 분석

## 9. 시스템 유지보수 및 업데이트 (슬라이드 9)
시스템 유지보수는 시스템의 안정성과 보안을 유지하기 위해 정기적으로 시스템을 점검하고 업데이트하는 과정입니다.

- **패키지 관리자**: Linux에서는 `apt`, `yum` 등의 패키지 관리자를 사용하여 소프트웨어를 업데이트합니다.
- **보안 업데이트**: 취약점을 방지하기 위해 정기적인 보안 패치 적용

## 10. 문제 해결 및 장애 복구 (슬라이드 10)
운영체제에서 발생하는 다양한 문제를 해결하고, 시스템 장애 시 복구하는 방법을 학습합니다.

- **문제 해결 단계**:
  1. 문제 파악 및 로그 분석
  2. 원인 분석 및 해결 방안 도출
  3. 복구 및 테스트
- **장애 복구**: 백업과 복구 시스템을 통해 데이터 손실을 방지하고 빠른 복구를 실행합니다.


## 추가 학습 자료: YouTube 강의 및 무료 MOOC 강의

시스템 관리 및 운영 개론에 대한 내용을 보완할 수 있도록, 아래와 같은 YouTube 강의와 무료 MOOC 강의를 추천합니다. 이 자료들은 강의에서 다룬 주요 개념들을 심화 학습할 수 있는 좋은 참고 자료입니다.

### YouTube 강의 추천

1. **[Linux System Administration Full Course](https://www.youtube.com/watch?v=UCr04qIB7uc) by The Linux Foundation**  
   [![Linux System Administration Full Course](https://img.youtube.com/vi/UCr04qIB7uc/0.jpg)](https://www.youtube.com/watch?v=UCr04qIB7uc)
   - **설명**: 리눅스 시스템 관리의 모든 기본 개념을 다루는 풀 코스입니다. 운영체제 설정, 사용자 관리, 네트워크 설정 등을 포함합니다.

2. **[Introduction to Linux – Full Course for Beginners](https://www.youtube.com/watch?v=sWbUDq4S6Y8) by freeCodeCamp**  
   [![Introduction to Linux – Full Course](https://img.youtube.com/vi/sWbUDq4S6Y8/0.jpg)](https://www.youtube.com/watch?v=sWbUDq4S6Y8)
   - **설명**: 리눅스 초보자를 위한 강의로, 시스템 관리와 운영의 기본적인 개념을 쉽게 학습할 수 있습니다.

3. **[Free Linux Crash Course with Labs](https://www.freecodecamp.org/news/free-linux-crash-course-with-labs) by freeCodeCamp**  
   [![Free Linux Crash Course with Labs](https://img.youtube.com/vi/0tw8t7wJr-4/0.jpg)](https://www.youtube.com/watch?v=0tw8t7wJr-4)
   - **설명**: 리눅스 시스템 관리에 대한 핵심 개념을 배우고 실습을 통해 이를 적용할 수 있는 강의입니다.

4. **[Linux Tutorial for Beginners: Learn Linux](https://www.youtube.com/watch?v=V8hGKbr7X9c) by Edureka**  
   [![Linux Tutorial for Beginners](https://img.youtube.com/vi/V8hGKbr7X9c/0.jpg)](https://www.youtube.com/watch?v=V8hGKbr7X9c)
   - **설명**: 리눅스 명령어와 운영체제 관리에 대한 기본 개념을 다루는 초보자를 위한 튜토리얼입니다.

5. **[Networking Fundamentals – Full Course](https://www.youtube.com/watch?v=qiQR5rTSshw) by NetworkChuck**  
   [![Networking Fundamentals](https://img.youtube.com/vi/qiQR5rTSshw/0.jpg)](https://www.youtube.com/watch?v=qiQR5rTSshw)
   - **설명**: 네트워크 기초와 TCP/IP, DNS 등 네트워크 관리에 필요한 기본적인 개념을 설명하는 강의입니다.

### 무료 MOOC 강의 추천

1. **[Linux for System Administrators by edX (The Linux Foundation)](https://www.edx.org/course/linuxfoundationx-linux-system-administration)**  
   - **설명**: 리눅스 시스템 관리에 대한 기본 개념부터 고급 관리 기법까지 학습할 수 있는 무료 MOOC 강의입니다. 운영체제의 기초, 네트워크 설정, 서버 관리 등을 학습할 수 있습니다.

2. **[Introduction to Computer Networks and Internet Protocols by Coursera](https://www.coursera.org/learn/computer-networking)**  
   - **설명**: 네트워크의 기본 구조와 TCP/IP 프로토콜을 학습할 수 있는 무료 강의로, 운영체제와의 연관성도 다룹니다.

---

이 자료들은 시스템 관리 및 운영의 핵심 개념을 심화 학습할 수 있는 좋은 참고 자료들입니다. GitHub 강의와 병행하여 활용하면 학습 효과를 극대화할 수 있습니다.

