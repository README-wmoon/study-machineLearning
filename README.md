### AI (Artificial Intelligence)
<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/cfb98ea9-3979-4d80-84a3-bbf94df39efa" width="800px">

#### Rule-base AI
- 특정 상황을 이해하는 전문가가 직접 입력값(문제)과 특징을 전달(규칙)하여 출력값(정답)을 내보내는 알고리즘이다.
- 광범위한 데이터 수집, 정리 또는 교육이 필요하지 않으므로 전문가의 기존 지식을 기반으로 비지니스 규칙을 정의하여 구현 복잡성을 줄일 수 있다.
- 의사 결정 프로세스가 명시적인 "if-then" 사전 정의 규칙에 의존하므로 높은 투명성을 제공한다.
- 본질적으로 정적이며 유연성이 없기 때문에, 사전 정의된 규칙을 수동으로 조정하여 변화나 진화하는 조건에만 적응할 수 있다.
- 사전 정의된 규칙이 명확한 지침을 제공하지 않는 모호하거나 불확실한 상황에 직면할 때 어려움을 겪을 수 있다.
- 미리 정의된 기준에 의존하면, 전문가 개인의 편견이 들어갈 수 밖에 없고, 이로 인해 미묘한 행동을 설명하지 못할 수 있으며 잠재적으로 불공평하거나 부정확한 평가로 이어질 수 있다.

#### Machine Learning AI
- 데이터를 기반으로 규칙성(패턴)을 학습하여 결과를 추론하는 알고리즘이다.
- 현실 세계의 패턴을 분석하여 개발자가 직접 코드를 작성하는 것이 어려웠으나 머신러닝을 이용해서 해결할 수 있다.
- <sub>※</sub> 데이터 마이닝, 음성 인식(언어 구분), 영상 인식(이미지 판별), 자연어 처리(번역, 문맥 찾기)에서 머신러닝이 적용된다.  
<sub>※ 데이터 마이닝이란, 대규모 데이터 안에서 체계적이고 자동적으로 통계적 규칙이나 짜임을 분석하여 가치있는 정보를 빼내는 과정이다.</sub>
- 데이터의 패턴을 학습하여 이를 통해 예측 등을 수행할 수 있다.

1. 지도 학습(Supervised Learning)

> 입력값(문제)과 출력값(정답)을 전달하면, 알아서 특징을 직접 추출하는 방식이다.  
> 다른 입력값(문제)과 동일한 출력값(정답)을 전달하면 새로운 특징을 알아서 추출한다.   

> 문제(Feature)(독립변수)와 답(Target, Label)(종속변수)을 주는 것이다.  
> - 분류 (코로나 양성/음성, 사기 번호/일반 번호 등 단일 값 예측)  
> - 회귀 (1년 뒤의 매출액, 내일 주식 가격 등 연속 값 예측)  

2. 비지도 학습(Unsupervised Learning)

> 입력값(문제)만 전달하고 정답 없이 특징만 추출하는 학습이다.  
> 추출한 특징에 대해 AI가 출력값(정답)을 부여하여 입력값(문제)은 출력값(정답)이라는 것을 알아낸다.

> 문제(Feature)를 주고 답은 주지 않는 것이다. 
> - 군집화 (클러스터링, 비슷한 문제를 분석하여 편을 나누어 각 편으로 모으는 것)
> - 차원 축소 (문제의 개수를 압축(축소)하여 함축된 의미를 찾아내는 것)

3. 강화 학습(Reinforcement Learning)

> https://kr.mathworks.com/discovery/reinforcement-learning.html

#### Machine Learning의 단점
- 데이터에 의존적이다 (Garbage In, Garbage Out), 데이터가 안좋으면 결과도 안좋을 수 밖에 없다.
- 학습 데이터로 잘 만들어진 로직을 가진 모델일지라도 실제 데이터 적용 시 정확한 결과가 나오지 않을 수 있다.
- 머신러닝 학습을 통해 로직이 생기면, 나온 결과가 어떻게 이렇게 나왔는 지에 대한 분석이 쉽지 않다(블랙박스).
- 데이터를 넣으면 원하는 것처럼 좋은 결과를 얻기란 쉽지 않다.

