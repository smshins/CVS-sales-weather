# CVS-sales-weather
How convenience store sales change according to weather condition

---

## Introduction 개요
How the weather impacts convenience store sales?
This analysis targets to predict sales indicators based on the daily and hourly weather conditions using Machine Learning methods.
By applying multiple ML methods, it aims to choose best-performanced model among them.

---

## Datasets 데이터셋

- Time period 기간: 2017.1.1 ~ 2018.12.31
- Datasets from 데이터 출처:
  - CVS sales data: convenience store sales data
  - Weather data: Korea Meteorological Administration(KMA, 기상청) datasets, Air Korea
- Data includes 데이터 구성:
  - CVS sales data: sales quantity, total sales, number of transactions by time unit(3 hours) and product category
  - Weather data: precipitation, daily/hourly temperature, snow/rain flags, air quality indices (PM10, PM2.5)
  - Data were collected from 7 metropolitan cities in South Korea - Seoul, Busan, Guangju, Daejeon, Daegu, Ulsan, Incheon.

---

## Machine Learning Models 분석 방법

총 8가지 머신 러닝 알고리즘을 적용하여, 날씨 정보를 바탕으로 제품군의 매출/판매량/거래건수를 예측하였다.
A total of 8 algorithms were used to predict sales metrics based on weather features:

| Model Group         | Algorithms Used                                      |
|---------------------|------------------------------------------------------|
| Decision Tree-based | Decision Tree                        |
| Ensemble (Bagging)  | Random Forest, Bagging                                             |
| Ensemble (Boosting) | AdaBoost, Gradient Boosting, XGBoost                 |
| Other Classifiers   | Support Vector Machine (SVM), K-Nearest Neighbors (KNN) |

---

## Key Insights 주요 결과

### 요약
- 미세먼지 농도가 높은 날에는...
- 강수량이 많을수록...
- 기온이 높을수록...
- Boosting/Bagging 계열 모델들이 높은 예측 정확도 ($R^2$, RMSE) 기록

### 모델 성능 비교


---

## 폴더 구조

- `data/` : 분석에 사용된 원본 & 가공 데이터
- `notebooks/` : 데이터 전처리, EDA, 모델링 주피터 노트북
- `results/` : 시각화 결과 이미지, 모델 성능 비교표 등의 분석 결과
- `requirements.txt` : 필요한 라이브러리 목록

---

## 사용 기술 스택 Tech Stack

- Python (pandas, numpy, matplotlib, seaborn, sci-py)
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## 연락처
- GitHub:
- Email:
