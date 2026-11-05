# Tomás Oriol Freixa

**Data Scientist** | Machine Learning · Time series forecasting · Python · SQL

- 🌍 San Sebastián, Spain
- ✉️ tomas20oriol@gmail.com
- 🎓 Master's in Data Analysis in Engineering @ Tecnun (2026–2027)
- 🎓 Industrial Engineering & Management @ Tecnun (2026)
- 📊 Applied Data Science Program @ Zrive (2026)

---

I'm an Industrial Management engineer starting my career in data science. I'm currently
doing the Master's in Data Analysis in Engineering at Tecnun.

What I enjoy most is the part that comes before the model: understanding the problem well
and what the prediction is going to be used for. In the projects I've done so far I've
learned that it pays to start with something simple, validate carefully, and ask a lot of
questions to the people who know the day-to-day.

I work mostly with Python, machine learning and time series forecasting, and more recently
with cloud platforms and AI agents. I'm still learning.

I finish the master's in June 2027 and would like to join a data team then. If you'd like
to talk, write to me.

---

## Projects

**[Predicting myopia in medical students](https://github.com/tomas20oriol-jpg/miopia-ml-project)** · *Machine Learning course project, Tecnun*
Four classification targets (myopia, myopia magna and two multi-class versions) on 132 students,
where only 18 have myopia magna, so always answering "no" already gets 86% accuracy and finds
nobody. I set the validation scheme and the rule for accepting a model before comparing any:
repeated stratified cross-validation, nested for tuned models, and a candidate replaced the simple
baseline only if it beat it fold by fold. Logistic regression on axial length alone turned out
to be a strong baseline. XGBoost won on myopia magna (balanced accuracy 0.90, 83% of the cases
found) and the axial length / corneal radius ratio, taken from the literature, helped on the other
targets. I also repeated the whole selection inside the folds to measure how optimistic the scores
are, and reported that the gain disappears on one target. Built with scikit-learn and XGBoost, with
unit tests.

**[Customer segmentation and retention](https://github.com/tomas20oriol-jpg/customer-segmentation-retention)** · *Online Retail II (UCI)*
Two years of orders from a UK online giftware retailer. I cleaned the data (duplicates,
cancellations matched to their sales, non-product charges), grouped customers into four
segments with K-Means, studied retention by cohort and the time to a second order with
survival analysis, and built a churn model validated over time. A logistic regression stayed
as the final model because gradient boosting did not beat it under a rule set beforehand.
Each result comes with its limitations, and the report has recommendations per segment.

**[Predicting electric vehicle purchases](https://github.com/tomas20oriol-jpg/ev-purchase-prediction)** · *Kaggle Playground Series S6E9*
Binary classification on 668k customers. A logistic regression baseline (ROC-AUC 0.938) set
the bar; every later candidate was compared with it fold by fold and only accepted if the
gain was consistent. Final ensemble of LightGBM, XGBoost, CatBoost and HistGradientBoosting:
ROC-AUC 0.946 in cross-validation and on the leaderboard. Everything fitted on data lives
inside an sklearn Pipeline, so there is no leakage, and the repo includes unit tests.

**[Tecnun Study Coach](https://github.com/tomas20oriol-jpg/tecnun-study-coach)** · *Microsoft Foundry agent*
A chat assistant for a university data science course. The course information is spread over
several PDFs (syllabus, lab schedule, grading rubric), so finding a deadline or working out the
grade needed in the remaining labs takes time, and there is no direct way to report a broken
dataset. The assistant answers from the course documents and cites the source, does the grade
calculations with code instead of estimating them, and opens a GitHub issue for the teaching staff
when a student reports a problem. It never hands over full solutions to graded labs. Built as an
agent in Microsoft Foundry with Azure AI Search over the course PDFs, Code Interpreter and MCP
connections to Microsoft Learn and GitHub, plus a Python client for terminal and web.

**Short-term traffic demand forecasting** · *final degree project, Aleatica · graded 10/10*
72-hour forecasts of toll plaza demand to plan staffing. Seven model families — SARIMA,
SARIMAX, XGBoost, LightGBM, LSTM, Temporal Fusion Transformer and Prophet — plus hybrids and
a stacking ensemble, compared under a single walk-forward protocol. Best result: MAE 90.0,
R² 0.85 (+20% over the baseline), lifting staffing allocation accuracy from 41% to 65%.
For production I recommended the best single model instead: it trains in about 20 minutes
rather than 3–4 hours, and the operations team can read its forecast.
*(Private repository: contains operator data.)*

**[Applied Data Science Program](https://github.com/tomas20oriol-jpg/zrive-ds)** · *Zrive*
Push-notification targeting for a groceries app on 2.8M rows: temporal splits to prevent
leakage, linear and gradient boosting models benchmarked on the same features, probability
calibration, and the pipeline packaged as tested Python modules.

**Production plant digitalisation** · *Alumigraf*
Data structuring in SAP and Power BI dashboards used daily by management to replace
paper-based reporting. *(Private: internal company systems.)*

**Maintenance work order analysis** · *JG Ingenieros*
Statistical analysis of 140k+ maintenance work orders (2017–2023) to find usage patterns
and areas for improvement, written up as an article.

---

## What I work with

**Code** — Python (pandas, Polars, scikit-learn, statsmodels, matplotlib) · SQL / SQL Server · R

**Modelling** — LightGBM · XGBoost · CatBoost · Prophet · LSTM · Temporal Fusion Transformer

**Cloud & AI** — Microsoft Azure (AI Search, Entra ID) · Microsoft Foundry · Microsoft Fabric · AWS (EC2, S3, CloudWatch) · AI agents · RAG · MCP

**Tools** — Git · Poetry · Power BI · SAP Business One · Excel

**Areas** — Statistics & probability · Machine Learning · Time series forecasting · Deep Learning

---

## Let's connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/tomás-oriol-freixa-750762285/)
