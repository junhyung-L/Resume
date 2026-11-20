# 이준형 | 데이터 사이언티스트

[English](README.en.md)

[junhyunglee.kr@gmail.com](mailto:junhyunglee.kr@gmail.com) · [GitHub](https://github.com/junhyung-L) · [LinkedIn](https://www.linkedin.com/in/junhyung-lee-data) · [포트폴리오](https://github.com/junhyung-L/Portfolio/blob/main/README.ko.md)

## 소개

고객·정책·공간 데이터로 예측 모델과 의사결정 시뮬레이션을 만듭니다. 결과마다 데이터 범위와 평가 조건, 결과가 보여 주는 것과 보여 주지 않는 것을 함께 적습니다.

## 경력

- **인턴** | 하나금융융합기술원 BigData&AI Cell, 2026.07.13–현재
  - 기존 주식등급평가모형을 재구현할 수 있도록 시장·재무 데이터 전처리와 변수 생성 로직을 명세서로 정리하고, AI 보조 코딩으로 재구현해 원본 결과와 비교·검증했습니다.
  - 신용카드 스코어카드 모형을 구현하고, 블록체인 데이터를 활용해 이상거래탐지(FDS) 분석을 수행했습니다.
  - 사내 데이터 분석·사이언스 프로그램의 기능을 파악하고 개선 사항을 도출했습니다.
- **학부연구생** | 인천대학교 [DIVE Lab](https://github.com/thekimk/DIVE-Research), 2025.02–2026.02 — 아래 구매 전환 예측 논문 제1저자, 마케팅 피로도 효과에 대한 인과추론 후속 연구 진행 중

## 연구

### [동태적 마케팅 지식 기반 구매 전환 예측](https://github.com/junhyung-L/crm-conversion-prediction) | 제1저자, 『마케팅연구』(한국마케팅학회) 2026.11 게재 예정

- REES46 CRM 메시지 1억 7,200만 건(고객 약 185만 명, 캠페인 1,907개, 전환율 0.1234%)에서 구매 주기·시계열적 반응·마케팅 피로도·채널 효과성의 4대 동태적 피처군을 설계하고 9종 모형을 비교했습니다.
- XGBoost가 원분포 holdout에서 F1 0.3806, PR-AUC 0.3620으로 가장 높았고, 재현율을 0.3074에서 0.5230으로 끌어올렸습니다. 상위 0.78% 메시지가 전환의 95.83%를 포착합니다(정밀도 15.26%, 무작위 대비 123.7배).

### Context-Aware Conversion Intelligence | 제2저자, Ubi-Media 2027 발표 채택

- 김경원, 이준형. 「Context-Aware Conversion Intelligence: A Data-Centric and Resource-Efficient Framework for Ultra-Sparse Multichannel E-Commerce Interactions」. 제15회 International Conference on Ubi-Media Computing(2027년 1월, 일본 오키나와) 발표 논문으로 채택. 위 CRM 연구와 같은 데이터·변수를 다룬 국제학술대회 논문이며, 기여는 Conceptualization, Investigation입니다.

## 프로젝트

- **[DCN-V2와 행동 시퀀스 인코더를 활용한 CTR 예측](https://github.com/junhyung-L/ctr-sequence-modeling):** DCN-V2에 DIN·DIEN·BST 시퀀스 인코더를 붙여 비교했습니다. DIEN 검증 PR-AUC 0.0792(무작위 대비 약 4배), ROC-AUC 0.7413.
- **[신용카드 고객 세그먼트 분류](https://github.com/junhyung-L/credit-card-customer-segmentation):** 학습 240만 행·857개 컬럼의 결측 패턴별 처리와 CatBoost·스태킹을 비교했습니다. DACON private 0.6251(58위·상위 25%), 내부 표본 weighted F1 0.8936(다수 클래스 기준 0.7026).
- **[중고 전기차 가격 예측](https://github.com/junhyung-L/used-ev-price-forecasting):** 배터리 용량 대체 모델과 XGBoost 가격 회귀를 분리했습니다. DACON 리더보드 정규화 RMSE 0.919.
- **[Job Simulator AI](https://github.com/junhyung-L/ai-interview-simulator):** 2026년 제1회 KEG 바이브코딩 콘테스트에서 8일 동안 개발. Next.js로 면접·고객 응대·영업 역할극과 피드백 API를 만들고, 실제 LLM 경로와 API 키 없는 데모 경로를 분리했습니다.

## 수상

| 대회 · 상격 · 날짜 | 프로젝트와 역할 |
|---|---|
| 2025 PBL 프로그램 · **대상**(인천광역시장상) · 2026.02.27 | [동인천 원도심 상권 마케팅 파일럿](https://github.com/junhyung-L/dongincheon-marketing-pilot): Marketing & Data Analysis 역할로 공실 데이터와 상인 인터뷰를 실행 과제로 정리하고 30일 매장 파일럿 운영 |
| 2025 인천대학교 산학 캡스톤디자인 경진대회 · **금상** · 2025.07.01 | [인천 e음 캐시백 정책 시뮬레이션](https://github.com/junhyung-L/incheon-eeum-policy-simulation): 4인 팀 팀장, 예산 2,000억 원 안의 캐시백 일정 66개 비교 |
| 2024 임업통계 스마트활용 경진대회 · **대상**(산림청장상) · 2024.12.13 | [산림 작물 적합지·생산량 분석](https://github.com/junhyung-L/forestry-crop-suitability): GIS 토양 레이어·기후·생산 데이터와 작물별 분류·회귀 모델 |

상장 사본은 요청 시 제공합니다.

## 학력

- **산업경영공학 학사(우등졸업)** | 인천대학교, 2024.03–2026.02 (편입)
- **산업경영공학과 재학** | 국립한국교통대학교, 2020.03–2023.12 (인천대학교 편입)

## 기술

- **모델링:** Python, PyTorch, scikit-learn, XGBoost, LightGBM, CatBoost, statsmodels, SHAP
- **데이터·공간:** Pandas, SQL, PostgreSQL, BigQuery, Dask, GeoPandas
- **앱·시각화:** Next.js, Tableau
- **관심 분야:** Machine Learning, RecSys, GIS, Causal Inference, XAI

## 자격증

Google Data Analytics Professional Certificate · ADsP · SQLD · 빅데이터분석기사
