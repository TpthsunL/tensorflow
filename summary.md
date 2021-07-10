용어정리¶
epoch : 전체 데이터가 모두 학습한 단위

ex) 60,000개의 데이터가 모두 학습되었다면 -> 1epoch
30epoch = 60,000개의 데이터에 대하여 30번 학습하겠다는 의미

loss : 정답 값과의 오차 (loss는 낮을 수록 좋음)

Accuracy(acc) : 정확도

supervised Learning(지도학습)

입력 데이터&출력데이터가 존재 (<-> 비지도학습은 입력 데이터만 존재함)
분류와 회귀로 나뉨.
회귀 : 연속된 수치를 가지고 논다.
==tesorflow문제에서는 1,5번 문제가 회귀, 2,3,4 문제가 분류==

input/Output, Features/Labels
여기서는 인풋과 아웃풋 데이터라고 얘기 안할 것이다!!
인풋데이터 : x, Features
아웃풋 데이터 : y, Labels
batch / batch size
보통 학습을 할 때, node에 있는 weight들을 업데이트 시키면서 학습을 한다.
이때 기준은, 1 epoch이 끝날때, 되는게 아니라 batch가 끝날때 시행된다고 볼 수 있다.
bath란? 1개의 epoch에서 여러 개의 샘플을 나누어 학습하는 단위이다.*
bathsize는 몇개로 묶을지, batch 묶은개 몇개?

1000개의 이미지를 학습하는 경우,

batch_size = 10 => (1000개의 이미지)/(batch_size=10) = 총 100개의 batch
batch_size = 20 => (1000개의 이미지)/(batch_size=20) = 총 50개의 batch
** 따라서 batch size를 어떻게 설정하느냐에 따라서 가중치의 횟수를 정한다.**
