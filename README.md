# Used Car Price Prediction by Regression

본 프로젝트는 중고차의 가격에 영향을 미치는 주요 요인을 식별하고, 이를 바탕으로 회귀 분석 모델을 통해 중고차 가격을 예측하는 것을 목표로 합니다. 실제 중고차 거래 플랫폼에서 수집한 데이터를 기반으로 전처리, EDA, 회귀모델 구축, 진단, 해석의 전 과정을 포함하고 있습니다.

<br/>

## 프로젝트 개요

- **프로젝트 주제**: 중고차 가격 결정 요인 분석 및 예측 모델링
- **분석 방법**: 다중선형회귀분석 (OLS), 이상치 제거, 변수 변환, 정규성 검정 등
- **진행 목적**: 회귀모델의 이론적 배경을 실제 데이터에 적용하여 실무 능력 향상 및 통찰 도출

<br/>

## 파일 구성

| 파일명 | 설명 |
|--------|------|
| `usedcarprice_prediction_by_regression.ipynb` | 전체 분석이 포함된 주피터 노트북 |
| `car_data.csv` | 분석에 사용된 정제된 데이터셋 |
| `중고차 가격 예측 회귀분석 보고서.pdf` | 분석 과정과 결과를 요약한 프로젝트 보고서 |

<br/>

## 사용한 변수 요약

- **독립 변수**:  
  - `Miles`: 주행 거리  
  - `MSRP`: 신차 가격  
  - `Interior`, `Exterior`: 차량 내부/외부 색상 선호도  
  - `Accident Reported`: 사고 유무  
  - `Past Owners`: 소유주 수

- **종속 변수**:  
  - `Used Car Price`: 중고차 가격

<br/>

## 주요 분석 내용

- 데이터 전처리: 결측값/이상값 제거, 문자열 정제, 수치형 변환
- 탐색적 분석 (EDA): 변수 간 상관관계 시각화, 변수 축소 및 범주화
- 회귀모형 구축: 다중선형회귀 분석(OLS), 변수 선택, 이상치 제거
- 모델 진단: R², AIC/BIC, VIF, Q-Q Plot, Cook's Distance 등
- 해석: 각 변수의 회귀계수에 따른 중고차 가격 영향 해석

<br/>

## 결과 요약

| 변수               | 해석                                                                 |
|--------------------|----------------------------------------------------------------------|
| 주행 거리 (Miles)   | 1 mile 증가 시 약 0.15달러 가격 하락                                 |
| 외부 색상 (Exterior)| 인기색일 경우 약 $624 상승                                            |
| 내부 색상 (Interior)| 선호색상일 경우 약 $1,112 상승                                        |
| 사고 유무           | 사고 발생 시 약 $678 하락                                             |
| 소유주 수           | 소유주 수가 많을수록 약 $2,285 하락                                   |
| 신차 가격 (MSRP)    | MSRP의 약 39% 수준에서 가격 결정됨                                    |

<br/>

## 데이터 및 참고 자료

- 분석 데이터 출처: 
  [Used Car Price Prediction Dataset (Kaggle)](https://www.kaggle.com/datasets/ayaz11/used-car-price-prediction/data?select=car_web_scraped_dataset.csv)

- 외부 참고 자료:  
  [Axalta 글로벌 차량 색상 선호도 리포트](https://www.axalta.com/kr/ko_KR/ColorCompetency/ColourPopularityReports.html)

<br/>
 
- **분석 도구**: Python, Jupyter Notebook, pandas, statsmodels, matplotlib 등

---
