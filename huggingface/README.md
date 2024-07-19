### 코더 회고
- 배운 점: huggingface transformers를 활용하여 pretrained 모델을 불러오고 fine-tuning하는 법을 배웠다
- 아쉬운 점: 학습 시간이 너무 길어 전처리에 대한 실험을 해보지 못 했다
- 어려운 점: 다른 노트북에서 wandb를 사용하고 현재 노트북에서는 wandb를 import하지 않았는데도 wandb가 쓰였다. 그 이유를 조금 더 찾아보고 싶다
- 느낀 점: 실제로 많이 쓰이는 부분을 배워서 좋다

### 실험 결과
1. 기존 하이퍼파라미터
    ```
    training_arguments = TrainingArguments(
    output_dir,                             # output이 저장될 경로
    evaluation_strategy="steps",           #evaluation하는 빈도
    eval_steps=1000,  # 1000 스텝마다 평가 수행
    learning_rate = 2e-5,                         #learning_rate
    per_device_train_batch_size = 8,   # 각 device 당 batch size (내부적으로 DataLoader를 사용하여 지정된 배치 크기로 데이터를 로드)
    per_device_eval_batch_size = 8,    # evaluation 시에 batch size
    num_train_epochs = 1,                     # train 시킬 총 epochs
    weight_decay = 0.01,                        # weight decay
    )
    ```
   ![image](https://github.com/user-attachments/assets/a008c2ea-bf98-4021-9507-f6d046924d5c)

2. 학습률 5e-5로 변경
   ![image](https://github.com/user-attachments/assets/12c426c7-1204-49bc-ae3e-da0842033d35)
   - 약간 향상됨
3. wandb 활용하여 random search
   ![image](https://github.com/user-attachments/assets/14fd4028-7d07-4a01-9eec-8cf7f3022b3d)

4. 2에서 data collator와 group_by length 옵션 추가
   ![image](https://github.com/user-attachments/assets/9b6bc79e-83cb-4529-aff1-d2aefb8eea8e)
   ![image](https://github.com/user-attachments/assets/61741bf1-5088-4924-b375-c451452802ed)

---
🔑 **PRT(Peer Review Template)**
리뷰어: 

- [x]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요? (완성도)**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 
    퀘스트 문제 요구조건 등을 지칭
        - 해당 조건을 만족하는 부분의 코드 및 결과물을 캡쳐하여 사진으로 첨부
        1. 모델과 데이터를 정상적으로 불러오고, 작동하는 것을 확인하였다.
        2. Preprocessing을 개선하고, fine-tuning을 통해 모델의 성능을 개선시켰다.
        3. 모델 학습에 Bucketing을 성공적으로 적용하고, 그 결과를 비교분석하였다.


- [x]  **2. 프로젝트에서 핵심적인 부분에 대한 설명이 주석(닥스트링) 및 마크다운 형태로 잘 기록되어있나요? (설명)**
    - [x]  모델 선정 이유

    - [x]  Metrics 선정 이유

    - [x]  Loss 선정 이유

    - 하면서 궁금했던 점에 대해서 주석을 달아놓거나   


- [x]  **3. 체크리스트에 해당하는 항목들을 모두 수행하였나요? (문제 해결)**
    - [x]  데이터를 분할하여 프로젝트를 진행했나요? (train, validation, test 데이터로 구분)
    - [x]  하이퍼파라미터를 변경해가며 여러 시도를 했나요? (learning rate, dropout rate, unit, batch size, epoch 등)
    - [x]  각 실험을 시각화하여 비교하였나요?
    - [x]  모든 실험 결과가 기록되었나요?

- [x]  **4. 프로젝트에 대한 회고가 상세히 기록 되어 있나요? (회고, 정리)**
    - [x]  배운 점
    - [x]  아쉬운 점
    - [x]  느낀 점
    - [x]  어려웠던 점
