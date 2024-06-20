### 코더 회고
배운 점: 트랜스포머 구조에 대해서 확실히 이해할 수 있었다. 각 모듈이 어디에, 왜, 어떻게 있어야 하는 지를 배웠다

아쉬운 점: 데이터셋을 보니 맞춤법이 안 맞는 문장도 있었고, 최종 추론에서 같은 단어라도 맞춤법에 따라 다른 답을 내놓는 것을 확인해서 맞춤법 관련 전처리도 함께 수행해보고 싶었는데 시간이 부족했다

어려운 점: tf.data.Dataset API에 대한 이해가 부족해 validation dataset을 적용할 때 어려움이 있었다. 배치가 이미 적용된 데이터셋에 대해 배치 적용 이전 크기를 기준으로 나누려고 해서 문제가 발생했다. 배치 적용 전 train과 validation으로 나누고 배치를 적용하니 문제를 해결할 수 있었다

느낀 점: 트랜스포머에 대해 공부한 게 이번이 처음이 아닌데 이제야 어느 정도 알 것 같다. 

---
🔑 **PRT(Peer Review Template)**

- [X]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요? (완성도)**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 
    퀘스트 문제 요구조건 등을 지칭
        - 해당 조건을 만족하는 부분의 코드 및 결과물을 캡쳐하여 사진으로 첨부
          1. 공백과 특수문자 처리, 토크나이징, 병렬데이터 구축의 과정이 적절히 진행되었다.<br>
             ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/0abf8a0f-d434-49bd-8cbe-92c8533779a3)<br>

          2. 구현한 트랜스포머 모델이 한국어 병렬 데이터 학습 시 안정적으로 수렴하였다.<br>
             ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/18fe4043-6ac2-4089-97af-06c61e3e89d3)<br>

          4. 한국어 입력문장에 대해 한국어로 답변하는 함수를 구현하였다.	한국어 입력문장에 맥락에 맞는 한국어로 답변을 리턴하였다.<br>
        ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/ce9b720e-790c-47a2-9dc0-cedc805344fa)


- [X]  **2. 프로젝트에서 핵심적인 부분에 대한 설명이 주석(닥스트링) 및 마크다운 형태로 잘 기록되어있나요? (설명)**
    - []  모델 선정 이유 
    - []  Metrics 선정 이유  
    - []  Loss 선정 이유
    - 모델 선정 이유나 Metrics 선정이유, Loss 선정 이유는 없었지만 하면서 궁금했던 점에 대해서 주석을 달아놓거나<br>
    ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/909a5f00-2ec5-4091-acd2-e9b6af370a74)<br>
      중요부분에 주석을 달아주셨습니다.<br>
      ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/19633cbb-2242-4a03-8a05-1e8e53c3523f) <br>

    


- [X]  **3. 체크리스트에 해당하는 항목들을 모두 수행하였나요? (문제 해결)**
    - [X]  데이터를 분할하여 프로젝트를 진행했나요? (train, validation, test 데이터로 구분)<br>
    ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/d75f3ca3-dd81-4482-9f48-d93d98dd5d6a)<br>
    - [X]  하이퍼파라미터를 변경해가며 여러 시도를 했나요? (learning rate, dropout rate, unit, batch size, epoch 등)<br>
    ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/36978daf-5505-4cf8-b2d5-44755576ccb3)<br>
    ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/07b6f482-0488-4247-b76b-f7a802ac2350)<br>
    ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/72115c07-f4c3-42a6-b209-1d266184e1f9)<br>
    ![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/286bb8fd-2832-4e18-9049-2267c381cf86)<br>
너무 잘 해주셨습니다.

    - [X]  각 실험을 시각화하여 비교하였나요?  
![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/f0407fe6-c32b-4f0c-a023-308d47e04459)<br>
![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/693a22be-ebff-4a57-a6de-c30088291401)<br>
![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/d1cd2fcd-0cab-4c7b-8943-11d048bb13c5)<br>
![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/df1ae92c-95a5-4b7c-bc90-a4afc60e4f65)<br>
![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/33b8e2a0-1fb6-4b7e-93bd-1bdc69fccfa1)<br>
너무 잘해주셨습니다.


_______________________________________________________________________________________________________
리뷰어의 느낀점:
전처리시 숫자를 전부다 한글처리한 것도 인상적이었습니다. 또한 모델에서 더 많은 레이어와 다양한 하이퍼파라미터를 사용하여 실험하시는 것도 매우 인상적이었습니다. 실험하시는 방법을 보고 저도 앞으로 어떤식으로 다양하게 실험할 수 있을지를 깨달았던 것 같습니다.


    - [X]  모든 실험 결과가 기록되었나요?
        <br>위의 스크린샷들을 보면 결과가 잘 기록되어있는 것을 알 수 있습니다.
 
- [X]  **4. 프로젝트에 대한 회고가 상세히 기록 되어 있나요? (회고, 정리)**
    - [X]  배운 점
    - [X]  아쉬운 점
    - [X]  느낀 점
    - [X]  어려웠던 점
![image](https://github.com/4rldur0/AIFFEL-Quest/assets/104029654/2e697885-cc0d-41ba-a985-6548d9eaa705)
