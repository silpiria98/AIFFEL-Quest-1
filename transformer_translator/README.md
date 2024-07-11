### 코더 회고
배운 점: 트랜스포머 구현 코드에 대해 더 잘 이해하게 되었다

아쉬운 점: masking 부분을 수정하느라 실제 추론 부분을 잘 확인하지 못해서 아쉽다. 

어려운 점: 노드의 정답 코드에서 masking이 잘못 정의된 것 같아 수정했는데 shape을 맞추고 학습이 되도록 알맞게 수정하는 게 어려웠다. 한가지 궁금한 점은 원래의 노드 코드로 해도 정상적으로 작동하는데, 그 이유가 궁금하다

느낀 점: 지난 번 트랜스포머로 챗봇을 만들었을 때보다 더 세세한 부분에 집중할 수 있었다

---
### 리뷰어
🔑 **PRT(Peer Review Template)**

- [x]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요? (완성도)**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 
    퀘스트 문제 요구조건 등을 지칭
        - 해당 조건을 만족하는 부분의 코드 및 결과물을 캡쳐하여 사진으로 첨부
          <img width="904" alt="스크린샷 2024-07-11 오후 5 13 07" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/10970657-64ae-4a4c-86f9-51b35cdae2f4">
          <img width="903" alt="스크린샷 2024-07-11 오후 5 14 03" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/14d7a3a6-4d52-48d3-9c28-6a4de2b1cdad">
          <img width="900" alt="스크린샷 2024-07-11 오후 5 14 39" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/c9ade1a7-7e69-4aa2-a9e7-34af73aace57">


- [x]  **2. 프로젝트에서 핵심적인 부분에 대한 설명이 주석(닥스트링) 및 마크다운 형태로 잘 기록되어있나요? (설명)**
    - [x]  모델 선정 이유
    - [x]  Metrics 선정 이유
    - [x]  Loss 선정 이유
    - 하면서 궁금했던 점에 대해서 주석을 달아놓거나
      <img width="866" alt="스크린샷 2024-07-11 오후 5 19 36" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/ca771971-eb87-4b15-9460-3586c61ed56a">  
      <img width="866" alt="스크린샷 2024-07-11 오후 5 19 11" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/213e68d4-c564-48bc-89ac-bae31ec087b9">  
      <img width="873" alt="스크린샷 2024-07-11 오후 5 15 27" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/3eea34db-6192-4e8d-8088-4403fd3c4009">  
      실험을 진행하면서 주석을 잘 작성하였음.


- [x]  **3. 체크리스트에 해당하는 항목들을 모두 수행하였나요? (문제 해결)**
    - [x]  데이터를 분할하여 프로젝트를 진행했나요? (train, validation, test 데이터로 구분)<br>
    - [x]  하이퍼파라미터를 변경해가며 여러 시도를 했나요? (learning rate, dropout rate, unit, batch size, epoch 등)<br>
    - [x]  각 실험을 시각화하여 비교하였나요?
      <img width="900" alt="스크린샷 2024-07-11 오후 5 21 24" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/16298df7-d79e-4847-94f4-cda1e32ab0f9">
      <img width="905" alt="스크린샷 2024-07-11 오후 5 22 36" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/5216cdd1-96b3-4510-9132-5d58012a1a76">  
      ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/aa0943fc-3051-443f-8927-ccab7c10b8dd)

 
- [x]  **4. 프로젝트에 대한 회고가 상세히 기록 되어 있나요? (회고, 정리)**
    - [x]  배운 점
    - [x]  아쉬운 점
    - [x]  느낀 점
    - [x]  어려웠던 점
      <img width="1028" alt="스크린샷 2024-07-11 오후 5 24 10" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/5573111b-946c-4a4c-af6e-7f4eb3ce377e">  

코더: 김나경  
리뷰어: 이정희
