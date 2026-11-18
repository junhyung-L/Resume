# Junhyung Lee | Data Scientist

[한국어](README.md)

[jun010914@inu.ac.kr](mailto:jun010914@inu.ac.kr) · [GitHub](https://github.com/junhyung-L) · [LinkedIn](https://www.linkedin.com/in/junhyung-lee-data) · [Portfolio](https://github.com/junhyung-L/Portfolio)

## Profile

I build prediction models and decision simulations from customer, policy, and spatial data. For each result I state the data, the evaluation setting, and what it does and does not show.

## Experience

- **Intern** | BigData&AI Cell, Hana Financial Convergence Technology Institute, 13 Jul 2026–present
- **Undergraduate Researcher** | [DIVE Lab](https://github.com/thekimk/DIVE-Research), Incheon National University, Feb 2025–Feb 2026 — first author of the conversion-prediction paper below; follow-up causal-inference study on marketing-fatigue effects in progress

## Research

### [Purchase Conversion Prediction with Dynamic Marketing Knowledge](https://github.com/junhyung-L/crm-conversion-prediction) | First author, *마케팅연구* (Korean Marketing Association), forthcoming Nov 2026

- Designed four groups of time-varying features (purchase cycle, temporal response, marketing fatigue, channel effectiveness) on 172 million REES46 CRM messages (about 1.85 million customers, 1,907 campaigns, 0.1234% conversion) and compared nine models.
- XGBoost had the best F1 (0.3806) and PR-AUC (0.3620) on the original-distribution holdout and lifted recall from 0.3074 to 0.5230. The top 0.78% of messages captured 95.83% of conversions (precision 15.26%, 123.7x lift over random).

## Projects

- **[CTR Prediction with DCN-V2 and Behavior-Sequence Encoders](https://github.com/junhyung-L/ctr-sequence-modeling):** compared DIN, DIEN, and BST sequence encoders on a DCN-V2 backbone. DIEN validation PR-AUC 0.0792 (about 4x random), ROC-AUC 0.7413.
- **[Credit-Card Customer Segment Classification](https://github.com/junhyung-L/credit-card-customer-segmentation):** compared missingness-aware CatBoost and stacking over 2,400,000 training rows and 857 columns. DACON private 0.6251 (58th, top 25%); internal-sample weighted F1 0.8936 vs 0.7026 majority baseline.
- **[Used-EV Price Prediction](https://github.com/junhyung-L/used-ev-price-forecasting):** separated a battery-capacity imputation model from XGBoost price regression. DACON leaderboard normalized RMSE 0.919.
- **[Job Simulator AI](https://github.com/junhyung-L/ai-interview-simulator):** built Next.js roleplay and feedback APIs for interview, customer-support, and sales practice, with separate live-LLM and keyless demo paths.

## Awards

| Competition · Award · Date | Project and role |
|---|---|
| 2025 PBL Program · **Grand Prize** (Incheon Metropolitan City Mayor's Award) · 27 Feb 2026 | [Dong-Incheon Marketing Pilot](https://github.com/junhyung-L/dongincheon-marketing-pilot): Marketing & Data Analysis role; turned vacancy data and merchant interviews into action items and ran a 30-day store pilot |
| 2025 Incheon National University Industry-Academic Capstone Design Competition · **Gold Prize** · 1 Jul 2025 | [Incheon e-Eum Cashback Policy Simulation](https://github.com/junhyung-L/incheon-eeum-policy-simulation): team lead of four; compared 66 cashback schedules within a KRW 200 billion budget |
| 2024 Forestry Statistics Smart Use Competition · **Grand Prize** (Korea Forest Service Commissioner Award) · 13 Dec 2024 | [Forestry Crop Suitability and Yield Analysis](https://github.com/junhyung-L/forestry-crop-suitability): GIS soil layers, climate, and production data with per-crop classification and regression models |

Award certificates are available on request.

## Education

- **B.S. with honors, Industrial & Management Engineering** | Incheon National University, Mar 2024–Feb 2026 (transfer)
- **Industrial & Management Engineering (transferred out)** | Korea National University of Transportation, Mar 2020–Dec 2023

## Skills

- **Modeling:** Python, PyTorch, scikit-learn, XGBoost, LightGBM, CatBoost, statsmodels, SHAP
- **Data & spatial:** Pandas, SQL, PostgreSQL, BigQuery, Dask, GeoPandas
- **Apps & visualization:** Next.js, Tableau
- **Focus:** Machine Learning, RecSys, GIS, Causal Inference, XAI

## Certifications

Google Data Analytics Professional Certificate · ADsP · SQLD · Big Data Analysis Engineer
