# LAB_Project
## LAB실 개인과제(쿠버네티스를 이용한 네트워크 플로우 수집 및 데이터 활용)

### 1. 쿠버네티스(k8s) 환경 구성: Master(8g,40g) + worker1(8g,40g) + worker2(8g,40g), CNI: Cilium, Openstack, Ubuntu 22.04 //완성

### 2. Cilium Hubble 설정 및 Hubble Observe 명령어를 사용해서 MongoDB에 Network Flow 데이터 수집 및 singe layer 데이터로 변환(30s 에 한번씩) //완성(gRPC, Protobuf 추가 공부 필요)

### 3. 수집된 데이터를 Anomaly Detection에 맞게 선별 및 가공 MongoDB로 연결 및 스트리밍 // 어느정도 완성(기능적으로 동작은 되나 오버헤드가 있음)

### 4. tensorflow를 사용해서 네트워크 이상 데이터 실시간 학습 및 판별 가능 // 어느정도 완성(기능적으로 동작은 되나 오버헤드가 있음), One-Hot Encoder, Isolation Forest

### 5. n개의 데이터를 실시간 학습 시키면서 데이터가 쌓일때 마다 오래된 m개의 데이터를 삭제시키고 m개의 데이터를 추가 해서 슬라이딩 윈도우를 사용해서 학습하는 방법으로 변경 //완성

### 6. collection.watch() 대신 kafka 적용 및 이상탐지 모델 테스트 방법 고민 //진행중

