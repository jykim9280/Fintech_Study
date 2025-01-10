# Fintech_Study
스타트업 서비스기획팀 팀장인 ChatGPT가 캐글 데이터를 바탕으로한 과제를 준 개인 프로젝트

## 250111_신용카드 고객 데이터 분석
데이터 : [Credit Card customers](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers/data)
### 주요 작업
- 고객 세그먼트 도출 : 고객의 연령대, 소득 수준, 신용 사용 비율 등을 분석하여 고객을 그룹화하고, 각 그룹에 맞는 카드 추천 전략을 수립
- LightGBM 모델을 선정하여 예측 모델을 최적화
### 분석 결과 보고서
1. 최적 모델
- 모델: LightGBM
- F1 Macro Score: 0.78
2. 최종 모델 성능
  
| Metric         | Precision | Recall | F1-Score |
|----------------|-----------|--------|----------|
| Class 0 (Basic)| 0.99      | 0.98   | 0.99     |
| Class 1 (Silver)| 0.67     | 0.72   | 0.69     |
| Class 2 (Gold) | 0.60      | 1.00   | 0.75     |
| Class 3 (Platinum)| 0.70  | 0.80   | 0.74     |
3. 데이터 추가 분석
- **새로운 특성 추가**: `Avg_Trans_Amt`
- **시각적 결과**: Gold 카드 고객의 평균 거래 금액이 가장 높음.
