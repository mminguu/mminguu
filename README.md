![header](https://capsule-render.vercel.app/api?type=waving&color=0:FF9A9E,100:FAD0C4&height=250&section=header&text=Hello,%20I'm%20Minji%20&fontSize=70&fontColor=ffffff&desc=AI%20PL%20·%20AI%20Agentic%20Engineering&descSize=22&descAlignY=75&animation=twinkling)

<div align="center">

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 280">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0f2942"/>
      <stop offset="50%" style="stop-color:#1a6b8a"/>
      <stop offset="100%" style="stop-color:#0abfbc"/>
    </linearGradient>
  </defs>

  <rect width="900" height="280" fill="url(#bg)" rx="12"/>

  <path d="M0,200 C150,170 300,230 450,200 C600,170 750,210 900,190 L900,280 L0,280 Z" fill="#0a1f35" opacity="0.85"/>
  <path d="M0,220 C120,200 280,245 450,220 C620,195 780,235 900,215 L900,280 L0,280 Z" fill="#071525" opacity="0.6"/>

  <text x="450" y="115" font-family="'Segoe UI', Arial, sans-serif" font-size="70" font-weight="800"
    fill="white" text-anchor="middle" letter-spacing="-1">✨ Welcome to Minji Land</text>

  <text x="450" y="115" font-family="'Segoe UI', Arial, sans-serif" font-size="65" font-weight="800"
    fill="white" text-anchor="middle" letter-spacing="-1">"AI와 데이터가 함께 어울려 노는 공간입니다."</text>

  <text x="450" y="115" font-family="'Segoe UI', Arial, sans-serif" font-size="65" font-weight="800"
    fill="white" text-anchor="middle" letter-spacing="-1">"복잡한 데이터의 미로를 지나 효율적인 시스템이라는 성을 짓고자 합니다."</text>
</svg>

</div>

---

## ✨ About the Owner

> **"현장의 신호 속에서 문제의 패턴을 읽어내는 개발자"**

> **"방대한 운영 데이터를 정밀하게 들여다보며 시스템의 병목을 해결하는 데이터 기반의 엔지니어"**

- 🏡 **Base**: Seoul
- 🔍 **Mission**: 복잡한 데이터 속 패턴을 찾아 AI 서비스라는 짜릿한 경험으로 연결합니다.
- 🔧 **Expertise**: End-to-End 파이프라인 설계부터 LLM 서비스 배포까지, 파크의 모든 설비를 직접 구축하고자 합니다.

---

## 🍿 Souvenir Shop (Tech Stack)

**Language & Data**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

**ML / DL & Vision**
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) ![CLIP](https://img.shields.io/badge/CLIP_(OpenAI)-412991?style=flat-square&logo=openai&logoColor=white)

**LLM / RAG & Infra**
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)

---

## 🎢 어트랙션 (Projects)

### 🎠 [FTOGuard — 특허·디자인 침해 리스크 판단 AI 서비스](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN20-FINAL-2TEAM)
> `Computer Vision` `Deep Learning` `RAG` `LangGraph` `vLLM` `RunPod`

FTO(Freedom-To-Operate) 조사에 평균 2주 이상, 수백만 원이 소요되는 문제를 해결하기 위한 AI 의사결정 보조 서비스.
사용자가 제품 이미지를 업로드하면 KIPRIS 특허 DB에서 유사 디자인을 자동 검색하고, VLM이 침해 리스크를 분석해 최종 FTO 리포트를 생성.

- **데이터 파이프라인**: KIPRIS API → XML 파싱 → Canny Edge Detection 전처리 → ChromaDB 적재, 최종 **21,829개** 고품질 임베딩 확보
- **Embedding Collapse 탐지**: 전체 쌍의 79.3%가 유사도 0.7 이상임을 수치로 증명 → Triplet Loss 기반 CLIP 파인튜닝으로 개선
- **시스템 아키텍처**: RunPod Serverless에 sLLM 2개(Qwen2.5-14B+QLoRA, Qwen2.5-VL-7B) vLLM 서빙, LangGraph `interrupt()`로 Human-in-the-loop 구현
- **인프라**: AWS EC2 · S3 · RDS, Docker, FastAPI

---

### 🤖 [청년이음 — 청년·1인 가구 생활복지 지원 챗봇](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN20-4th-1TEAM)
> `RAG` `LangChain` `Django` `ChromaDB` `BM25` `GPT-4o-mini`

복잡한 정부 지원 정책 속에서 개인 맞춤 혜택을 빠르게 찾아주는 RAG 기반 챗봇.

- **백엔드 설계**: Django 앱 구조 체계화, Policy 모델 33개 필드 설계, RESTful `/search/` API 구현
- **검색 파이프라인**: BM25(40%) + Vector Search(60%) Ensemble Retriever → RRF Fusion → RegionFilter 후처리
- **데이터 파이프라인**: 온통청년 Open API 수집, 의미 단위 청킹, 3,550개 문서 임베딩

---

### ⛲️ [Customer Churn Prediction — 고객 이탈 예측](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN20-2nd-3TEAM)
> `Machine Learning` `XGBoost` `EDA` `GridSearchCV`

통신 서비스 고객의 이탈 가능성을 예측하여 전략적 인사이트를 제공하는 ML 프로젝트.

- Logistic Regression · Decision Tree · Random Forest · XGBoost · LightGBM 5개 모델 비교
- K-Fold CV + GridSearchCV 튜닝 → **XGBoost 최종 선정**
- Feature Importance: 계약 기간(Contract), 월 요금(MonthlyCharges)이 이탈 핵심 변수로 도출

---

### 🚗 [Vehicle Registration & FAQ System](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN20-1ST-1TEAM)
> `Python` `Pandas` `Streamlit`

자동차 등록 현황 및 기업 FAQ 조회 시스템.


---

## 🎫 Fast Pass (Currently Learning)

| 구역 | 운영 계획 |
|------|------|
| **LLM Zone** | sLLM Fine-tuning (QLoRA) & Multimodal LLM 마스터 중 |
| **Agent City** | LangGraph를 이용한 고도화된 Multi-agent 협업 설계 |
| **Data Factory** | 대용량 데이터 수집 및 Vector DB 최적화 파이프라인 확장 |
| **Cloud Square** | vLLM & MLOps를 활용한 끊김 없는 서비스 배포 환경 구축 |
| **Core Dev** | 견고한 시스템: 예외 처리 강화 및 지수 백오프 기반의 재시도 로직을 통한 데이터 파이프라인 신뢰성 확보 |

---

<div align="center"  font-size="70" font-weight="800">
🎡 <b>Minji Land</b>는 연중무휴 성장 중입니다! <br/>
<sub>Seoul-based · Data-driven Adventure · Always Learning 🤍</sub>
</div>