#### R vs Python

- R
  
  > 개발 언어에 익숙하지 않지만 통계 분석에 능한 현업 사용자일 경우
  > 오랜 기간동안 쌓인 다양하고 많은 통계 패키지

- Python
  
  > 직관적인 문법, 객체지향 함수형 프로그래밍언어, 다양한 라이브러리
  > 다양한 영역(운영체제, 서버, 네트워크, 등)으로 연계 및 상용화하기 좋음

### 머신러닝과 딥러닝은 R보다는 "파이썬"을 사용하자!!

### 분류 (Classifier)
- 대표적인 지도학습 방법 중 하나이며, 다양한 문제와 정답을 학습한 뒤 별도의 테스트에서 정답을 예측한다.
- 주어진 문제와 정답을 먼저 학습한 뒤 새로운 문제에 대한 정답을 예측하는 방식이다.
- 이진 분류 (Binary Classification)의 경우 정답은 0(음성, Negative)과 1(양성, Positive)과 같이 True, False값을 가진다.
- 다중 분류 (Muticlass Classification)는 정답이 가질 수 있는 값은 3개 이상이다(예: 0, 1, 2, 3).

#### 피쳐 (Feature) -> 독립변수
- 데이터 세트의 일반 컬럼이며, 2차원 이상의 다차원 데이터까지 통들어 피처라고 한다.
- 타켓을 제외한 나머지 속성을 의미한다.

#### 레이블(Label), 클래스(Class), 타켓(Target), 결정(Decision) -> 종속 변수
- 지도 학습 시, 데이터의 학습을 위해 주어지는 정답을 의미한다.
- 지도 학습 중, 분류의 경우 이를 레이블 또는 클래스라고도 부른다.

<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/31a8a7fb-f13d-458d-9370-90b32668c2ed" width="600px" style="margin-left: 10px">

### 분류 예측 프로세스
<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/57063526-5ed6-4137-8b2c-f439233d8a9c">

#### 데이터 세트 분리
**train_test_split(feature, target, test_size, random_state)**

- 학습 데이터 세트와 테스트 데이터 세트를 분리해준다.
- feature: 전체 데이터 세트 중 feature
- target: 전체 데이터 세트 중 target
- test_size: 테스트 세트의 비율(0 ~ 1)
- random_state: 매번 동일한 결과를 원할 때, 원하는 seed(기준점)를 작성한다.

#### 모델 학습
**fit(train_feature, train_target)** - fit -> 지도학습
- 모델을 학습시킬 때 사용한다.
- train_feature: 훈련 데이트 세트 중 feature
- train_target: 훈련 데이트 세트 중 target

#### 평가
**accuracy_score(y_test, predict(X_test))**
- 모델이 얼마나 잘 예측했는지를 "정확도"라는 평가 지표로 평가할 때 사용한다.
- y_test: 실제 정답
- predict(X_test): 예측한 정답

### 데이터 전처리★☆★☆

#### StandardScaler()
- 데이터의 평균을 0, 분산을 1이 되도록, 표준 정규분포를 따르게 하는 스케일링
- +- 1.96을 벗어나면 이상치로 판단한다.
- <code>from sklearn.preprocessing import StandardScaler</code>

#### MinMaxScaler()
- 데이터가 0~1 사이에 위치하도록 최소값은 0, 최대값은 1로 변환한다
- 서로 다른 단위의 feature끼리 비교가 가능해진다.
- <code>from sklearn.preprocessing import MinMaxScaler</code>

#### MaxAbsScaler()
- 모든 값을 -1~1 사이에 위치하도록, 절대값의 최소값은 0, 최대값은 1이 되도록 변환한다.
- 양의 방향에 대한 단위뿐 아니라 음의 방향에 대한 단위까지 스케일링하고자 할 때 사용한다.
- <code>from sklearn.preprocessing import MaxAbsScaler</code>

