# Portfolio

---

## 2024년 임업통계 스마트활용 경진대회 – 산림자원 활용 BM 및 웹페이지
- 예비 임업인을 위한 **작물별 최적 재배지 추천·시각화 서비스** 개발 (기후/토양/생산량 통합 분석)  
- 작물 특성마다 **모델 성능 차이**가 있어, 작물별 맞춤형 ML 모델 채택(SVM/랜덤포레스트/로지스틱 회귀)  
- 최종 결과물: **웹 데모 서비스(Publr)** 및 **보고서·발표자료(PPT)** 제출  
- `Python` `GeoPandas` `Matplotlib` `ML(SVM/RF/Logit)` `AUC`  
- [Github](https://github.com/junhyung-L/2024-Forestry-Statistics-Smart-Competition-Contest)

1. **Data Collection**  
   - 산림청, 임업진흥원, 기상청 등에서 재배 적지도·토양 정보·기후 데이터·생산량·가격 데이터를 통합 수집.  

2. **Data Preprocessing & EDA**  
   - 생산량 상위 품목 중심으로 데이터 구성, 결측치는 지역 단위 **최빈값 대체** 적용.  
   - 상관분석 기반으로 주요 변수 선별, 기후-토양-생산 간 상관 구조 시각화.  

3. **Modeling**  
   - SVM, 랜덤포레스트, 로지스틱 회귀 모델별 AUC 성능 비교.  
   - 작물별 최적 모델 도출 (예: 표고/더덕=RF, 밤/도라지=Logit 등).  

4. **Service / Deliverables**  
   - 최적 재배지·연도별 생산량·가격을 지도 기반으로 시각화.  
   - Publr 플랫폼을 통해 웹 시연 서비스 제공.  
   - 최종 보고서 및 발표자료 제출.  

---

## 인천e음 캐시백 정책 반응성 분석 & 전략 제언 (2025 산학 캡스톤 경진대회)
- **지역화폐 캐시백 타이밍** 최적화를 위한 정책 분석 연구 (정성 + 정량 접근 결합)  
- LightGBM 기반 **소비 예측 모델 + ROI 시뮬레이션** → 최적 상향 조합 제시 (예: 4·6·9월)  
- 대회 최종 **금상 수상**, 기간: 2025.03.04–06.20  
- `Python` `LightGBM` `Time-series` `Survey/TextMining` `ROI Simulation`  
- [Github](https://github.com/junhyung-L/2025-Industry-Academic-Capstone-Design-Competition)

1. **Data**  
   - 인천e음 결제/가맹/가입·충전 데이터, KOSIS 인구 통계, 거시·심리지표(CSI, 금리 등), 정책 메타데이터(명절·비율 변화).  

2. **Methods**  
   - 정성: 설문조사, 뉴스 텍스트마이닝, 소비자 인터뷰.  
   - 정량: LightGBM 예측, Hurst 지수 기반 패턴 탐지, ROI 시뮬레이션.  

3. **Findings**  
   - **예산 제약 하 ROI 최대화 규칙** 발견:  
     - 소비 반등 직전 시점 상향  
     - 명절 전·후 집중 운영  
     - 장기 유지 후 첫 상향 효과 극대화  
   - 지역별 차등 운영 전략 제시.  

4. **Outcome**  
   - 금상 수상, 데이터 기반 연간 정책 가이드라인 설계.  

---

## 신용카드 고객 세그먼트 분류 AI (Dacon)
- 약 24만 명 × 857 피처의 대규모 데이터로 **고객 세그먼트 분류 AI** 개발  
- 내부 F1 **0.8936(스태킹)** 달성, 리더보드: Public 0.64636 / Private 0.6251 (상위 25%)  
- `Python` `XGBoost` `CatBoost` `Logistic` `Stacking` `Dask`  
- [Github](https://github.com/junhyung-L/Credit-Card-Customer-Segment-Classification-AI-Competition)

1. **EDA**  
   - 클래스 불균형 및 결측 구조 파악.  
   - 결측값 자체를 정보로 활용하는 규칙형 대체 전략 설계.  

2. **Preprocessing**  
   - 고결측 컬럼 제거 및 대체, 로그 변환+표준화, 범주형 인코딩(LabelEncoder).  
   - **대용량 처리 최적화**를 위해 Dask 도입.  

3. **Modeling**  
   - XGBoost를 기본 모델로 발전.  
   - CatBoost, Logistic Regression, MLP와 비교 실험.  
   - **Stacking(meta=LogReg)**으로 최고 성능 확보.  

4. **SOTA 시도**  
   - TabNet, FT-Transformer, NODE 등 딥러닝 탭ular 모델 실험.  
   - 성능·리소스 한계로 불리했으나 학습적인 의의 확보.  

5. **Results**  
   - Public/Private 점수, 내부 F1, 모델별 성능 비교표 및 시각화.  

---

## 폴린(Fallin): 고령자 낙상 위험 예측 및 안전 경로 안내 (제11회 인천 공공데이터 경진대회)
- 경사·조도·기상·인구통계를 융합한 **보행로 단위 낙상 위험도 산정 및 지도 시각화**  
- 위험 가중치 기반 **최소 위험 경로 안내 개념** 설계  
- 최종 보고서·주석 포함 노트북·결과물 제출  
- `Python` `Geo/DEM` `Folium` `KOSIS` `Feature Engineering`  
- [Github](https://github.com/junhyung-L/The-11th-Incheon-Public-Data-Utilization-Competition)

1. **Data**  
   - 보행로/등고선 Shapefile, 도로 조도 CSV, 기상청 API, 고령자 통계 데이터 활용.  

2. **Pipeline**  
   - DEM 보간 후 **경사도 계산**, 시간·좌표 기반 **조도·기상 데이터 결합**.  
   - 위험 점수를 가중합산하여 등급화(낮음~매우 높음).  

3. **Viz & Deliverables**  
   - Folium 기반 인터랙티브 지도 제공.  
   - 위험도 Tooltip, 지도 시각화, PDF 보고서 및 노트북 완성.  

---

## 동원×KAIST AI: 페르소나 기반 신제품 월별 수요 예측 (2024.07–2025.06)
- LLM 기반 **소비자 페르소나 생성** → 속성/가중치/월별 패턴 정의  
- **몬테카를로 시뮬레이션**으로 12개월 수요 예측  
- LightGBM 가격 예측 모델과 유통/광고/프로모션 달력 반영 → 최종 `submission.csv` 산출  
- `Python` `LLM` `MonteCarlo` `LightGBM` `Forecast`  
- [Github](https://github.com/junhyung-L/2025-Dongwon_KAIST-AI-Competition-Unlocking-Future-Sales-Demographics)

1. **Problem Setup**  
   - 12개월 선행 수요 예측.  
   - 페르소나별 정의·속성 가중치·계절성·인지도·재구매율 고려.  

2. **Data/Models**  
   - 제품 가격 데이터 수집(네이버 쇼핑 등).  
   - LightGBM 가격 모델 학습 + 페르소나 시뮬레이션 결합.  

3. **Outputs**  
   - `submission.csv`, `monthly_forecast.csv`, `persona_profiles.json` 등 산출물 구성.  

---

## SubLocal – 지역 소상공인 구독 결제·정산 OMO (FIN:NECT Challenge)
- 소상공인의 **매출 안정성**과 소비자의 **편리한 자동 결제 경험**을 동시에 제공하는 구독형 플랫폼 기획  
- 소비자 앱/점주 대시보드/운영 포털로 구성된 **OMO 서비스 플로우**와 **KPI·로드맵·아키텍처** 제시  
- `Product Design` `Fintech` `Analytics` `Recommender` `Web Demo`  
- [Github](https://github.com/junhyung-L/2025-FIN.NECT-Challenge)

1. **Problem & Solution**  
   - 지역 상권 매출의 불안정성과 반복 결제 번거로움을 해결.  
   - **구독/결제/주문/정산 일체형 OMO 서비스**로 해결책 제안.  

2. **MVP & Features**  
   - 구독 관리, 알림, 원클릭 재주문, 점주 대시보드 지표, 양도 가능한 구독권 마켓 설계.  
   - 실제 **웹 데모 링크** 포함.  

3. **Architecture & KPI**  
   - Subscription Engine, Billing, Analytics, Recommender로 서비스 구조 제시.  
   - KPI: 전환율, 유지율, NPS, 매출 개선.  

---

## 전기차 가격 예측 해커톤 (Read EVs With Data)
- EV 스펙·주행·배터리·연식 데이터 기반 **가격 회귀 예측(XGBoost)**  
- **RMSE(정규화) 0.91972** 달성, 주요 변수: 배터리 용량·최대 주행거리·연식·브랜드·주행거리  
- `Python` `XGBoost` `EDA` `Feature Importance`  
- [Github](https://github.com/junhyung-L/EV-Price-Forecast-Hackathon-Read-EVs-With-Data)

1. **EDA & Features**  
   - 변수 분포 및 상관 분석, 범주형 변수와 가격 관계 확인.  
   - 결측 대체, 이상치 처리 및 인코딩.  

2. **Modeling**  
   - XGBRegressor 기반 회귀 모델.  
   - Hyperparameter Tuning + Early Stopping 적용.  

3. **Results**  
   - 리더보드 RMSE 공개, Feature Importance 시각화로 주요 요인 도출.  

---

## 우울증 위험 예측 모델 개발 및 요인 분석
- 대학생 데이터(502명·11변수) 기반 **우울증 위험 분류 모델** 구축  
- 주요 위험 요인 탐색 및 변수 영향력 시각화  
- `Python` `Pandas` `Scikit-learn` `Matplotlib` `Seaborn`  
- [Github](https://github.com/junhyung-L/Development-of-Depression-Risk-Prediction-Model-and-Analysis-of-Key-Factors)

1. **Data**  
   - Kaggle Student Depression Dataset 활용.  

2. **Analysis**  
   - 변수별 탐색·상관 분석, 위험 요인 도출.  
   - Logistic Regression, RandomForest 등 분류 모델 학습 및 평가.  

3. **Deliverables**  
   - 시각화 그래프 및 분석 리포트.  

---

## CTR 광고 클릭 예측 모델 (Dacon) – 정리중
- [Github](https://github.com/junhyung-L/TOSS-NEXT-ML-CHALLENGE-Development-of-Ad-Click-Prediction-CTR-Model)

---

## 코드 표절률 검사기 – 정리중
- [Github](https://github.com/junhyung-L/Code-Copydetector)

---

## Marketing Mix – 정리중
- [Github](https://github.com/junhyung-L/Marketing-Mix)

---
