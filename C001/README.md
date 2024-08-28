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

## 1-1. 연구주제 및 연구목적

<div align="center">
  
<h3> "UIG 심층수송량 분석 및 예측을 통한 기후온난화 심각성 재고"
<br>
(In-depth Analysis and prediction of UIG Transport Volumes for Assessing the Severity of Climate Change) </h3>

<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/ee2f75a2-1535-4dbd-8d14-9029544327cc"> <img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/20229b8d-678e-4024-a3d9-6e30d39b120e">
</div>

✅ 해양은 기상과 밀접한 상호작용을 지닌다. 상단 좌측 그림 빨간 동그라미에 속하는 '동해(East Sea)'는 대한민국 한반도 인근 바다에 비해 좁은 면적을 차지해 상대적으로 순환속도가 빠르다. 따라서 동해는 '대양의 미래 모습을 예측할 수 있는 자연실험실'로 불린다. 또한, '동해(East Sea)'는 북한한류와 동한난류가 만나는 지점으로 해류의 영향을 연구하는 데 의미가 깊다고 할 수 있다. 
<br>
<br>
✅ 동해에 위치한 UIG(Uleung Interplain Gap)란 '울릉해저간극'으로 상단 우측 그림 빨간 동그라미를 의미하며, 울릉도와 독도 사이의 심해통로이다. 프로젝트의 주 목적은 <b>UIG(울릉해저간극) 데이터를 사용해 남향 수송량 추세를 파악 및 예측(prophet 시계열 모델 활용)하고, 이를 근거로 지구 온난화 및 해양 생태계 문제의 심각성을 파악</b>하는 데 있다.
<br>
<br>
✅ 2002년부터 2004년까지 측정된 약 3년치의 Western UIG(U1-U3) 및 Eastern UIG(U4-U5)의 유속(Ur, cm/s) 데이터, 그리고 longitude()와 depth(m) 두 특성 데이터를 활용해 얻은 해저 지형 단면적 데이터를 기반으로 <b>수송량(Sv) 데이터를 산출</b>한다.
<br>
<br>
✅ 산출된 3년치의 수송량 데이터와 유속 데이터 간의 상관관계를 조사한 뒤, 1996년부터 2020년까지의 U3 남향 수송량 데이터를 활용해 prophet 모델링을 진행해 <b>약 24년 치의 U3 남향 수송량 데이터 및 추세</b>를 산출한다.
<br>
<br>
✅ 최종적으로, 주어진 각종 해양 관련 데이터와 외부 해양 오픈 데이터(정점 U3 깊이별 수온 데이터, 울릉도 조위관측소 수온/기온 OpenAPI), 그리고 산출해 낸 수송량 데이터와 추세 결과를 종합해 <b>데이터와 실제 지구 해양 환경 문제와의 연관성을 파이썬 시각화 결과물로 입증하고, 미래의 기후온난화 심각성</b>을 논하고자 한다.

## 1-2. 선행연구