#### 결정 트리 (Decision Tree)
- 매우 쉽고 유연하게 적용될 수 있는 알고리즘으로서 데이터의 스케일링, 정규화 등의 데이터 전처리의 의존도가 매우 적다.
- 학습을 통해 데이터에 있는 규칙을 자동으로 찾아내서 Tree 기반의 분류 규칙을 만든다.
- 각 특성이 개별적으로 처리되어 데이터를 분할하는데 데이터 스케일의 영향을 받지 않으므로 결정트리에서는 정규화나 표준화같은 전처리 과정이 필요없다.
- 영향을 가장 많이 미치는 feature를 찾아낼 수도 있다.
- 예측 성능을 계속해서 향상시키면 복잡한 규칙 구조를 가지기 때문에 <sub>❈</sub>과적합(Overfitting)이 발생해서 예측 성능이 저하될 수도 있다.
- 가장 상위 노드를 "루트 노드"라고 하며, 나머지 분기점을 "서브 노드", 결정된 분류값 노드를 "리프 노드"라고 한다.

<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/e77f5bd7-af5c-4394-94f1-bb45abafa561" width="550" style="margin: 20px 0 20px 20px">

- 복잡도를 감소시키는 것이 주목적이며, 정보의 복잡도를 불순도(Impurity)라고 한다.
- 이를 수치화한 값으로 지니 계수(Gini Coeficient)가 있다.
- 클래스가 섞이지 않고 분류가 잘 되었다면, 불순도 낮다.
- 클래스가 많이 섞여 있고 분류가 잘 안되었다면, 불순도 높다.
- 통계적 분산 정도를 정량화하여 표현한 값이고, 0과 1사이의 값을 가진다.
- 지니 계수가 낮을 수록 분류가 잘 된 것이다.

---
<sub>❈ 과적합이란, 학습 데이터를 과하게 학습시켜서 실제 데이터에서는 오차가 오히려 증가하는 현상이다. </sub>

<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/6f2deba2-a18c-4c91-bdd0-d9dfac4122e0" width="350" style="margin: -10px">

#### Graphviz
- 결정트리 모델을 시각화할 수 있다.
- https://graphviz.org/download/  
  graphviz-9.0.0 (64-bit) EXE installer [sha256]
- https://drive.google.com/file/d/1oCXidIjNAvUT2UcNFEdhRfFhnZ96iHrp/view?usp=sharing

#### Feature별 중요도
**각 feature가 분류를 나누는 데에 얼마나 큰 영향을 미쳤는지를 표기하는 척도이다.**
- feature_importances_
- 분류를 결정하는 데에 얼만큼 기여했는지를 feature별로 수치를 리턴해준다

### 교차 검증 (Cross Validation)★☆★☆★☆★☆
- 기존 방식에서는 데이터 세트에서 학습 데이터 세트와 테스트 데이터 세트를 분리한 뒤 모델 검증을 진행한다.
- 교차 검증 시, 학습 데이터를 다시 분할하여 학습 데이터와 모델 성능을 1차 평가하는 검증 데이터로 나눈다.

<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/70bef569-1b55-4504-8c3c-b40ee203671c" width="500px">

#### 교차 검증의 장단점
- 👍특정 데이터 세트에 대한 과적합 방지
- 👍데이터 세트 규모가 적을 시 과소적합 방지
- 👎모델 훈련, 모델 평가에 소요되는 시간 증가
- 즉, 과적합을 피하고 하이퍼 파라미터를 튜닝함으로써 모델을 일반화하고 신뢰성을 증가시키기 위한 목적이다.

#### 교차 검증의 종류
K-Fold
- k개의 데이터 폴드 세트를 만든 뒤 k번만큼 학습과 검증 평가를 반복해서 수행하는 방식.
- 학습 데이터와 검증 데이터를 정확히 자르기 때문에 타겟 데이터의 비중이 한 곳으로 치충될 수 있다.
- 예를 들어, 0, 1, 2 중에서 0, 1, 두 가지만 잘라서 검증하게 되면 다른 하나의 타겟 데이터를 예측할 수 없게 된다.
- Stratified K-Fold로 해결한다.

