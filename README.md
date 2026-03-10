# 📌 레드와인, 화이트와인 분류 머신러닝

## 1. 문제 정의
- 와인은 산도, 당도, 알코올 함량 등 다양한 화학적 성분에 의해 특징이 구분된다. 본 프로젝트에서는 이러한 와인의 화학적 특성 데이터를 활용해 해당 와인이 레드와인인지, 화이트와인인지 분류하는 머신러닝 모델을 구축하는 것을 목표로한다.<br>
## 2. 데이터
- Kaggle Wine Quality Dataset<br>
type: 레드와인인지 화이트 와인인지 구별<br>
fixed acidity: 고정산도<br>
volatile acidity: 휘발성 산도<br>
citric acid: 시트르산(구연산)<br>
residual sugar: 잔여당분<br>
chlorides: 염화물<br>
free sulfur dioxide: 자유 이산화황<br>
total sulfur dioxide: 총 이산화황<br>
density: 밀도<br>
pH: 산성도<br>
sulphates: 황산염<br>
alcohol: 알코올도수<br>
quality: 등급<br>

## 3. 분석 과정
1. 데이터 이해
   - 데이터 구조와 각 변수의 특성 파악
     * 데이터 컬럼 확인
     * 수치형 변수 요약통계 확인
     * 데이터 분포 및 기본 통계 분석
2. 데이터 전처리
   - 결측치 확인 및 제거
   - 중복 데이터 제거
   - 범주형 변수 인코딩(와인타입 변수)
     * 화이트 0, 레드 1
3. 모델 학습
   - 데이터의 비선형 관계 학습과 변수 중요도를 통해 어떤 화학 특성이 분류에 중요한지 해석가능한 **Decision Tree** 사용
   - 모델 학습 및 평가
     * 직접 계산한 정확도, sklearn 함수, 모델 score를 비교하여 결과를 확인함
## 4. 결과
- 약 97.9%의 정확도를 보였다.
- 와인의 화학적 특성이 와인을 구분하는데 유의미한 정보를 제공한다는 것을 알 수 있었다.

## 5. 사용기술
- Python, Pandas, Matplotlib, seaborn, scikit-learn(train_test_split, DecisionTreeClassifier, accracu_score, classification_report)
