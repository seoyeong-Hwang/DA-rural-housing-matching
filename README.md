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
