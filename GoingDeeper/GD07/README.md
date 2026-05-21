# AIFFEL Campus Online Code Peer Review Templete
- 코더 : 최수정
- 리뷰어 : 정주열


# PRT(Peer Review Template)
- [x]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
        - mini BERT 모델을 제작했고, 아래와 같이 학습 과정 중에 MLM, NSP loss가 감소하는게 확인되었습니다.
    <img width="1658" height="583" alt="image" src="https://github.com/user-attachments/assets/66d6f7fd-3e55-4f2d-90f9-3815ce111cc8" />

- [x]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 해당 코드 블럭을 왜 핵심적이라고 생각하는지 확인
    - 해당 코드 블럭에 doc string/annotation이 달려 있는지 확인
    - 해당 코드의 기능, 존재 이유, 작동 원리 등을 기술했는지 확인
    - 주석을 보고 코드 이해가 잘 되었는지 확인
        - 데이터 전처리 하는것(MASK, NSP pair)이 BERT 모델의 핵심 부분 중 하나라고 생각하는데 아래와 같이 몇 퍼센트 비율로 나누어서 데이터를 전처리 했는지 잘 표기 되어 있어서 이해하기 쉬웠습니다.
    <img width="907" height="521" alt="image" src="https://github.com/user-attachments/assets/4d4c4ec5-3b6b-4f2d-b376-d2747f1e6fb8" />

- [x]  **3. 에러가 난 부분을 디버깅하여 문제를 해결한 기록을 남겼거나
새로운 시도 또는 추가 실험을 수행해봤나요?**
    - 문제 원인 및 해결 과정을 잘 기록하였는지 확인
    - 프로젝트 평가 기준에 더해 추가적으로 수행한 나만의 시도, 
    실험이 기록되어 있는지 확인
        - 10 epoch으로 학습을 완료했다가 아래 사진과 같이 결과를 확인하고 문제를 분석해서 50 epoch 더 학습해서 더 좋은 결과를 냈습니다.
    <img width="567" height="511" alt="image" src="https://github.com/user-attachments/assets/c5b81f0b-9e19-45b7-808a-8988cb3a0e75" />
    <img width="510" height="689" alt="image" src="https://github.com/user-attachments/assets/28840ab1-436c-443f-8914-5f3f8ca6cdef" />


- [x]  **4. 회고를 잘 작성했나요?**
    - 주어진 문제를 해결하는 완성된 코드 내지 프로젝트 결과물에 대해
    배운점과 아쉬운점, 느낀점 등이 기록되어 있는지 확인
    - 전체 코드 실행 플로우를 그래프로 그려서 이해를 돕고 있는지 확인
        - 이 프로젝트에서 주어진 테스크를 완료하였고, Ablation study까지 어느정도 진행한 부분과 시간 관계상 수행하지 못한 부분에 대해서 회고한 내용이 잘 작성되어 있습니다.
    <img width="1802" height="355" alt="image" src="https://github.com/user-attachments/assets/cc503efe-e9d2-4d73-953c-010e5cc08f21" />

- [x]  **5. 코드가 간결하고 효율적인가요?**
    - 파이썬 스타일 가이드 (PEP8) 를 준수하였는지 확인
    - 코드 중복을 최소화하고 범용적으로 사용할 수 있도록 함수화/모듈화했는지 확인
        - 코드가 함수화/모듈화가 잘되어 있습니다. 특히 BERT 모델 생성 부분에서 주석 설명과 함께 각각 함수의 역할이 무엇인지 설명이 잘 되어 있습니다.
    <img width="639" height="774" alt="image" src="https://github.com/user-attachments/assets/1b8edf06-acf0-49be-b651-96de89502f7a" />


# 회고(참고 링크 및 코드 개선)
BERT pretrained model 제작 프로젝트에서 루브릭을 다 잘 지켜가면서 완수하신 것 같습니다. 또한 결과를 넘어서 Ablation study까지 하신 것은 대단한 것 같습니다. 또한 Ablation study에서 결과 그래프로 보여주신 것은 정말 좋았던것 같습니다. 참고해서 저도 좋은 성능이 나온 방법을 구현해보겠습니다. 많이 배워갑니다!
