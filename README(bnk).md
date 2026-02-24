# 전세계 행복 지수 (2015 ~ 2024) EDA

## Kaggle Dataset
* **2015 ~ 2019**: https://www.kaggle.com/datasets/unsdsn/world-happiness
* **2020 ~ 2024**: https://www.kaggle.com/datasets/samithsachidanandan/world-happiness-report-2020-2024

---

## 팀원

| GitHub | dhksrlghd | rusidian | nobrain711     | imseunghyeon264 | ParkMinseon22 | ch3477-sudo |
|-------|-------|-------|---------|-------|-------|-------|
| Profile | @dhksrlghd | @rusidian | @nobrain711 | @limseunghyeon264 | @ParkMinseon22 | @ch3477-sudo |
| Name | 홍원기 | 장한재 | 조동휘     | 임승현 | 박민선 | 윤찬호 |

---

## 개발 규칙
### 변수 네이밍
- 변수: `snake_case`
- 클래스: `PascalCase`
- 상수: `UPPER_CASE`
- DataFrame: `_df`
  > 예: user_df, sample_df

---

###  폴더 구조
```
project/
|
├─── data/              
├─── HongWanGi          
├─── JangHanJae         
├─── JoDongHwi          
├─── LimSeungHyeon      
├─── ParkMinSeon        
├─── YunChanHo          
├─── requirements.txt   
├─── LICENSE            
├─── .gitignore
└─── README.md
```
> 파이참 프로젝트를 프로젝트 폴더의 루트 경로로 열어서 작업해 주세요.   
> 개인 작업 공간에는 `md`와쥬피터 노트북만 있게 끔 해주세요.

---
## git

### git commit type
- feat: 새로운 기능
- fix: 버그 수정
- chore: 설정 변경
- docs: 문서 수정
- refactor: 코드 구조 개선 (기능 변경 없음)


### 커밋 메시지 작성 규칙

본 프로젝트는 Conventional Commits 규칙을 따릅니다.

- 커밋 제목(head)은 반드시 영어로 작성합니다.
- 커밋 타입은 소문자(feat, fix, chore, docs, refactor 등)를 사용합니다.
- 제목은 72자 이내로 간결하게 작성합니다.
- 필요할 경우 커밋 본문(body)에 한국어 설명을 추가할 수 있습니다.
- 이슈가 있는 경우 커밋 메시지에 이슈 번호를 함께 명시합니다. (예: #12)

#### 작성 형식

<type>(scope): 간단한 요약

예시:
```git

git commit -m "docs(README): add project rules

 - 팀 프로젝트 규칙을 README에 정리함

Refs: #0"
```

---

### Issue 작성 규칙

본 프로젝트에서는 개발을 시작하기 전에  
반드시 작업 내용을 Issue로 먼저 작성합니다.

Issue는 작업의 목적과 범위를 명확히 하기 위한 용도이며,  
커밋 및 PR은 해당 Issue를 기준으로 연결합니다.

Issue 작성자는 기본적으로 Author를 작성합니다.  
Assignee는 무조건 지정한다.

#### 양식
```markdown
## 작업 내용
- 무엇을 할 것인지 간단히 설명

## 목적
- 이 작업이 왜 필요한지

## 완료 기준
- [ ] 어떤 상태가 되면 완료인지

Author: @github_name
```
---

### Pull Request
PR을 하시기 전에 무조건 `sync`를 진행한 이후에 요청을 보냅니다.   
또한 PR 중에서 파일이 겹치는 경우에는 PR을 요청하지 마세요.

---

## Requirements

### Core (Data Handling)

- **numpy** — version 1.26 or higher  
- **pandas** — version 2.1 or higher  

---

### Visualization

- **matplotlib** — version 3.8 or higher  
- **seaborn** — version 0.13 or higher  

---

###  Statistics & Scientific Computing

- **scipy** — version 1.11 or higher  

---

### Geospatial Analysis

- **geopandas** — version 0.14 or higher  
- **shapely** — version 2.0 or higher  
- **pyproj** — version 3.6 or higher  
- **fiona** — version 1.9 or higher  

---
### Machine Learning

- **scikit-learn** — version 1.4 or higher  

---

### Notebook Environment

- **jupyterlab** — version 4.1 or higher  
- **ipykernel** — version 6.29 or higher  
- **ipython** — version 8.20 or higher  

---

## pip installation
### Using pip
```bash
pip install -r requirements.txt
```

---

### Using conda
```bash
conda create -n eda_env python=3.12
conda activate eda_env
conda install geopandas
pip install -r requirements.txt
```