This is the MOC about EAG; Electroarthrography

---
## ==1. definition

EAG는 관절연골에서 발생하는 전위를 기록하는 것
임상에서 활용할 수 있다면 진단적 가치를 가질 수 있음

---
## ==2. Related work

선행연구는 3가지로 나뉠 수 있다.

	1. Buschmann et al. 의 메인 연구그룹의 논문들
	2. Elbow EAG에 대해 1가지 논문을 발표한 인도 그룹
	3. 예전 cartilage streaming potential 및 strain-generated potential 에 대한 최신연구들

### 2.1 Brief Summary 
	1. Buschmann 등의 연구
		1. OA 와 prosthetic knee 에서의 EAG 감소 및 소실
		2. TFL & GCM 등의 knee joint crossing muscle  들이 COG 의 변화에 따라 자세유지를 위해 수축하는 것과 관련
		3. 반복된 weight shift 에서 신호값이 줄어듦
		4. movement는 weight shift 사용 - 연골 부하 위치가 일정했을 것
		5. sensor point 는 joint line area - computer modeling하였음 - PF joint 의 정보는 없을 것

### 2.2. Significance
---

## ==3. Future work

- 선행연구에서 보고되지 않았던 관절각도변화에 따른 EAG 관찰
- 


---

## ==4. Method

- 능동신전/수동신전/스쿼트 에서 무릎관절의 각도변화에 따른 EAG를 측정하고자 함.
- 8군데에서 측정함, 4군데는 patellar 주변의 retinaculum,  나머지는 joint line 을 따라서
- 명료화해야하는 부분
	- 수동신전에서도 연골변형이 생기는지 - 논문찾기
	- cartilage, loading area 로 부터, outer cartilage 및 surface 까지의 거리에 따른 전위의 크기 및 역전
	- Synovial fluid 의 영향

### ==4.1. Data analysis

#### Data processing
 - Env: 파이참, AWS(ID: sense0906@gmail.com / PW: )
 - code(setting.py & main.py) 실행
 - 측정순서.txt에서 각 동작 확인
 - GUI 사용
	 - 능동신전 =   leg stretch(1) (7-14)
	 - 수동신전 (완전굴곡포함) = leg bend(2) (by each angle) (28-35)
	 - 스쿼트 = squat (14-21)
	 - 텍스트추출(Win + Shift + T) & paste to 엑셀파일
	 - 

스쿼트 (14-21) squat


#### Statistical analysis

-   raw data 분석에서 move별 boxplot 겹쳐그리기
-   absolute & outlier 제거 코드(현재 에러남) 로도 구해보는 것 좋을
-   AP 데이터에서 move 별 boxplot 겹쳐그리기
-   raw data & AP 데이터에서 각 move별로 channel 들의 유의한 차이 통계