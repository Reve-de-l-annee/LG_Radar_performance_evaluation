# LG_Radar_performance_evaluation
자율주행 센서의 안테나 성능 예측 AI 경진대회

### [자동차 레이더 공정과정 소개](https://github.com/Reve-de-l-annee/LG_Radar_performance_evaluation/blob/517f956acd5cbd02eb4414af7377831460065111/description/Manufacturing%20process.md)

### [공정 과정별 컬럼 분류](https://github.com/Reve-de-l-annee/LG_Radar_performance_evaluation/blob/0d526ae33a2bf037b1e48425ce47118d44992734/description/Features.md)
---

| 프로젝트 순서 | Point | 세부 내용 |
| --- | --- | --- |
| 문제 정의 | 해결할 점, 찾아내야할 점 | 공정 데이터와 제품 성능간 상관 분석을 통해 제품의 불량을 예측/분석 |
| 데이터 수집 | 공개 데이터, 자체 수집, 제공된 데이터 | LG Aimers (train, test) |
| 데이터 전처리 | 문제에 따라서 처리해야할 방향 설정 | 6시그마로 outlier 탐지, '방열재료 1,2,3의 면적 대비 무게, 회전수 당 삽입깊이' 추가 |
| Feature Engineering | 모델 선정 혹은 평가 지표에 큰 영향 | Feature Selection |
| 알고리즘 선택 | 기본적, 현대적 | RF, XGBoost, LightGBM, MultioutputRegressor |
| 모델 학습 | 하이퍼파라미터,데이터 나누기 | Default, train, val, test |
| 모델 평가 | 확률 | Normalized RMSE (NRMSE) |
| 모델 성능 향상 | 성능 지표, 하이퍼파라미터, 데이터 리터러시 재수정 | Bayesian-optimization, HyperOpt 파라미터 튜닝|
