# Disk, Partition and Volume

## Disk

- 컴퓨터나 서버에 장착되어 블록 단위 저장 공간을 제공하는 저장 장치
- 원래는 HDD만을 가리켰으나, 저장 매체가 다양해지면서 SSD(SATA·NVMe), 플래시 기반 스토리지(eMMC, UFS 등) USB 플래스 드라이브·SD 카드, RAM 디스크, 가상 디스크나 클라우드 블록 스토리지도 넓은 의미의 디스크로 부름

HDD

- 하드디스크 드라이브
- 자기 Platter를 회전시키고 Head와 Arm으로 데이터를 읽고 쓰는 저장 장치

## Partition

- 하나의 물리 디스크를 논리적으로 쪼갠 구획으로, OS는 각 파티션을 독립된 블록 디바이스로 인식해 별도 디스크처럼 취급하며 각자 다른 파일 시스템을 설치할 수 있음
- 순수 파티션은 디스크 안에서 연속적인 공간이어야 함

Primary Partition (주 파티션)

- MBR 디스크에서 최대 4개 생성이 가능하며, 그 이상의 파티션이 필요할 경우 확장/논리 추가
  - 4개의 주 파티션 혹은 3개의 주 파티션과 하나의 확장 파티션을 가질 수 있음
- GPT 디스크에서 4개 이상의 주 파티션을 만들 수 있음

Extended Partition (확장 파티션)

- 논리 파티션을 담는 컨테이너 역할로, 주 파티션 중 1개만 지정 가능
- 파일 시스템 탑재 불가 (직접 포맷·마운트 불가)

Logical Partition (논리 파티션)

- 확장 파티션 내 N개 생성해 실제 데이터 저장
- 주 파티션과 다르게 OS 부팅이 불가하나 파일 시스템 탑재 가능

## Volume

- 하나의 파일 시스템이 차지하는 논리적 저장 공간
- OS가 이를 하나의 드라이브/마운트 지점으로 취급
- 볼륨은 연속될 수도 있고, 여러 파티션·디스크를 묶은 비연속 공간일 수도 있음
  - 파티션은 물리 디스크 내부의 연속 블록 범위
- 일반적으로 디스크를 파티션으로 구분하고, 각 파티션을 파일 시스템으로 포맷하여 볼륨을 만들어 사용

## 출처

[디스크, 파티션, 볼륨이란?(feat. 볼륨이 뭔데?)](https://orange-makiyato.tistory.com/95)

[[File System] Partition VS Volume](https://hyd3.tistory.com/122)

[[OS] 디스크(Disk) /파티션(Partition) / 볼륨(Volum) / 파일시스템 용어정리](https://pearlluck.tistory.com/179)

[[Digital Forensic] 볼륨과 파티션](https://yum-history.tistory.com/223)

[파티션과 볼륨이 뭐냐면](https://velog.io/@kirisame/%ED%8C%8C%ED%8B%B0%EC%85%98%EA%B3%BC-%EB%B3%BC%EB%A5%A8%EC%9D%B4-%EB%AD%90%EB%83%90%EB%A9%B4)