Stratified K-Fold
- K-Fold와 마찬가지로 k번 수행하지만, 학습 데이터 세트와 검증 데이터 세트가 가지는 타겟 분포도가 유사하도록 검증한다.
- 타켓 데이터의 비중을 항상 똑같게 자르기 때문에 데이터가 한 곳으로 치중되는 것을 방지한다.

<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/7d3224ba-b68a-4e91-9a71-bb09ca7b88a0" width="600px">

GridSearchCV
- 교차 검증과 최족의 하이퍼 파라미터 튜닝을 한 번에 할 수 있는 객체이다
- max_depth와 min_sample_split에 1차원 정수형 list를 전달하면, 2차원으로 결합하여 격자(Grid)를 만들고, 이 중 최적의 점을 찾아낸다.
- 딥러닝에서는 학습 속도가 머신러닝에 비해 느리고, 레이어(층)가 깊어질 수록 조정해주어야 할 하이퍼 파라미터 값이 많아지기 때문에, RandomSearchCV에서 대략적인 범위를 찾은 다음, GridSearchCV로 디테일을 조정하는 방식을 사용한다.

<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/f35f11d9-abcf-4c8a-93c1-89e8dd5ddeed" width="500px">

#### 편하게 수행할 수 있는 교차 검증
**cross_val_score(estimator, x, y, cv, scoring)**
- estimator: classifier 종류 모델이면 내부적으로 startified K-Fold로 진행된다.
- x: features
- y: targets
- cv: 폴드 세트 개수
- scoring: 평가 함수, 정확도(accuracy)외에 다른 것은 다른 장에서 배운다.

#### GridSearchCV
**GridSearchCV(estimator, param_grid, cv, refit, return_train_score)**
- estimator: 학습할 모델 객체 작성
- param_grid: dict형태로 전달해야 하며, 주요 key값은 max_depth, min_samples_split이다.
- cv: 폴드 세트 개수
- refit: 전달한 모델 객체에 최적의 하이퍼 파라미터로 적용하고자 할 때
- return_train_score: 교차 검증 점수를 가져올 지에 대해 True 또는 False를 전달한다.

### 분류 (Classification) 성능 평가 지표★☆★☆★☆★☆★☆★☆★☆★☆★☆(엄청 중요함)

#### 정확도 (Accuracy)
- 직관적으로 모델 예측 성능을 나타낼 수 있다.
- 2진 분류일 경우 데이터 구성에 따라 타겟 데이터 분포가 불균형하다면, 정확도 한 가지만으로는 적합한 성능 평가 지표가 될 수 없다.
- 강아지와 고양이 모두 무조건 생존으로 예측하는 모델이 있다고 가정한다.  
  생존한 강아지 80마리와 사망한 고양이 20마리를 테스트하면, 정확도는 80%이다.
  이 모델을 사용하면, 사망한 강아지 혹은 고양이를 절대 예측할 수 없다.

<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/9adbcc26-0111-4cfe-ab53-50ac0c706937" width="400px">

#### 오차 행렬 (Confusion Matrix)
- 학습된 분류 모델이 예측을 수행하면서 얼마나 예측에 오류가 있는지도 함께 보여주는 지표이다.
- 데이터가 한 곳으로 치우친 것도 확인할 수 있으며, TP, TN, FP, FN, 4가지로 구성되어 있다.
- 오차 행렬로 분류 성능 평가 지표의 모든 것을 구할 수 있다(정확도, 정밀도, 재현율, F1 Score, ROC AUC)

<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/bdf0b82f-7e00-4fc9-a1af-f3f74b3186c1" width="600px">  

1. TN: 예측한 값은 음성이고, 실제 값도 음성일 때 (맞춤)
2. FP: 예측한 값은 양성이고, 실제 값은 음성일 때 (틀림)
3. FN: 예측한 값은 음성이고, 실제 값은 양성일 때 (틀림)
4. TP: 예측한 값은 양성이고, 실제 값도 양성일 때 (맞춤)

