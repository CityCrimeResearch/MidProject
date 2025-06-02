# 🧠 프로젝트명:  서울에서 마계에 가장 어울리는 동네는 어디일까? 

## 📌 개요 (Overview)
서울시 자치구별 범죄 데이터를 바탕으로 다양한 사회적 지표와의 관계를 분석하고, 범죄 발생률이 높은 지역의 특성을 탐색

---

## 🎯 목적 (Objective)
- 범죄율에 영향을 미치는 사회적 요인을 분석
- 위험지역 예측 또는 정책적 인사이트 도출
- Tableau 및 Python을 활용한 시각적 스토리텔링

---

## 📂 사용 데이터 (Dataset)
| 출처 | 설명 |
|------|------|
| 공공데이터포털 | 자치구별 범죄 발생 건수 등 |
|  KOSIS국가통계포털 | 인구, 1인 가구, 소득, 외국인 비율 등 |
| 통계청 | 실업률, 주거취약지수 등 |

📁 `./data/raw/`에 원본 데이터, `./data/processed/`에 전처리된 데이터 포함

---

## 🛠️ 사용 기술 (Tech Stack)
- Python (pandas, numpy, seaborn, matplotlib, scikit-learn, scipy, statsmodels)
- Jupyter Notebook
- Tableau
- Git/GitHub

---

## 🔍 🔍 주요 분석 과정 (Pipeline)
1. 데이터 수집 및 정리

- 다양한 공개 데이터를 수집 (경찰청, 서울열린데이터광장 등)

- 컬럼 단위 통일, 결측치 및 이상치 처리

- 변수명 표준화 및 데이터 병합

2. 정규화 및 전처리

- 단위가 다른 변수 간 비교를 위해 MinMaxScaler로 정규화

- 해석을 위한 역정규화도 일부 변수에 적용 (ex. 봉사활동 등)

3. 탐색적 데이터 분석 (EDA)

- 변수 분포 및 기초 통계량 확인

- seaborn, matplotlib을 활용한 시각적 패턴 탐색

4. 상관관계 분석

- spearmanr, pearsonr 등 통계 기법을 활용한 변수 간 관계 분석

- statsmodels를 활용하여 회귀선 시각화 및 회귀계수 해석

5. 시각화 및 인사이트 도출

- 변수별 범죄율과의 관계를 직관적으로 표현

- Tableau 또는 Python 기반 시각화 자료를 통해 인사이트 전달

---

## 📊 주요 결과 요약
- 외국인 비율, 실업률, 1인 가구 비율은 **범죄율과 유의미한 양의 상관관계**를 보임
- 범죄율이 높은 지역은 **중심지 접근성** 및 **야간 유동인구**와도 관련 있음
- Tableau 대시보드를 통해 자치구별 위험도 직관적으로 확인 가능

---

## 🔗 프로젝트 결과 링크
- Tableau 대시보드: [🔗 바로가기](https://public.tableau.com/views/example_dashboard)
- 블로그 정리글: [🔗 바로가기](https://velog.io/@username/crime-analysis)

---

## 🙋‍♀️ 팀원

| 팀원 | 역할 |
|------|------|
| 강민경 | 팀리더 |
| 조준혁 | SM |
| 이관형 | 발표자 |
| 안효빈 | 발표자료제작 |

- GitHub: [🔗 바로가기](https://github.com/CityCrimeResearch/MidProject)  
