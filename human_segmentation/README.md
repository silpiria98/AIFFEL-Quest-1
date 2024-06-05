### 코더 회고
배운 점: 이미지 세그멘테이션에 대해 자세히 알아볼 수 있었고, 실제 어플리케이션에 어떻게 적용되는지 배울 수 있었다.

아쉬운 점: 가느다란 물체에 대해 정확도를 향상시키는 방법을 찾고 싶었는데 찾지 못해 아쉽다

어려운 점: 검색하면 학습 단계에서 성능을 향상 시키는 내용이 대부분이라 해결책을 생각해내는 것이 꽤 어려웠다. 

느낀 점: 어렵긴 했지만 직접 해결책을 생각해내고, 실험으로 그것이 증명되었을 때 매우 뿌듯했다


---
🔑 **PRT(Peer Review Template)**

- [x]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요? (완성도)**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 
    퀘스트 문제 요구조건 등을 지칭
        - 해당 조건을 만족하는 부분의 코드 및 결과물을 캡쳐하여 사진으로 첨부
    <img width="986" alt="image" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/63a9a533-15bd-44d0-8ba3-def534aaa17b"><br>
    <img width="986" alt="image" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/74ef5316-50b1-4c02-9567-62ce1c01f05a"><br>
    3장 이상의 사진에 블러, 크로마키를 처리하였음.<br>
    다양한 해결 방법이 작성되어 있음.<br>

- [x]  **2. 프로젝트에서 핵심적인 부분에 대한 설명이 주석(닥스트링) 및 마크다운 형태로 잘 기록되어있나요? (설명)**
    - [x]  ~~모델 선정 이유~~  
    - [x]  ~~Metrics 선정 이유~~  
    - [x]  ~~Loss 선정 이유~~  
    <img width="688" alt="image" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/6ea2cf8c-06f2-4630-a4c3-ac143d50f7db"><br>
    프로젝트 전체에 걸쳐서 설명이 잘 기록되어 있음.<br>

- [x]  **3. 체크리스트에 해당하는 항목들을 모두 수행하였나요? (문제 해결)**
    - [x]  ~~데이터를 분할하여 프로젝트를 진행했나요? (train, validation, test 데이터로 구분)~~  
    - [x]  ~~하이퍼파라미터를 변경해가며 여러 시도를 했나요? (learning rate, dropout rate, unit, batch size, epoch 등)~~  
    - [x]  각 실험을 시각화하여 비교하였나요?  
    - [x]  모든 실험 결과가 기록되었나요?
    <img width="910" alt="image" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/db83fb15-9a2f-4085-994c-51d01772676a"><br>
    각 실험에 대해 시각화가 되었고, 실혐 결과가 기록되어 있음.

- [x]  **4. 프로젝트에 대한 회고가 상세히 기록 되어 있나요? (회고, 정리)**
    - [x]  배운 점
    - [x]  아쉬운 점
    - [x]  느낀 점
    - [x]  어려웠던 점
    <img width="662" alt="image" src="https://github.com/4rldur0/AIFFEL-Quest/assets/82493052/f467ef6a-f76d-48d9-ab14-2b05de834978">
---
### 리뷰어 회고
#### instance segmentation
해결 방법에 instance segmentation을 활용에 대한 내용이 있었음. 생각하지 못 했던 부분이라 많은 것을 배울 수 있었음.<br>
instance segmentation을 이용하면 어떤 객체에 관심이 있는지 annotation이 있어야 함. 해당 문제는 가장 큰 객체 외엔 모두 0인 mask를 만드는 방법 등을 활용할 수 있을 것같음.<br>
#### 함수 생성
코드 리뷰 중 blurring_kernel_size, 배경 crop 등의 이슈로 함수를 생성하지 않고, 하나씩 적용하였다고 말씀하셨음.<br>
함수로 생성한다면 blurring_kernel_size는 이미지의 크기에 비례해서 설정할 수 있을 것같음.<br>
```python
# 수두코드
blur_ksize = img_orig.shape[0] // 2000 , img_orig.shape[0] // 2000<br>
```
<br>
배경 crop은 deeplab v3 모델을 이용해서, 이미지의 y축을 행으로 두면서 background가 아닌 id가 행에 포함되는지 확인<br>
background가 아닌 id가 포함된다면 break 후 윗 부분을 crop하면 함수로 작성할 수 있을 것같음.