- 위 강아지와 고양이의 생존률 예측 모델의 오차 행렬은 다음과 같이 나온다.  
  
<img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/2d763928-7350-476e-9df9-afd69f19419f" width="600px">  

- 100마리 전부 생존(음성, Negative)으로 예측했으며, 그 중 80마리는 실제 음성이고, 나머지 20마리는 실제 양성이기 때문이다.
- 보통 2진 분류일 경우 음성과 양성을 구분하는 의료학, 연구분야 등에서 많이 사용되며, 두 가지 상황으로 나눌 수 있다.
> 1. 질병이나 이상이 없는데도 양성으로 오진하는 것을 방지하기 위해
>> - 특이도(Specificity): 정상을 정상으로 진단하는 비율(▲TN)
>> - 재현율(Recall)이 낮아지고 정밀도(Precision)가 높아질 수 있다.
> 2. 암 진단에서 양성인 환자를 놓치지 않고 최대한 많이 식별하기 위해
>> - 민감도(Sensitivity): 질병이 있는 사람을 질병이 있다고 진단하는 비율(▲TP)
>> - 재현율(Recall)이 높아지고 정밀도(Precision)가 낮아질 수 있다.

- 1.의 경우 Positive보다는 Negative 예측 정확도를 높일 것이다.  
  ▲TN, ▼TP, 또한, Positive로 예측하는 경우가 매우 작기 때문에, ▼FP
- 2.의 경우 Negative보다는 Positive 예측 정확도를 높일 것이다.  
  ▲TP, ▼TN, 또한, Negative로 예측하는 경우가 매우 작기 때문에, ▼FN
- 📌결과적으로 정확한 판단이 아님에도 불구하고 정확도가 매우 높게 나타나는, 수치적인 판단 오류를 해결해기 위해서는 특이도와 민감도를 잘 조절해야한다.  

#### 정밀도 (Precision)
- 예측을 Positive로 한 대상 중, 예측과 실제 값이 Positive로 일치한 데이터의 비율을 뜻한다.
- ▲TP, ▼FP일 경우 정밀도가 상승한다.
- precision_score()를 사용하여 정밀도를 구할 수 있다.

#### 재현율 (Recall)
- 실제 값이 Positive인 대상 중, 얼마나 놓치지 않고 Positive로 예측했는 가의 비율을 뜻한다.
- ▲TP, ▼FN일 경우 재현율이 상승한다.
- recall_score()를 사용하여 재현율을 구할 수 있다.

#### 정밀도와 재현율의 트레이드 오프 (Trade-off)
- 분류 시, 결정 임계값(Threshold)을 조정해서 정밀도 또는 재현율의 수치를 높일 수 있다.

> 가정: 구급대원 AI가 교통사고 현장에서 피해자를 병원으로 이송해야할지 판단해야 하는 시나리오.
> - Dead (Positive): 피해자가 이미 사망했을 경우
> - Alive (Negative): 피해자가 아직 살아있을 경우  

> - TP: 모델이 Dead를 Dead로 올바르게 분류한 경우
> - FP: 모델이 Alive를 Dead로 잘못 분류한 경우 (error I)
> - TN: 모델이 Alive를 Alive로 올바르게 분류한 경우
> - FN: 모델이 Dead를 Alive로 잘못 분류한 경우 (error II)

> - error I의 비용(FP)은 error II의 비용(FN)보다 훨씬 더 나쁘다! ▼FP, ▼error I
> 
> <img src="https://github.com/README-wmoon/study-dataAnalysis/assets/129862668/e47db28b-0c0e-4b40-bef7-fa0b152f5b37" width="500px">

