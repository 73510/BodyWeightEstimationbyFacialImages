# 셀카로 몸무게 예측하기

이 프로젝트는 얼굴 사진(정면 및 측면)과 기본 정보(키, 성별, 인종)만으로 몸무게를 예측하는 AI 모델을 개발합니다.

## 주요 기능

- 얼굴 이미지와 정형 데이터를 결합한 하이브리드 모델
- EfficientNet을 사용한 이미지 특징 추출
- 정형 데이터 처리를 위한 DNN 모델
- 전체 데이터 학습 후 아시아인 데이터로 fine-tuning

## 파일 구조

- `01_preprocess.ipynb`: 데이터 전처리 
- `02_front_model.ipynb`: 정면 얼굴 모델 
- `03_side_model.ipynb`: 측면 얼굴 모델
- `04_structured_data_model.ipynb`: 정형 데이터 모델
- `05_hybrid_model.ipynb`: 하이브리드 모델 구현
- `06_transfer2asian.ipynb`: 아시아인 데이터 fine-tuning
- `07_model_test.ipynb`: 모델 테스트 및 평가

## 성능

- 평균 절대 오차(MAE): 5.05kg
[Used the dataset from kaggle](https://www.kaggle.com/datasets/elliotp/idoc-mugshots)

## 향후 계획

- 데이터 증강 기법 강화
- 얼굴 특징점 추출 알고리즘 개선
- 앙상블 기법 적용
- 전신 사진 활용 및 체형 분석 추가
- 시계열 데이터 분석 도입
