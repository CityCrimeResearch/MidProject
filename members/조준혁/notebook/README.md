# 🧠 프로젝트명:  서울에서 마계에 가장 어울리는 동네는 어디일까? 


## 📌 개요 (Overview)
본 프로젝트는 서울특별시 25개 자치구를 대상으로, 범죄 발생률과 사회적 불안 요인(1인 가구, 외국인 비율, 학업중단율 등) 간의 상관관계를 분석하고, 이를 바탕으로 ‘마계’에 가까운 위험 자치구를 도출하는 것을 목적으로 합니다.

- 분석 단위: 2023년 기준 서울시 자치구

- 중점 변수: 구조적 요인(1인 가구, 외국인), 교육 요인(학업중단율), 사회참여, 정서적 요인, 실업률 등

- 목표: 단순 범죄 건수 중심의 위험 판단을 넘어서 사회 구조적 위험 요소와 범죄의 상관성을 해석

---
## 🙋‍♀️ 팀원

| 팀원 | 역할 |
|------|------|
| 강민경 | 팀리더 |
| 조준혁 | SM |
| 이관형 | 발표자 |
| 안효빈 | 발표자료제작 |

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

- 태블로 시각화를 통한 추세선 분석 및
- 히트맵을 통한 상관관계 분석
  
5. 시각화 및 인사이트 도출

- 변수별 범죄율과의 관계를 직관적으로 표현

- Tableau 기반 시각화 자료를 통해 인사이트 전달

---

## 📊 주요 결과 요약
- 외국인 비율, 실업률, 1인 가구 비율은 **범죄율과 유의미한 양의 상관관계**를 보임
- Tableau 대시보드를 통해 자치구별 위험도 직관적으로 확인 가능
---


- GitHub: [🔗 바로가기](https://github.com/CityCrimeResearch/MidProject)  