> - 정밀도 (Precision): 모델이 Dead로 예측한 환자 중에서 실제로 Dead인 환자의 비율을 나타낸다. 즉, 양성으로 예측한 결과 중 얼마나 많은 것이 진짜 양성인지 측정한다.  
> - 재현율 (Recall): 실제 Dead 피해자 중에서 모델이 Dead로 정확하게 예측한 피해자의 비율을 나타낸다. 즉, 모델이 얼마나 많은 Dead 피해자를 "놓치지 않고" 감지했는지 측정한다.  

> - 이는 정밀도를 높여야 하며, Threshold(임계값)을 높여서 FP를 낮추고(▲정밀도), FN을 높여야 한다(▼재현율).
> - 즉, Negative(Alive)로 예측할 확률이 높아져야 생명을 구할 확률이 높아지고, Threshold value(임계값)를 높여주는 것이다.
> - 위의 시나리오처럼 한 쪽의 수치를 강제로 높이면 다른 한 쪽의 수치는 떨어지며,  
  이를 정밀도와 재현율의 "트레이드 오프"라고 한다.
> - 임계치가 높아지면 정밀도가 높아진다. 반대로 임계치가 낮아지면 재현율이 높아진다.

#### F1 Score
- 2진 분류 모델의 성능을 평가하는 지표 중 하나이다.
- 정밀도(Precision)와 재현율(Recall)의 조화 평균으로 계산되는 성능 측정 지표이다.
- 정확도(Accuracy)와 같이 전체 성능에 대한 지표가 아닌 타켓 데이터별 성능을 자세히 분석하는 평가지표이다.
- 정밀도(Precision)와 재현율(Recall), 두 개의 평가 지표를 모두 고려하여 예측 성능을 평가하기 때문에 두 지표의 평균치를 구하는 조화 평균을 사용하여 조금 더 정확하게 모델의 예측 성능을 평가할 수 있다.
- 텍스트 분류, 정보 검색, 암 진단 등에서 사용되는 모델의 성능을 평가할 수 있다.

<img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/8a57090f-6fc7-441d-a66d-dfe20a6a43aa" width="600px">

- F1 Score는 0~1까지 점수를 매길 수 있으며, 0에 가까울 수록 정밀도와 재현율 모두 낮다는 뜻이다.

#### ROC Curve, AUC
- ROC(Receiver Operating Characteristic)는 수신기 동작 특성이라는 뜻이고, 이러한 이름이 붙은 이유는 2차 세계대전 때 무선 기기 성능 평가 때 사용되었기 떄문이다. 
- FPR이 변할 때 TPR이 어떻게 변하는지를 나타내는 곡선이며, FPR이 급격히 떨어지더라도 TPR은 천천히 떨어지는 것이 좋은 성능이 가진 모델로 판단한다.  
- AUC(Area Under the Curve)는 ROC 곡선 밑의 면적을 구한 것으로서, 일반적으로 1에 가까울 수록 좋은 수치이다.  


- ROC Curve가 축에 붙을 수록(좌상단 모서리) 좋은 성능을 나타내는 것이며, 높이와 밑변이 1인 사각형으로 가정했을 경우 ROC Curve가 축에 붙을 수록 AUC 면적이 넓어지며 1에 가까워진다.  
- 모델이 양성이 음성을 얼마나 잘 분류하는지 시각화할 수 있다.  
- 보통 F1 Score가 0.7이상일 경우 좋은 모델이라고 간주한다.  

<img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/e18d6116-416a-45a6-bfa5-3bf0f6fc7a2f" width="230px">


### 베이즈 추론, 베이즈 정리, 베이즈 추정 (Bayesian Inference)
- 역확률(inverse probability) 문제를 해결하기 위한 방법으로서, 조건부 확률(P(B|A)))을 알고 있을 때, 정반대인 조건부 확률(P(A|B))을 구하는 방법이다.
- 추론 대상의 사전 확률과 추가적인 정보를 기반으로 해당 대상의 "사후 확률"을 추론하는 통계적 방법이다.
- 어떤 사건이 서로 "배반"하는(독립하는) 원인 둘에 의해 일어난다고 하면, 실제 사건이 일어났을 때 이 사건이 두 원인 중 하나일 확률을 구하는 방식이다.
- 어떤 상황에서 N개의 원인이 있을 때, 실제 사건이 발생하면 N개 중 한 가지 원인일 확률을 구하는 방법이다.
- 기존 사건들의 확률을 알 수 없을 때, 전혀 사용할 수 없는 방식이다.
- 하지만, 그 간 데이터가 쌓이면서, 기존 사건들의 확률을 대략적으로 뽑아낼 수 있게 되었다.
- 이로 인해, 사회적 통계나 주식에서 베이즈 정리 활용이 필수로 꼽히고 있다.  

