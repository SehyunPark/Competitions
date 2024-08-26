<div align="center", class="contest">
  
![header](https://capsule-render.vercel.app/api?type=wave&color=52F9F4&text=2nd%20JOISS%20Ocean%20Science%20BigData%20Contest&fontSize=40&fontColor=011B65&height=200)

| Category | Description |
| :--------: | :-----------: |
| Contest Title | 2nd JOISS Ocean Science BigData Contest |
| Contest Date | 2022/08/16 ~ 2022/11/22 |
| Contest Details | SEALAB Home Page[▶️](http://sealab.kr/contest) <br> Participation Certificate[▶️](https://github.com/SehyunPark/Projects/blob/main/C001/Pariticipation_Certificate.pdf)|
| Team Name | HyunDuo |
| Contest Submissions | Code(python)[▶️](https://github.com/SehyunPark/Projects/blob/main/C001/Submission_Code(Python).ipynb) <br> Code(python) Packages List(Version included)[▶️](https://github.com/SehyunPark/Projects/blob/main/C001/Submission_Packages_List.txt) <br> Presentation Slides[▶️](https://github.com/SehyunPark/Projects) |
| Contest Result | 일반부 우수상(Second Prize)[▶️](https://github.com/SehyunPark/Projects/blob/main/C001/Award_Certificate.png) <br> Leaderboard[▶️](http://sealab.kr/contest/awards) |
| Media Coverage | News Coverage[▶️](https://www.sedaily.com/NewsView/26F0IMRJAK) <br> Contest Review - YouTube[▶️](https://www.youtube.com/watch?v=GW1l5pFcMxI) |

</div>

# 1. 연구주제 및 가설 설정

## 1-1. 연구주제

<div align="center">
  
<b> "UIG 심층수송량 분석 및 예측을 통한 기후온난화 심각성 재고" </b>

</div>

## 1-2. 연구목적
<div align="center">
<img width="600" height = "600" alt="image" src="https://github.com/user-attachments/assets/68149543-515a-47ff-ae67-44fe99475a26">
</div>

- 해양은 기상과 밀접한 상호작용을 지닌다. 특히 상단 그림과 같이 빨간 동그라미에 속하는 '동해(East Sea)'는 '대양의 미래 모습을 예측할 수 있는 자연실험실'로, 다른 인근 바다에 비해 상대적으로 순환속도가 빠르다. 또한, '동해(East Sea)'는 북한한류와 동한난류가 만나는 지점



# 2. 데이터 분석

# 3. 분석 결과

# 4. 결론 및 참고문헌




<div align="center">

<b> "In-depth Analysis and Prediction of UIG Transport Volumes for Assessing the Severity of Climate Change" </b>
<img width="811" alt="image" src="https://github.com/user-attachments/assets/dc84f63f-76bf-40c3-b9b5-160d01f4ebe0">

</div>

- 상단 오른쪽 모식도 용어 설명(JB: 일본 분지, UB: 울릉 분지, YB: 야마토 분지 - 수심 2000m 이상의 깊고 평평한 해저 지형)
- 동해는 평균수심 1500m 이상 깊은 바다로 표층과 심층수가 교환되는 대류작용이 발생한다. 주로 동해 북부 내역에서 차가운 공기에 의해 표층수가 냉각되어 표층이 얼게 된다. 이후 표층에 염분이 방출되고 표층수의 밀도가 상승한다. 그 결과 동해 수심 1500m 깊은 곳까지 표층수가 가라앉게 된다. 가라앉은 이후 1500m 이상의 심층 해수 순환은 상단 오른쪽 모식도처럼 동해의 해저지형 가장자리에 따라 크게 반시계방향으로 순환한다.

<div align="center">

<img width="811" alt="image" src="https://github.com/user-attachments/assets/99e2b1df-f219-4fac-9ffa-4b053ec2fd66">

</div>

- 해저지형 가장자리에 따른 반시계방향 순환은 상단 왼쪽 그림과 같이 울릉도에서 가까운 곳(U1, U2 부근)은 북쪽에서 남쪽으로 흘러 나오고, 독도에 가까운 곳(U4, U5 부근)은 남쪽에서 북쪽으로 흘러 나간다.
- 상단 오른쪽 그림은 남쪽에서 북쪽을 바라본 방향에서의 그림으로, Western UIG(U1, U2, U3)는 북쪽에서 남쪽으로 흐르는 방향 우세, Eastern UIG(U4~U5)는 남쪽에서 북쪽으로 흐르는 방향이 우세하다.

## Data Explanation

- 지정 DataSet

  - 자료 1: 2002년 ~ 2004년 정점 U1 ~ U5 까지의 데이터
    - Sheet 1: Longitude 130.9302143인 Depth 0부터(상단 오른쪽 그림 왼쪽 울릉도 부근) Longitude 131.87인 Depth 0(상단 오른쪽 그림 오른쪽 독도 부근)까지 Longitude에 따른 Depth 자료
    - Sheet 2: U1 ~ U5 지점 각각의 Longitude와 Latitude
    - Sheet 3 ~ 11: U1a, U1b, U2a, U2b, U3a, U3b, U4a, U4b, U5a 각 지점에의 2002년 ~ 2004년 시간별 지정위치 유속(Ur Current Speed) (단위 cm/s)
  
  - 자료 2: 1996년 ~ 2020년 정점 U3에서의 데이터
    - U3의 수심 1800m에서의 유속 데이터(1996년 11월 4일 22시 ~ 2020년 11월 11일 7시)

- 외부 DataSet
  - 자료 1: 1996년 ~ 2020년 정점 U3(EC1)의 깊이별 수온 데이터(SEANOE) ([Source](https://www.seanoe.org/data/00677/78916/))
  - 자료 2: 2012년 ~ 2020년 울릉도 조위관측소

    - 수온 OpenAPI(바다누리해양정보서비스) ([Source](http://www.khoa.go.kr/oceangrid/khoa/takepart/openapi/openApiObsTempTideRealDataInfo.do))
    - 기온 OpenAPI(바다누리해양정보서비스) ([Source](http://www.khoa.go.kr/oceangrid/khoa/takepart/openapi/openApiObsAtempTideRealDataInfo.do))

## Data Analysis

### 1. 연구주제 및 가설설정

### 2. 데이터 분석

### 3. 분석결과



## Results



## Conclusion












