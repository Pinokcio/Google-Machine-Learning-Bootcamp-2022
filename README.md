# Google-Machine-Learning-Bootcamp-2022

구글 ML 부트캠프의 기록 ( 2022/06/15 ~ 2022/09/15 )

### <Coursera 강의 수강>
- [Deep Learning Specialization (Coursera)](https://www.notion.so/heesungu/Deep-Learning-Specialization-b1666dabf20f47feaab59131528d7842)
  - 머신러닝 학습 과정을 기초단계부터 설명해준다.
  - Optimization, Regularization, Hyperparameter tuning 등을 다룬다.
  - ML project의 과정을 목표 설정 단계부터 피드백 단계까지 다루며, 그 사이 여러 방법들을 제시한다. 
  - Computer Vision의 기초를 다룬다.
  - NLP의 기초를 다룬다.
- [Tensorflow for AL/ML/DL (Coursera)](https://www.notion.so/heesungu/TensorFlow-for-AI-ML-DL-2c9743e81696418d8f0189a90f1310b7)
  - Tensorflow의 기초를 설명한다.
  - Computer Vision 문제를 다룰 때 사용되는 여러 함수 및 다양한 방법론을 다룬다.
  - NLP 문제를 다룰 때 사용되는 여러 합수 및 다양한 방법론을 다룬다.
  - Time Series Data를 다루며 CNN과 RNN 등을 이용하여 Prediction하는 방법을 설명한다.

후기 : 
- 강의에서는 부트캠프를 시작하기 이전부터 알고 있던 내용을 상당수 다루었다. 그만큼 기초적인 내용이 대부분이라고 할 수 있다. 하지만 들으면서 그간 알았던 지식들의 깊이가 얕았구나라는 느낌을 받았다. 
- layer를 쌓고 각 layer가 어떤 기능을 하는지는 알고 있었지만 그 layer를 tensorflow나 pytorch와 같은 워크프레임 없이는 구현해본적도 없고 구현할수도 없었다. 하지만 이 강의에서는 그런 내용을 다룬다. regularization이나 optimization를 포함한 학습 과정 또한 forward, back propagation을 직접 계산하며 하나하나 집고 넘어간다. 
- 하이퍼파라미터 튜닝은 ML 개발에서 가장 중요하다고도 볼 수 있지만 그 과정은 경험적이니 직접 해보라는 말을 들을 때가 많았다. 그렇기때문에 항상 시작이 애매했는데 이 강의에서는 그러한 가이드라인을 제시해준다. 직접 다양한 하이퍼파라미터를 설정하도록 하고 그 변화를 보는 방법을 알려줌으로써 해석의 눈을 기를 수 있었다.
- 습관처럼 train/dev/test set을 나누지만 각 크기를 나누고 해석하며 피드백까지 이어지기는 어려웠다. 이 강의에서는 그러한 경험까지 공유해주며 모델 개선 방향을 제시해주었다. 
- 이외에도 다양한 모델 및 함수의 활용을 배우고 ML 엔지니어로서의 기초를 다지는데 큰 도움이 됐다.

### <Tensorflow Developer Certificate 자격증 취득>
![TensorFlow_Developer_Certificate_유희성](https://user-images.githubusercontent.com/28750225/191905028-c7e6b6f7-7194-4c0c-8ef6-f63a2a8ecc7a.PNG)

후기 :
- Coursera 강의를 베이스로 3~4일정도의 준비기간 후 시험을 봤다.
- 간단한 regression, cnn, rnn, lstm, time series 문제가 나왔다.
- 모든 데이터를 사용하고싶은 욕심때문에 valid set 설정을 안했더니 제출결과가 오락가락해서 다시 설정하였다.
- time series 문제에서 lstm을 사용하여 문제를 푸는데 output의 형식이 맞지 않아 오류가 발생했다. lstm의 return_sequnece를 잘못설정해서 발생한 문제였다.
- 2번문제의 테스트케이스가 가끔 4/5로 나오는것을 제외하고는 5/5로 시험을 마감했다.

### <Kaggle 대회 참가>
[Paddy Doctor: Paddy Disease Classification](https://www.kaggle.com/competitions/paddy-disease-classification/overview)에 참가하였다.

https://github.com/Pinokcio/Google-Machine-Learning-Bootcamp-2022/blob/main/Kaggle/Paddy_disease_prediction.ipynb

- 학습데이터가 꽤 많았기 때문에 학습환경과 시간을 생각했을 때, 가벼운 모델을 사용하는 것이 좋겠다고 판단하였다.
- InceptionV3 : 속도는 빠르나 accuracy가 낮음
- efficientNet : 속도도 준수하고 accuracy도 괜찮게 나옴. B2, B4, V2S, V2L 등의 모델을 다양하게 사용함
- SwinTransformer : 속도는 비교적 느리나 accuracy가 괜찮게 나옴. 메모리 사용량이 높은 관계로 batch size를 낮게 설정함
- 위 모델들 중 성능이 괜찮게 나온 모델들에 대해 soft voting을 실행하여 결과로 제출함 
- 결과 : public 25% / private 31%
- [기록](https://www.notion.so/heesungu/paddy-disease-prediction-32c5c03938744156a768e5321134729a)

[2022 september TPS](https://www.kaggle.com/competitions/tabular-playground-series-sep-2022/overview)에 참가하였다.

https://github.com/Pinokcio/Google-Machine-Learning-Bootcamp-2022/blob/main/Kaggle/TPS2022SEP.ipynb

- [기록](https://www.notion.so/heesungu/2022-Sep-TPS-kaggle-b23397c7e3bb4b138a6e3fbe10aca140)