> ##### 예시
질병 A의 양성판정 정확도가 80%인 검사기가 있다. 검사를 시행해서 양성이 나왔다면, 이 사람이 80%의 확률로 병에 걸렸다고 이야기할 수 없다. 왜냐하면 검사기가 알려주는 확률과 양성일 경우 질병을 앓고 있을 확률은 조건부 확률의 의미에서 정반대이기 때문이다.  
<table style="width:50%; margin-left: 50px">
    <tr>
        <th>전제</th>
        <th>관심 사건</th>
        <th>확률</th>
    </tr>
    <tr>
        <th>병을 앓고 있다</th>
        <th>양성이다</th>
        <th>80%</th>
    </tr>
    <tr>
        <th>양성이다</th>
        <th>병을 앓고 있다</th>
        <th>알수 없음</th>
    </tr>
</table>  

> 이런 식의 확률을 구해야 하는 문제를 역확률 문제라고 하고 이를 베이즈 추론을 활용하여 구할 수 있다.  
단, 검사 대상인 질병의 유병률(사전 확률, 기존 사건들의 확률)을 알고 있어야 한다.  
전세계 인구 중 10%의 사람들이 질병 A를 앓는다고 가정한다.


<div style="width: 60%; display:flex; margin-top: -20px; margin-left:30px">
    <div>
        <img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/07118db9-4c9c-45e6-b16c-61da74686f34" width="300" style="margin-top:20px; margin-left:0">
    </div>
    <div style="margin-top: 28px; margin-left: 20px">
        <img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/672879ab-8e4b-4e4f-a386-9a5512286fbd" width="410" style="margin-top:20px; margin-left:0">
    </div>
</div>  

<div style="width: 60%; display:flex; margin-left:30px">
    <div>
        <img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/56873292-8274-4997-94ff-bf961d7dbf31" width="400" style="margin-top:20px; margin-left:0">
    </div>
    <div style="margin-top: 28px; margin-left: 20px">
        <img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/64af42fb-8c42-4709-9952-ec3c28e572cb" width="550" style="margin-top:-8px; margin-left:0">
    </div>
</div>  

> 🚩결과: 약 30.8%
<img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/9664aa4e-3c39-4ab3-8590-ad4db7530d7a" width="200" style="margin-top:20px; margin-left:0">

### 나이브 베이즈 분류 (Naive Bayes Classifier)
- 텍스트 분류를 위해 전통적으로 사용되는 분류기로서, 분류에 있어서 준수한 성능을 보인다.
- 베이즈 정리에 기반한 통계적 분류 기법으로서, 정확성도 높고 대용량 데이터에 대한 속도도 빠르다.
- 반드시 모든 feature가 서로 독립적이여야 한다. 즉, 서로 영향을 미치지 않는 feature들로 구성되어야 한다.
- 감정 분석, 스팸 메일 필터링, 텍스트 분류, 추천 시스템 등 여러 서비스에서 활용되는 분류 기법이다.
- 빠르고 정확하고 간단한 분류 방법이지만, 실제 데이터에서  
  모든 feature가 독립적인 경우는 드물기 때문에 실생활에 적용하기 어려운 점이 있다.

<img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/a0363323-cb51-41c0-aa18-e345c77c51b8" width="400px">


