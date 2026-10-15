<h1 align="center">Phan Thanh Tan</h1>

<p align="center">
  <b>Data Engineering & Machine Learning</b><br>
  Final-year Computer Science student at HCMUT · Ho Chi Minh City, Vietnam
</p>

<p align="center">
  <a href="https://portfolio-thanhtanphan.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://portfolio-thanhtanphan.netlify.app/Phan_Thanh_Tan_CV.pdf"><img src="https://img.shields.io/badge/CV-PDF-2a78d6?style=for-the-badge&logo=readthedocs&logoColor=white" alt="CV (PDF)"></a>
  <a href="https://www.linkedin.com/in/t%E1%BA%A5n-thanh-8906a6261/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:thanhtanphan011022@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

I build data pipelines and ML models end to end, and I report every result against a simple baseline with confidence intervals. I'm looking for a **Data Engineer, Data Analyst or Machine Learning internship**.

- **Baseline first.** Every model is compared with something simple: last week's demand, popularity, logistic regression.
- **Intervals, not single numbers.** Results come with bootstrap confidence intervals and a test set scored once.
- **Limitations written down.** Each README ends with what the project does not show.

## Featured projects

<table>
  <tr>
    <td width="40%"><a href="https://github.com/thanhtan2210/nyc-taxi-demand-forecasting"><img src="https://raw.githubusercontent.com/thanhtan2210/nyc-taxi-demand-forecasting/main/docs/images/map.png" alt="NYC taxi zone map from the Streamlit app"></a></td>
    <td>
      <h3><a href="https://github.com/thanhtan2210/nyc-taxi-demand-forecasting">NYC Taxi Demand Forecasting</a></h3>
      Next-hour pickups for 263 taxi zones from <b>376M</b> public TLC trip records (DuckDB star schema, one global XGBoost model).<br><br>
      <b>−40% MAE</b> against a same-hour-last-week baseline on three held-out months (WAPE 9.6–10.4% vs 16.1–17.6%).<br><br>
      <code>DuckDB</code> <code>SQL</code> <code>XGBoost</code> <code>Streamlit</code> <code>GitHub Actions</code><br><br>
      <a href="https://nyc-taxi-demand-forecasting-t.streamlit.app/">Live demo</a> · <a href="https://portfolio-thanhtanphan.netlify.app/work/nyc-taxi-demand-forecasting">Case study</a>
    </td>
  </tr>
  <tr>
    <td width="40%"><a href="https://github.com/thanhtan2210/realtime-sentiment-streaming"><img src="https://raw.githubusercontent.com/thanhtan2210/realtime-sentiment-streaming/main/docs/images/dashboard.png" alt="Airline sentiment dashboard replaying a recorded run"></a></td>
    <td>
      <h3><a href="https://github.com/thanhtan2210/realtime-sentiment-streaming">Airline Tweet Sentiment Stream</a></h3>
      Kafka → Spark Structured Streaming → MongoDB → Streamlit, with event-time windows, a watermark and deduplication.<br><br>
      Macro-F1 <b>0.711</b> [0.695, 0.728] vs 0.256 for always answering "negative"; stream predictions match the offline model on <b>4,196 / 4,196</b> tweets; <b>1,264.6 tweets/s</b> on a 2-vCPU GitHub runner.<br><br>
      <code>Kafka</code> <code>Spark</code> <code>MongoDB</code> <code>scikit-learn</code> <code>Docker</code>
    </td>
  </tr>
  <tr>
    <td width="40%"><a href="https://github.com/thanhtan2210/automl-churn-prediction"><img src="https://raw.githubusercontent.com/thanhtan2210/automl-churn-prediction/main/docs/images/05_customer_detail.png" alt="Churn Predictor customer detail panel with the reasons behind a risk score"></a></td>
    <td>
      <h3><a href="https://github.com/thanhtan2210/automl-churn-prediction">Churn Predictor: Leakage Audit and Rebuild</a></h3>
      An old pipeline reported ROC-AUC <b>0.999</b>. I traced it to three leaking columns and SMOTE before cross-validation, then rebuilt it with a leakage-checking profiler and an app that explains each customer's risk.<br><br>
      Clean IBM Telco test ROC-AUC <b>0.859</b> [0.837, 0.879] vs 0.849 for logistic regression; UCI Iranian 0.988 vs 0.927.<br><br>
      <code>LightGBM</code> <code>Optuna</code> <code>scikit-learn</code> <code>FastAPI</code> <code>Next.js</code><br><br>
      <a href="https://portfolio-thanhtanphan.netlify.app/work/automl-churn-prediction">Case study</a>
    </td>
  </tr>
  <tr>
    <td width="40%"><a href="https://github.com/thanhtan2210/movie-recommender-mlops"><img src="https://raw.githubusercontent.com/thanhtan2210/movie-recommender-mlops/main/docs/images/mlflow_registry.png" alt="MLflow model registry with the champion alias"></a></td>
    <td>
      <h3><a href="https://github.com/thanhtan2210/movie-recommender-mlops">Movie Recommender MLOps</a></h3>
      Monthly retraining on MovieLens 25M with a promotion gate: a challenger replaces the champion only if it is better with 95% confidence.<br><br>
      HitRate@10 <b>27.7%</b> vs 22.4% for popularity on an untouched month (1,475 users); served by FastAPI in Docker at about 5 ms median.<br><br>
      <code>scikit-learn</code> <code>MLflow</code> <code>Cloudflare R2</code> <code>FastAPI</code> <code>Docker</code><br><br>
      <a href="https://portfolio-thanhtanphan.netlify.app/work/movie-recommender-mlops">Case study</a>
    </td>
  </tr>
  <tr>
    <td width="40%"><a href="https://github.com/thanhtan2210/flight-price-prediction"><img src="https://raw.githubusercontent.com/thanhtan2210/flight-price-prediction/main/docs/images/predict.png" alt="Flight price app assessing a quoted fare"></a></td>
    <td>
      <h3><a href="https://github.com/thanhtan2210/flight-price-prediction">Flight Price Prediction & Quote Assessment</a></h3>
      Is this fare cheap, fair or expensive? An XGBoost price model plus a calibrated 80% price range (conformalized quantile regression).<br><br>
      R² <b>0.872</b>, MAE 678 INR; the 80% range covers <b>78.8%</b> of test fares; one stop costs a median 3,038 INR more than non-stop (95% CI 964–4,410).<br><br>
      <code>pandas</code> <code>XGBoost</code> <code>Streamlit</code><br><br>
      <a href="https://flight-price-prediction-t.streamlit.app/">Live demo</a> · <a href="https://portfolio-thanhtanphan.netlify.app/work/flight-price-prediction">Case study</a>
    </td>
  </tr>
</table>

## Tools I use

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white" alt="SQL">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
</p>
<p>
  <img src="https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black" alt="DuckDB">
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas">
  <img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" alt="Apache Kafka">
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="Apache Spark">
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" alt="MongoDB">
  <img src="https://img.shields.io/badge/Cloudflare%20R2-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare R2">
</p>
<p>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn">
  <img src="https://img.shields.io/badge/XGBoost-337AB7?style=flat-square" alt="XGBoost">
  <img src="https://img.shields.io/badge/LightGBM-02569B?style=flat-square" alt="LightGBM">
  <img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white" alt="MLflow">
</p>
<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit">
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js">
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions">
</p>

## Experience and education

- **Backend Developer Intern**, MyTegami.win · May – Jul 2025 · AI generation workflow with Genkit, Gemini and Zod schemas (TypeScript)
- **B.Sc. Computer Science**, Ho Chi Minh City University of Technology (HCMUT) · Oct 2022 – Jun 2027 (expected) · major in Data Engineering and Big Data
