#### 코더 회고
배운 점
- 추상적 요약과 추출적 요약의 차이점에 대해 잘 알 수 있었다

아쉬운 점, 어려웠던 점
- 학습을 돌려놓는 시간이 너무 길어 실험을 다양하게 해보지 못 한 게 아쉽다. news 데이터셋에서 summa 요약기가 자꾸 빈 결과를 내놓는 이유를 찾느라 시간이 조금 걸렸다

느낀 점
- 실제 생활에 적용될 수 있다고 느껴져 평소보다 더 즐겁게 할 수 있었다

---
### (리뷰어:이종무)
🔑 **PRT(Peer Review Template)**

- [O]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요? (완성도)**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 
    퀘스트 문제 요구조건 등을 지칭
        - 해당 조건을 만족하는 부분의 코드 및 결과물을 캡쳐하여 사진으로 첨부
          ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/169742259/98720dbb-6c97-43bd-a1be-4a782afda0ba)
          ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/169742259/0640a875-31f5-4d63-a59b-80a60c64a174)
          ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/169742259/bb0dba09-4ef3-42f6-9047-d450d606aed4)


- [Yes]  **2. 프로젝트에서 핵심적인 부분에 대한 설명이 주석(닥스트링) 및 마크다운 형태로 잘 기록되어있나요? (설명)**
    - [O]  모델 선정 이유
        - 기존의 seq2seq 모델의 단점인 기울기 소실을 보완하기 위해 attention을 추가해 보완해 사용해주셨습니다👍
          ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/169742259/2556c447-2295-4c47-a74c-78042e367d8e)
    - [O]  Metrics 선정 이유
        - 기존 rmsprop 보다 adam의 성능이 훨씬 좋았다는 연구를 발견해 적용하여 adam을 선택하셨습니다!
    - [O]  Loss 선정 이유
          ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/169742259/eb91c411-591d-4672-a7c8-4e405f597c7a)
      

- [Yes]  **3. 체크리스트에 해당하는 항목들을 모두 수행하였나요? (문제 해결)**
    - [O]  데이터를 분할하여 프로젝트를 진행했나요? (train, validation, test 데이터로 구분)
          ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/169742259/45c60ce2-efe0-425b-83da-fb876bd397a6)
    - [O]  하이퍼파라미터를 변경해가며 여러 시도를 했나요? (learning rate, dropout rate, unit, batch size, epoch 등)
          ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/169742259/6b64541a-2e13-490f-97e2-2ee27672ce30)
    - [Yes]  각 실험을 시각화하여 비교하였나요?
          ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/169742259/ab79e035-cc8b-4c50-8d36-8f87d8b6579e)
    - [Yes]  모든 실험 결과가 기록되었나요?
          ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/169742259/20219f79-ba79-4632-84e9-7890c813363c)





- [O]  **4. 프로젝트에 대한 회고가 상세히 기록 되어 있나요? (회고, 정리)**
    - [O]  배운 점
    - [O]  아쉬운 점
    - [O]  느낀 점
    - [O]  어려웠던 점
    - 구제적인 문제상황을 정의하고 해결하려고 시도하신 부분이 많이 인상깊었습니다💯

