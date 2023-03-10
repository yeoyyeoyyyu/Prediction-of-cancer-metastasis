# 유방암의 임파선 전이 예측 AI 경진대회

## 개요
림프절(임파선)은 암의 전이에 매우 치명적인 역할을 하기 때문에 림프절 전이 여부와 전이 단계를 파악하는 것이 암을 치료하고 진단하는 것에 있어서 매우 중요
<br>

## 주제
유방암 병리 슬라이드 영상과 임상 항목을 조합하여 유방암의 임파선 전이 여부 이진 분류
<br>

## 데이터
![image](https://user-images.githubusercontent.com/107402707/219846965-05a283c3-b73a-44f5-b865-962f503388f7.png)
<br>


## 모델 구조
1-1.이미지 데이터: ResNet50 모델을 사용하여 피쳐 추출 + fully connected layer <br>
1-2.임상 데이터: 연속형 데이터와 범주형 데이터 각각 인코딩 후 fully connected layer<br>
2.두 임베딩 벡터 concatenate<br>
4.output: 암 전이 여부<br>
![model structure](https://user-images.githubusercontent.com/107402707/223696602-35dfecfc-4331-499d-82c5-5207097fc4ac.png)
<br>

## 평가지표
암 전이가 있는데 없다고 하면 안되기 때문에 재현율 확인<br>
recall = TP / (TP + FN)

## 결과
<br>


#### 출처
[DACON 유방암의 임파선 전이 예측 AI 경진대회](https://dacon.io/competitions/official/236011/overview/description)
