<div align="center">

# 🏡 Rural Housing Matching Analysis

### 귀농인 유형별 빈집 주거지 매칭 데이터 분석

<img src="https://img.shields.io/badge/K--means-Clustering-F2C14E?style=flat-square"/>
<img src="https://img.shields.io/badge/AHP-MCDM-E45756?style=flat-square"/>
<img src="https://img.shields.io/badge/TOPSIS-MCDM-72B7B2?style=flat-square"/>
<img src="https://img.shields.io/badge/Tableau-Visualization-E97627?style=flat-square&logo=tableau&logoColor=white"/>

</div>

---

## 📌 Overview

농촌 빈집 증가와 귀농인의 주거 정보 부족 문제를 연결하여,  
**생활·농업 인프라와 귀농인 유형을 기반으로 적합한 빈집을 추천하는 데이터 분석 프로젝트**입니다.

분석 대상은 **경상남도, 경상북도, 전라남도, 전라북도**이며,  
빈집 주변 인프라를 정량화해 유사한 지역을 군집화하고 귀농인 유형별 추천 주거지를 도출했습니다.

---

## 🔍 Analysis Process
  
빈집·인프라 데이터 수집   
        ↓  
빈집↔ 인프라 거리 계산    
        ↓    
인프라 만족도 점수 산출    
        ↓   
K-means Clustering    
        ↓    
AHP 기반 유형별 가중치 설정     
        ↓    
TOPSIS 기반 유형-Cluster 매칭    
        ↓   
유형별 Top 10 빈집 선정   
        ↓    
Tableau Dashboard 제작  

## 🧩 Key Methods

### 1. Infrastructure Scoring
- 빈집과 생활·농업 인프라 간 거리를 계산
- 시그모이드 함수와 가중치 감쇠를 적용해 접근성을 정량화
- 동일 인프라는 가까운 시설부터 최대 5개까지 반영

### 2. K-means Clustering
- 17개 인프라 항목을 6개 요인으로 재구성
- Standard Scaling 적용
- Elbow Method를 통해 4개 군집으로 분류

### 3. AHP + TOPSIS
- 귀농인 유형별 인프라 중요도를 AHP로 가중치화
- TOPSIS를 활용해 귀농 유형과 적합 Cluster를 매칭
- Cluster 내 개별 빈집을 평가해 유형별 Top 10 후보 도출

---

## 👥 Farmer Types

| Type | Description |
|---|---|
| 🌱 청년창농형 | 농업 창업을 목표로 귀농 |
| 👴 은퇴생계형 | 은퇴 후 독립적인 생활을 위해 귀농 |
| 👨‍👩‍👧 가족정착형 | 가족 단위 정착을 목표로 귀농 |
| 🌾 영농상속형 | 부모 또는 가족의 농업을 물려받기 위해 귀농 |

### Matching Result

- **청년창농형** → 농업특화지역
- **은퇴생계형** → 인프라 우수지역
- **가족정착형** → 인프라 우수지역
- **영농상속형** → 인프라 우수지역

---

## 📊 Result

- 귀농인 유형별 **Top 10 빈집 후보** 도출
- 최종 상위 후보지가 **경상북도와 전라북도에 집중**
- 분석 대상 지역 간 **인프라 편차** 확인
- Tableau 대시보드를 통해  
  `귀농 유형 → 지역 → 빈집 → 인프라 수준` 탐색 가능
- 지역별 특산물 정보까지 연계해 귀농 준비 단계의 의사결정 지원

---

## 👤 My Contribution

### Multi-Criteria Decision Making
- 귀농인 유형별 인프라 중요도 설계
- AHP 기반 가중치 적용
- TOPSIS 기반 귀농 유형–Cluster 매칭
- 유형별 Top 10 빈집 도출

### Dashboard
- Tableau 기반 대시보드 제작
- 귀농 유형 및 지역 필터 구현
- 빈집별 인프라 만족도 시각화
- 지역별 특산물 조회 기능 구현

---

## 💡 Insight

> 단순히 빈집이 많은 지역을 추천하는 것이 아니라,  
> **귀농인의 정착 목적과 주변 인프라를 함께 고려해야  
> 실제 활용 가능한 주거지 추천이 가능하다.**
