

# 2023-2 NLP 2nd Project: Toxicity Detection

## 1. 데이터 이해
먼저, 제공된 데이터를 이해하는 것이 중요합니다. `train.csv`와 `test_for_inference.csv` 파일을 살펴보고, 댓글 텍스트와 악성 여부 레이블을 확인하세요.

## 2. 데이터 전처리
데이터 전처리는 NLP 프로젝트에서 중요한 단계입니다. 텍스트 데이터를 정제하고, 토큰화하며, 불용어를 제거하고, 텍스트를 숫자로 변환하는 등의 작업을 수행합니다.

## 3. 모델 구현
실습시간에 다루었거나 해당 내용 기반으로 응용할 수 있는 모델(word2vec, MLP, RNN 등)을 사용하여 악성 댓글 탐지 모델을 구현합니다. 트랜스포머 모델은 사용할 수 없습니다.

## 4. 모델 학습 및 평가
전처리된 데이터를 사용하여 모델을 학습시키고, 이를 평가합니다. 이 과정에서는 F1 및 ROC AUC를 이용해 평가합니다.

## 5. 결과 제출
`submission.csv` 파일을 생성하여 `test_data_for_inference.csv`에 대한 예측 결과를 추론하여 제출합니다. 또한, 재현 가능한 코드와 보고서도 함께 제출합니다. 보고서에는 최종 제출한 예측값을 위해 사용된 모델 구조 설명 및 모델 선택 과정의 근거가 되는 비교 실험 결과 등을 포함해야 합니다.

## 6. 유의 사항
- 제출 기한은 12월 14일 목요일 23:59입니다.
- 문화관 408호 실습실 환경에서 재현 가능해야 합니다.
- 실습 예제 코드, 검색 가능한 코드, LLM이 생성한 코드 등을 사용해도 됩니다. 하지만, 코드를 이해하고 사용해야 하며, 참조한 경우 어떤 부분을 얼마나 참조하였는지 보고서에 참조한 소스 URL과 함께 명시해야 합니다.
- 과제 제출물에 대해 정량적, 정성적 코드 유사도 검증을 수행합니다. 정량, 정성적 유사도가 높은 학생은 게시판을 통해 공지하며, 소명 기회를 제공합니다. 표절로 판명될 경우 코드가 유사한 학생들 모두 F 학점입니다.

이 가이드라인을 따라 프로젝트를 진행하면 좋을 것 같습니다. 추가적인 도움이 필요하시면 언제든지 말씀해주세요. 화이팅입니다! 😊

### 1. 데이터 이해 및 전처리
- 우선 주어진 train.csv 파일을 통해 데이터를 이해하는 것이 중요합니다. 댓글 텍스트와 해당 댓글이 악성인지 아닌지를 나타내는 레이블을 확인해보세요.
- 텍스트 데이터의 경우 일반적으로 전처리 과정이 필요합니다. 예를 들어, 불필요한 특수문자 제거, 소문자화, 불용어 제거, 토큰화 등의 작업을 수행해볼 수 있습니다.

### 2. 모델 구현
- 요구사항에 따르면 word2vec, MLP, RNN 등을 활용한 모델을 구현하셔야 합니다. 
- word2vec을 통해 단어 임베딩을 생성하고, 이를 RNN이나 MLP에 입력으로 사용하여 악성 댓글을 분류하는 모델을 만들 수 있습니다.

### 3. 모델 학습 및 검증
- 모델 학습에는 train.csv를 사용하고, 모델 성능을 검증하기 위해 데이터를 훈련 세트와 검증 세트로 분리할 수 있습니다. 
- 모델 성능은 F1 점수와 ROC AUC를 기준으로 평가하니, 이 두 가지 지표를 기준으로 모델을 평가하며 학습을 진행해야 합니다.

### 4. 예측 및 제출
- 학습된 모델을 통해 test_for_inference.csv의 댓글에 대한 악성 댓글 여부를 예측합니다.
- 예측 결과를 submission.csv에 작성하여 제출합니다.

### 5. 보고서 작성
- 프로젝트의 전체 과정, 사용한 모델, 모델 선택 과정의 근거, 실험 결과 등을 포함하여 보고서를 작성합니다.

주어진 요구사항을 충족시키기 위해 프로젝트를 이와 같이 진행해보는 것은 어떨까요? 이 외에 추가적인 도움이 필요하시면 언제든지 말씀해주세요.
