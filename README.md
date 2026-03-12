<div align="center">

<br/>

# Minji · 민지

**AI PL / AI Service Engineer**

*현장의 신호 속에서 문제의 패턴을 읽어내는 개발자.*
*방대한 운영 데이터를 정밀하게 들여다보며 시스템의 병목을 해결하는 데이터 기반의 엔지니어.*

<br/>

[![Gmail](https://img.shields.io/badge/mminguuu7@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:mminguuu7@gmail.com)
[![GitHub](https://img.shields.io/badge/@mminguu-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/mminguu)

</div>

---

## 🛠 Tech Stack

**Language & Data**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

**ML / DL**

![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-189fdd?style=flat-square&logoColor=white)

**Computer Vision**

![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![CLIP](https://img.shields.io/badge/CLIP_(OpenAI)-412991?style=flat-square&logo=openai&logoColor=white)

**LLM / RAG**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-F5A623?style=flat-square&logoColor=white)
![vLLM](https://img.shields.io/badge/vLLM-6E40C9?style=flat-square&logoColor=white)

**Infra & Tools**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## 📂 Projects

### 🔬 [FTOGuard — 특허·디자인 침해 리스크 판단 AI 서비스](https://github.com/mminguu/SKN20-FINAL-2TEAM)
> `Computer Vision` `Deep Learning` `RAG` `LangGraph` `vLLM` `RunPod`

FTO(Freedom-To-Operate) 조사에 평균 2주 이상, 수백만 원이 소요되는 문제를 해결하기 위한 AI 의사결정 보조 서비스.
사용자가 제품 이미지를 업로드하면 KIPRIS 특허 DB에서 유사 디자인을 자동 검색하고, VLM이 침해 리스크를 분석해 최종 FTO 리포트를 생성.

- **데이터 파이프라인**: KIPRIS API → XML 파싱 → Canny Edge Detection 전처리 → ChromaDB 적재, 최종 **21,829개** 고품질 임베딩 확보
- **Embedding Collapse 탐지**: 전체 쌍의 79.3%가 유사도 0.7 이상임을 수치로 증명 → Triplet Loss 기반 CLIP 파인튜닝으로 개선
- **시스템 아키텍처**: RunPod Serverless에 sLLM 2개(Qwen2.5-14B+QLoRA, Qwen2.5-VL-7B) vLLM 서빙, LangGraph `interrupt()`로 Human-in-the-loop 구현
- **인프라**: AWS EC2 · S3 · RDS, Docker, FastAPI

---

### 🤖 [청년이음 — 청년·1인 가구 생활복지 지원 챗봇](https://github.com/mminguu/SKN20-3rd-1TEAM)
> `RAG` `LangChain` `Django` `ChromaDB` `BM25` `GPT-4o-mini`

복잡한 정부 지원 정책 속에서 개인 맞춤 혜택을 빠르게 찾아주는 RAG 기반 챗봇.

- **백엔드 설계**: Django 앱 구조 체계화, Policy 모델 33개 필드 설계, RESTful `/search/` API 구현
- **검색 파이프라인**: BM25(40%) + Vector Search(60%) Ensemble Retriever → RRF Fusion → RegionFilter 후처리
- **데이터 파이프라인**: 온통청년 Open API 수집, 의미 단위 청킹, 3,550개 문서 임베딩

---

### 📉 [Customer Churn Prediction — 고객 이탈 예측](https://github.com/mminguu/SKN20-2nd-3TEAM)
> `Machine Learning` `XGBoost` `EDA` `GridSearchCV`

통신 서비스 고객의 이탈 가능성을 예측하여 전략적 인사이트를 제공하는 ML 프로젝트.

- Logistic Regression · Decision Tree · Random Forest · XGBoost · LightGBM 5개 모델 비교
- K-Fold CV + GridSearchCV 튜닝 → **XGBoost 최종 선정**
- Feature Importance: 계약 기간(Contract), 월 요금(MonthlyCharges)이 이탈 핵심 변수로 도출

---

### 🚗 [Vehicle Registration & FAQ System](https://github.com/mminguu/SKN20-1ST-1TEAM)
> `Python` `Pandas` `Streamlit`

자동차 등록 현황 및 기업 FAQ 조회 시스템.

---

## 📊 GitHub Stats

<div align="center">

![Minji's GitHub Stats](https://github-readme-stats.vercel.app/api?username=mminguu&show_icons=true&theme=default&hide_border=true&title_color=222222&text_color=555555&icon_color=888888&bg_color=ffffff)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=mminguu&layout=compact&hide_border=true&title_color=222222&text_color=555555&bg_color=ffffff)

</div>

---

## 🌱 Currently Learning

`LLM Fine-tuning` &nbsp;·&nbsp; `Agentic RAG` &nbsp;·&nbsp; `MLOps` &nbsp;·&nbsp; `AI Service Engineering`

---

<div align="center">
<sub>Seoul-based · data-driven · always learning 🤍</sub>
</div>
