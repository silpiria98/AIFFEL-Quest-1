
        - (2조 C2 신뢰) Classification - data type 1
            - 레이어 개수 늘어날수록 수렴 속도가 빨라짐
        - (4조 C4 이끔) Classification - data type 4
            - 입력층 vs 입력 뉴런 개수 
                → layer 2개 부터는 비슷한 표현 효과  
        - (1+5조 C1 상생) Regression - data type 2
            - 피처를 1개만 사용하거나 x1과 x1^2을 같이 사용했을 때 안 좋았음
            - 모델이 복잡할수록 더 큰 lr을 쓰는 게 나음. 현재 모델에서는 0.01이 최적값
        - (8조 부스2) Image Data : Layer 의 너비가 달라지는 경우
            - layer 너비가 늘어날수록 가장 좋은 성능, 빠른 수. 과적합의 우려 큼
        - (7조 부스1) Image Data : Layer의 구성이 달라지는 경우 1
            - 레이어 모듈에 변화가 있는 경우
            - Conv - Maxpool // Conv - Conv - Maxpool
                - conv 2개를 쓰면 첫번째 conv에서는 단순한 패턴, 두번째 conv에서는 복잡한 패턴을 학습할 수 있
        - (6조 M2 공유) Image Data :Layer의 구성이 달라지는 경우 2
            - 레이어 깊이에 변화가 있는 경우
            - Conv-maxpool을 한번 반복하는 경우 // Conv-maxpool을 여러 번 반복하는 경우
                - dense layer: 전체적인 특성을 봄/이미지 데이터: 지엽적인 특징이 있음
