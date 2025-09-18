# Portfolio

* * * * *

## 2024년 임업통계 스마트활용 경진대회 – 산림자원 활용 BM 및 웹페이지
- 예비 임업인을 위한 **작물별 최적 재배지 추천·시각화 서비스**(기후/토양/생산량 통합)  
- 작물 특성마다 **최적 모델이 상이**하여 작물별 맞춤형 모델 채택(SVM/랜덤포레스트/로지스틱)  
- 최종 **웹 데모**(Publr)와 **보고서/PPT** 제공  
- `Python` `GeoPandas` `Matplotlib` `ML(SVM/RF/Logit)` `AUC`  
- [Github](https://github.com/junhyung-L/2024-Forestry-Statistics-Smart-Competition-Contest)

1. Data Collection  
   - 산림청·임진원·기상청 등 공공데이터(재배적지도/토양/유효수분/기후/생산·가격) 수집.  

2. Data Preprocessing & EDA  
   - 생산량 Top 품목 선별, 기후·토양·생산 결합, 결측 **지역 최빈값** 대체, 상관계수로 주요 변수 선별.  

3. Modeling  
   - SVM/랜덤포레스트/로지스틱 회귀로 AUC 평가, **작물별 베스트 모델** 도출(예: 생표고/더덕=RF, 밤/도라지=Logit).  

4. Service / Deliverables  
   - 최적 재배지·연도별 생산량·가격 지도 시각화, Publr 웹 배포 / 최종 보고서·발표자료.  

* * * * *

## 인천e음 캐시백 정책 반응성 분석 & 전략 제언 (2025 산학 캡스톤 경진대회)
- **지역화폐 캐시백 타이밍**을 데이터로 설계하는 정책 분석 프로젝트(정성+정량)  
- LightGBM 기반 **소비 예측 + ROI 시뮬레이션**으로 상향 시기 Top 조합 제시(예: 4·6·9월 등)  
- **금상 수상**, 기간 2025.03.04–06.20  
- `Python` `LightGBM` `Time-series` `Survey/TextMining` `ROI Simulation`  
- [Github](https://github.com/junhyung-L/2025-Industry-Academic-Capstone-Design-Competition)

1. Data  
   - 인천e음 결제/가맹/가입·충전, KOSIS 인구, 거시·심리지표(CSI·금리), 정책 메타(명절/비율변동).  

2. Methods  
   - 설문·뉴스 텍스트마이닝·인터뷰(정성) + LightGBM 예측·Hurst 지수·ROI 시뮬레이션(정량).  

3. Findings  
   - **예산 제약 하 ROI 최대화 규칙**(반등 직전·명절 전/후·장기유지 후 첫 상향). 지역별 차등 운영 가이드.  

4. Outcome  
   - **금상**, 데이터 기반 정책 운영 체계 및 연간 가이드 제시.  

* * * * *

## 신용카드 고객 세그먼트 분류 AI (Dacon)
- 대규모(약 24만 표본·857 피처) 카드 데이터로 **고객 세그먼트 분류**  
- 내부 F1 **0.8936(스태킹)**, 리더보드: Public 0.64636 / Private 0.6251(상위 25%)  
- `Python` `XGBoost` `CatBoost` `Logistic` `Stacking` `Dask`  
- [Github](https://github.com/junhyung-L/Credit-Card-Customer-Segment-Classification-AI-Competition)

1. EDA  
   - 클래스 불균형·결측 구조 분석, 결측 패턴을 **정보로 활용**하는 규칙형 대체 설계.  

2. Preprocessing  
   - 고결측 컬럼 제거/대체, 로그+StandardScaler, LabelEncoder, 대용량 처리를 위한 **Dask**.  

3. Modeling  
   - XGB 베이스라인→개선, CatBoost/LogReg/MLP 비교, **Stacking(meta=LogReg)**로 최고 F1.  

4. SOTA 시도  
   - TabNet/FT-Transformer/NODE 등 딥러닝 탭ular 모델 실험→성능·리소스 한계로 불리.  

5. Results  
   - Public/Private 점수 및 내부 F1·비교표/그래프 정리.  

* * * * *

## 폴린(Fallin): 고령자 낙상 위험 예측 및 안전 경로 안내 (제11회 인천 공공데이터)
- 경사·조도·기상·통계를 융합해 **보행로 단위 낙상 위험도** 산정 및 **지도 시각화**  
- 위험가중치 기반 **최소 위험 경로** 개념 설계, 보고서/노트북/결과물 포함  
- `Python` `Geo/DEM` `Folium` `KOSIS` `Feature Engineering`  
- [Github](https://github.com/junhyung-L/The-11th-Incheon-Public-Data-Utilization-Competition)

1. Data  
   - 보행로/등고선 Shapefile, 도로 조도 CSV, 기상청 API, KOSIS 고령자 통계.  

2. Pipeline  
   - DEM 보간→**경사도** 계산, 시간·좌표 매칭으로 **조도·기상** 결합, **가중 위험 점수**와 등급화.  

3. Viz & Deliverables  
   - Folium 인터랙티브 지도, Tooltip(위험등급/지표), 제출 **PDF 보고서** 및 노트북.  

* * * * *

## 동원×KAIST AI: 페르소나 기반 신제품 월별 수요 예측 (’24.07–’25.06)
- LLM으로 **소비자 페르소나** 생성(속성·가중치·월별 패턴) → **몬테카를로 시뮬레이션**으로 12개월 수요 예측  
- **LightGBM 가격모델**과 유통/광고/프로모션 달력을 반영해 `submission.csv` 산출  
- `Python` `LLM` `MonteCarlo` `LightGBM` `Forecast`  
- [Github](https://github.com/junhyung-L/2025-Dongwon_KAIST-AI-Competition-Unlocking-Future-Sales-Demographics)

1. Problem Setup  
   - 12개월 선행 예측, 페르소나 정의/가중치/계절성, 인지도·재구매·유통·프로모션 반영.  

2. Data/Models  
   - 제품 정보·가격 수집(예: 네이버 쇼핑)→가격 예측 **LightGBM** + 페르소나 시뮬레이션.  

3. Outputs  
   - `results/submission.csv`, `monthly_forecast.csv`, `persona_profiles.json`, 리포트.  

* * * * *

## SubLocal – 지역 소상공인 구독 결제·정산 OMO (FIN:NECT Challenge)
- 소상공인의 **고정 매출 안정화**와 소비자의 **원클릭 주문·자동결제**를 동시에 구현하는 구독형 플랫폼 기획  
- **소비자 앱/점주 대시보드/운영 포털** MVP 플로우와 **KPI·로드맵·아키텍처** 제시  
- `Product Design` `Fintech` `Analytics` `Recommender` `Web Demo`  
- [Github](https://github.com/junhyung-L/2025-FIN.NECT-Challenge)

1. Problem & Solution  
   - 지역 상권 매출 변동성·반복 결제 번거로움 해결: **구독/결제/주문/정산 일체형 OMO**.  

2. MVP & Features  
   - 구독 관리·알림·원클릭 재주문·대시보드 지표·양도 마켓(확장). **웹 데모 링크** 포함.  

3. Architecture & KPI  
   - Subscription Engine/Billing/Analytics/Recommender 구성, 전환·유지·NPS·매출 KPI.  

* * * * *

## 전기차 가격 예측 해커톤 (Read EVs With Data)
- EV 스펙/주행/배터리/연식 등으로 **가격 회귀 예측(XGBoost)**  
- **RMSE(정규화) 0.91972**, 중요 변수: 배터리 용량·최대 주행거리·연식·브랜드·주행거리  
- `Python` `XGBoost` `EDA` `Feature Importance`  
- [Github](https://github.com/junhyung-L/EV-Price-Forecast-Hackathon-Read-EVs-With-Data)

1. EDA & Features  
   - 분포/상관/범주형-가격 관계 분석, 결측 대체·인코딩·이상치 처리.  

2. Modeling  
   - XGBRegressor + 하이퍼파라미터 튜닝, Early Stopping/검증 분할.  

3. Results  
   - 리더보드 RMSE 및 상위 Feature Importance 시각화.  

* * * * *

## 우울증 위험 예측 모델 개발 및 요인 분석
- 대학생 데이터(502명·11변수) 기반 **우울증 위험 분류** 및 **주요 요인 분석**  
- `Python` `Pandas` `Scikit-learn` `Matplotlib` `Seaborn`  
- [Github](https://github.com/junhyung-L/Development-of-Depression-Risk-Prediction-Model-and-Analysis-of-Key-Factors)

1. Data  
   - Kaggle Student Depression Dataset 활용, 노트북/리포트 구성.  

2. Analysis  
   - 변수 탐색·상관·시각화를 통해 위험 요인 정리, 분류 모델링(노트북 기반).

* * * * *

## CTR 광고 클릭 예측 모델 (Dacon) ->정리중
- [Github](https://github.com/junhyung-L/TOSS-NEXT-ML-CHALLENGE-Development-of-Ad-Click-Prediction-CTR-Model)
<!--
- 대학생 데이터(502명·11변수) 기반 **우울증 위험 분류** 및 **주요 요인 분석**  
- `Python` `Pandas` `Scikit-learn` `Matplotlib` `Seaborn`  


1. Data  
   - Kaggle Student Depression Dataset 활용, 노트북/리포트 구성.  

2. Analysis  
   - 변수 탐색·상관·시각화를 통해 위험 요인 정리, 분류 모델링(노트북 기반).  
-->

## 코드 표절률 검사기 ->정리중
- [Github](https://github.com/junhyung-L/Code-Copydetector)
<!--
- 대학생 데이터(502명·11변수) 기반 **우울증 위험 분류** 및 **주요 요인 분석**  
- `Python` `Pandas` `Scikit-learn` `Matplotlib` `Seaborn`  


1. Data  
   - Kaggle Student Depression Dataset 활용, 노트북/리포트 구성.  

2. Analysis  
   - 변수 탐색·상관·시각화를 통해 위험 요인 정리, 분류 모델링(노트북 기반).  
-->

## Marketing Mix ->정리중
- [Github](https://github.com/junhyung-L/Marketing-Mix)
<!--
- 대학생 데이터(502명·11변수) 기반 **우울증 위험 분류** 및 **주요 요인 분석**  
- `Python` `Pandas` `Scikit-learn` `Matplotlib` `Seaborn`  


1. Data  
   - Kaggle Student Depression Dataset 활용, 노트북/리포트 구성.  

2. Analysis  
   - 변수 탐색·상관·시각화를 통해 위험 요인 정리, 분류 모델링(노트북 기반).  
-->