### 서포터 벡터 머신 (SVM, Support Vectorj Machine)
- 기존의 분류 방법들은 '오류율 최소화'의 목적으로 설계되었다면, SVM은 두 부류 사이에 존재하는 '여백 최대화'의 목적으로 설계되었다.
- 분류 문제를 해결하는 지도 학습 모델 중 하나이며, 결정 경계라는 데이터 간 경계를 정의함으로써 분류를 할 수 있다.
- 새로운 데이터가 경계를 기준으로 어떤 방향에 잡히는지를 확인함으로써 해당 데이터의 카테고리를 예측할 수 있다.
- 데이터가 어느 카테고리에 속할지 판단하기 위해 가장 적절한 경계인 결정 경계를 찾는 선형 모델이다.

<img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/8702cdc7-8fa0-4b03-812c-073e5c2a3a4a" width="400px" style="margin-bottom: 60px"> 

#### 서포트 벡터 (Support Vector)
- 결정 경계를 결정하는 데이터(벡터)들을 서포트 벡터라고 부른다.
- 서포트 벡터들이 결정 경계 (Decision boundary)를 결정한다.
- 서포트 벡터와 결정 경계간의 거리를 마진(Margin)이라고 부르고, 마진이 크면 클 수록 좋은 결정 경계가 된다.
- 서포트 벡터들을 통해 결정 경계를 결정하게 되고, 다른 학습 데이터들은 무시될 수 있기 때문에 SVM의 속도가 빠를 수 있다.

#### 결정 경계 (Decision boundary)
- 새로운 데이터가 들어오더라도 결정 경계를 중심으로 두 집단이 멀리 떨어져 있어야 두 집단을 잘 구분할 수 있기 때문에 일반화하기 쉬워진다.
- 독립 변수의 차원보다 한 차원 낮아지며, N차원 공간에서 한 차원 낮은 N-1차원의 결정 경계가 생긴다.  
  즉, 2차원 공간에서는 초평면이 선으로 결정되고, 고차원에서는 결정 경계는 선이 아닌 평면 이상의 도형이며, 이를 "초평면(Hyperplane)"이라고 부른다.

<img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/9af2dc75-9cda-4f1f-92a9-68116e46e5e5" width="400px" style="margin-bottom: 60px">

#### 하드 마진(Hard margin)
- 매우 엄격하게 집단을 구분하는 방법으로 이상치를 허용해주지 않는 방법이다.
- 이상치를 허용하지 않기 때문에 과적합이 발생하기 쉽고, 최적의 결정경계를 잘못 구분하거나 못찾는 경우가 생길 수 있다.
- C(cost)는 패널티를 조절할 수 있고, 값이 커질수록 결정 경계가 데이터에 더 정확하게 맞춰진다.
- C를 낮추면 일을 덜 하게 하는 것이고, C를 높이면 일을 더 해서 더 섬세하게 찾아낸다.
- C가 너무 낮으면 underfitting될 가능성이 커지고, C가 너무 높으면 overfitting이 발생할 수 있다.

<img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/c2090d25-f228-49e7-b521-f22ec4d65cb6" width="350px" style="margin-bottom: 60px">

#### 소프트 마진(Soft margin)
- 이상치를 허용해서 일부 데이터를 잘못 분류하더라도 나머지 데이터를 더욱 잘 분류해주는 방법이다.
- 이상치 허용으로 인해 데이터의 패턴을 잘 감지하지 못하는 문제점이 생길 수 있다.

<img src="https://github.com/README-wmoon/study-machineLearning/assets/129862668/37aeb853-a850-442b-ae8a-f49c5113de1b" width="550px" style="margin-bottom: 60px">

> 📌 정리  
> 서포트 벡터 머신 알고리즘을 적용한 SVC 모델의 하이퍼파라미터은 Regularization cost, C에 값을 전달하여 ε(패널티)를 조절할 수 있다. C가 클 수록 loss function에서 오차항인 ε<sub>i</sub>의 영향력이 커지게 되기 때문에 마진의 크기가 줄어들고(하드 마진), 반대로 C가 작을 수록 마진의 크기가 늘어난다(소프트 마진). 적절히 조절하면 오히려 성능이 좋아질 수 있다.
