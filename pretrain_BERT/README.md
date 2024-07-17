### 코더 회고
- 배운 점: BERT 모델의 사전학습 프로세스를 배웠다
- 아쉬운 점: 학습을 한 번 돌릴때마다 30분 가량이 소요되어 많은 실험을 해보지 못 했다
- 어려운 점: 모델 자체의 코드에 대한 이해가 부족하다
- 느낀 점: memmap 이외의 데이터의 크기가 클 때 사용할 수 있는 기법에 대해 더 알아보고 싶다 

---
🔑 **PRT(Peer Review Template)**
리뷰어: 김서우

- [O]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요? (완성도)**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 
    퀘스트 문제 요구조건 등을 지칭
        - 해당 조건을 만족하는 부분의 코드 및 결과물을 캡쳐하여 사진으로 첨부
    1. 한글 코퍼스를 가공하여 BERT pretrain용 데이터셋을 잘 생성하였다.
           마스킹 생성, NSP 잘 적용해서 데이터셋을 만들었습니다.   
           ![image](https://github.com/user-attachments/assets/6352cb18-6860-4d1d-8fca-90d419fd68fb)   
           ![image](https://github.com/user-attachments/assets/4dfbf5fb-ed69-406b-8687-9ec687f99c40)
       
    2. 구현한 BERT 모델의 학습이 안정적으로 진행됨을 확인하였다 + 1M짜리 mini BERT 모델의 제작과 학습이 정상적으로 진행되었다.
           ![image](https://github.com/user-attachments/assets/346c6e06-7101-4411-b540-79535b50d9df)
           ![image](https://github.com/user-attachments/assets/510bb63a-bc52-467d-bc3a-fa818bd0c026)
           모델 제작과 학습 결과 시각화까지 모두 잘 진행하셨습니다. 


- [O]  **2. 프로젝트에서 핵심적인 부분에 대한 설명이 주석(닥스트링) 및 마크다운 형태로 잘 기록되어있나요? (설명)**
    - [O]  모델 선정 이유
          ![image](https://github.com/user-attachments/assets/cad0e22b-ca6c-4a33-8155-5d3993a2afaa)

    - [O]  Metrics 선정 이유
         ![image](https://github.com/user-attachments/assets/0768b82f-d176-40d8-92a9-244e5aad27c9)

    - [O]  Loss 선정 이유
        ![image](https://github.com/user-attachments/assets/3c5c77a5-1ca8-4da0-a8e4-fcd45997b78c)

    - 하면서 궁금했던 점에 대해서 주석을 달아놓거나   
        ![image](https://github.com/user-attachments/assets/f9fb9780-cc2f-4daf-874b-6626b5ae6ee1)


- [O]  **3. 체크리스트에 해당하는 항목들을 모두 수행하였나요? (문제 해결)**
    - [O]  각 실험을 시각화하여 비교하였나요?  
    - [O]  모든 실험 결과가 기록되었나요?
          - 1-2 와 내용이 같아 따로 첨부하지 않겠습니다. 모두 잘 기록되어 있습니다. 

- [O]  **4. 프로젝트에 대한 회고가 상세히 기록 되어 있나요? (회고, 정리)**
    - [O]  배운 점
    - [O]  아쉬운 점
    - [O]  느낀 점
    - [O]  어려웠던 점
    - **해당 마크다운 윗부분에 잘 기록되어 있습니다.**
