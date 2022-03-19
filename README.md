# NLP_Practice
<<<<<<< HEAD

VS코드와 Git을 이용한 자연어처리 연습

되도록이면 VS코드에서 연습하되 필요하면 Colab에서 활용

**22.03.19 작업 기록**

1) kkma에서 사용하는 환경인 jvm에서 기본적으로 

힙(Heap) 메모리를 얼마나 줬는지 모르겠지만 중간에 터져버리는 일 발생

검색해본 결과 init_jvm()에 인자값으로 메모리 할당량을 주고 실행하면 해결되는것으로 보임

2) 팀 회의간 결과 원본 데이터셋에서 3만개 정도로 쪼개자고 해서 샘플링 후 진행했으나

비교를 위한 원본 모델인 LSTM에서 에러가 발생했고

그 원인으로 대다일 관계가 성립하기 어려운 상태(X가 Y보다 적음)로 추정됨

**1차 시도**로 원본 데이터(Train)를 5만으로 샘플링 후 해보고

그 이후에도 깨진다 싶으면 그냥 원본으로 진행


**22.03.20 작업 기록(오전)**
1차 시도 (데이터를 15만에서 5만개 샘플링)

결과 : 실패

애초에 비율을 3:1로 조정해놓은걸 임의로 샘플링해서 생긴 문제이므로

두가지 해결책 마련

1) 그냥 원본으로 가기 = 15만 : 5만의 3대 1 비율로 정상적으로 가동할 것으로 예상

2) 테스트 데이터도 샘플링 : 3만 : 1만으로 3대 1비율 유지 및 가동 가능성 있음. 
**정확도 떨어질 것으로 예상**
=======
자연어처리 연습

필요하면 Colab에서 활용
>>>>>>> 482a3654aa2448839e4c82b40e9f424887f57884