✅ 1990년부터 2013년까지 해류 운동에너지가 10년마다 대략 15% 정도 증가한다. (Source[▶️](https://blog.naver.com/with_msip/222416428048))
<br>
<br>
✅ 지구온난화로 인해 해류속도가 빨라지고 있다. (Source[▶️](https://www.science.org/content/article/global-warming-speeding-ocean-currents-here-s-why))
<br>
<br>
✅ 북극 빙하는 빠른 속도로 녹고 있다. (Source[▶️](https://www.bbc.com/korean/international-56924659))
<br>
<br>
✅ 계절별로 동해 심층순환 방향 세기가 달라진다. (Source[▶️](https://www.riss.kr/search/detail/DetailView.do?p_mat_type=be54d9b8bc7cdb09&control_no=6db94c4e3b927f97ffe0bdc3ef48d419&outLink=K))
<br>
<br>
✅ 최근 10년간 북한한류의 수온이 약 0.1도 감소하는 추이를 보이며, 이는 한류의 영향 증가로 추론할 수 있다. (Source[▶️](chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://www.jkosmee.or.kr/xml/12089/12089.pdf))
<br>
<br>
✅ 북한한류계수의 영향은 동계보다 하계에 더욱 우세하다. (Source[▶️](chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://www.jkosmee.or.kr/xml/12089/12089.pdf))
<br>
<br>
✅ 위도에 따른 열 불균형은 기온과 표층수의 온도 차이와 관련 있다. 이는 곧 해수의 순환에 영향을 준다. (Source[▶️](https://www.dbpia.co.kr/Journal/articleDetail?nodeId=NODE09037117))

## 1-3. 도메인 지식

<div align="center">

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/dc84f63f-76bf-40c3-b9b5-160d01f4ebe0">

</div>

✅ 상단 오른쪽 모식도 용어 설명(JB: 일본 분지, UB: 울릉 분지, YB: 야마토 분지 - 수심 2000m 이상의 깊고 평평한 해저 지형)
<br>
<br>
✅ 동해는 평균수심 1500m 이상 깊은 바다로 상단 왼쪽 그림과 같이 표층과 심층수가 교환되는 대류작용이 발생한다. 주로 동해 북부 내역에서 차가운 공기에 의해 표층수가 냉각되어 표층이 얼게 된다. 이후 표층에 염분이 방출되고 표층수의 밀도가 상승한다. 그 결과 동해 수심 1500m 깊은 곳까지 표층수가 가라앉게 된다. 가라앉은 이후 1500m 이상의 심층 해수 순환은 상단 오른쪽 그림처럼 동해의 해저지형 가장자리에 따라 크게 반시계방향으로 순환한다.

<div align="center">

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/99e2b1df-f219-4fac-9ffa-4b053ec2fd66">

</div>

✅ 해저지형 가장자리에 따른 반시계방향 순환은 상단 왼쪽 그림과 같이 울릉도에서 가까운 곳(U1, U2 부근)은 북쪽에서 남쪽으로 흘러 나오고, 독도에 가까운 곳(U4, U5 부근)은 남쪽에서 북쪽으로 흘러 나간다.
<br>
<br>
✅ 상단 오른쪽 그림은 남쪽에서 북쪽을 바라본 방향에서의 그림으로, Western UIG(U1, U2, U3)는 북쪽에서 남쪽으로 흐르는 방향 우세, Eastern UIG(U4~U5)는 남쪽에서 북쪽으로 흐르는 방향이 우세하다.



## 1-4. 가설 설정
<div align="center"> <h3>
"북한한류계수의 영향력이 점점 커질 것으로 추정되며, western UIG 분기별 심층 수송량은 해가 지남에 따라 변화폭이 점점 커지는 방향으로 증가할 것이다."
</div> </h3>

## 1-4. 분석 데이터 소개

✅ 지정 데이터셋
- 2002년부터 2004년까지의 Western UIG(U1, U2, U3) 유속 데이터
- 1996년부터 2020년까지의 U3(EC1) 유속 데이터
- U1, U2, U3, U4, U5 각 지점 위도/경도 및 UIG 지형 깊이에 따른 경도 데이터

<br>

✅ 외부 데이터셋
- 1996년부터 2020년까지의 U3(EC1) 깊이별 수온 데이터 (SEANOE) (Source[▶️](https://www.seanoe.org/data/00677/78916/))
- 2012년부터 2020년까지의 울릉도 조위관측소 Open API (수온 Open API ([▶️](http://www.khoa.go.kr/oceangrid/khoa/takepart/openapi/openApiObsTempTideRealDataInfo.do)) / 기온 Open API ([▶️](http://www.khoa.go.kr/oceangrid/khoa/takepart/openapi/openApiObsAtempTideRealDataInfo.do)))

# 2. 데이터 분석

## 2-1. Western UIG 심층 수송량 계산


## 2-2. 유속과 Western UIG 심층 수송량과의 상관관계 산출

## 2-3. Western UIG 심층 수송량 장기 추세 산출

## 2-4. Prophet 모델을 사용한 Western UIG 심층 수송량 예측 Trend 산출 및 모델 검증

## 2-5. U3 1500m 심층수온 Trend & 표층수온과 기온 차이 Trend 산출




# 3. 분석 결과


## 3-1. 프로젝트 기대 효과


# 4. 결론 및 참고문헌

✅ "Deep flow and transport through the UIG in Southwestern East Sea"

- 수송량 계산 과정 참고
- UB, JB 분지 위치 및 지형 참고
- UIG 해류흐름 및 방향 참고
- 수송량 단위 참고

<br>

✅ "동해 연안(울릉분지)의 최근 10년간 해양변화"

- 북한한류계수(NKCW), 대마난류계수(TC) 특성 참고

<br>

✅ "동해 심층순환의 계절변화에 대한 수치실험"

- 계절별 해류특성, 변화 참고
- 울릉도-독도 반시계방향 해류 내용 참고

<br>

✅ "한국 서해안 표층수 온도와 기온의 상관성 연구"

- 표층수 및 기온 경향성 참고
- 열 불균형과의 관계성 참고

<br>

✅ "동해 재분석 자료에 나타난 북한한류의 계절 및 경년변동성"

- 북한한류계수 남하경로 참고
- 북한한류 남하경향성 참고







