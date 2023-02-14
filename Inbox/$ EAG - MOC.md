  
-   `Title:` [[$ EAG - MOC]]
-   `Type:` [[$]]
-   `Tags:` #🧠️/📝️/🌞️ 
-   `organizer:`   
-   `meeting Date:` 
-   `Reviewed Date:` [[2023-02-11]]

This is the MOC about EAG; Electroarthrography

---
## 1. definition

EAG는 관절연골에서 발생하는 전위를 기록하는 것
임상에서 활용할 수 있다면 진단적 가치를 가질 수 있음


---
## 2.  # Background knowledge


## 2.0 Introductive factors
- From related work
	- Tibiofemoral cartilage loading 에 따라서 joint line 에서 연골전위가 측정된다. Cartilage 는 SGP - strain generated potential 을 만든다.
	
- 선행연구의 findings
	- 관절 각도의 변화에 따라 loading 이 없어도 전위 차가 발생한다.
		- 가설1: 수동 굴곡시에도 loading에 따른 strain 은 나타날 가능성
		- 가설검증: 
	- 관절연골은 세군데 있다.
	
		그 중 Articular cartilage 에서의 변화를 보려고 한다.
### 2.1 Related work
	선행연구는 3가지로 나뉠 수 있다.
	1. Buschmann et al. 의 메인 연구그룹의 논문들
	2. Elbow EAG에 대해 1가지 논문을 발표한 인도 그룹
	3. 예전 cartilage streaming potential 및 strain-generated potential 에 대한 최신연구들

### 2.1.1 Brief Summary 
	1. Buschmann 등의 연구
		1. OA 와 prosthetic knee 에서의 EAG 감소 및 소실
		2. TFL & GCM 등의 knee joint crossing muscle  들이 COG 의 변화에 따라 자세유지를 위해 수축하는 것과 관련
		3. 반복된 weight shift 에서 신호값이 줄어듦
		4. movement는 weight shift 사용 - 연골 부하 위치가 일정했을 것
		5. sensor point 는 joint line area - computer modeling하였음 - PF joint 의 정보는 없을 것

### 2.1.2 Significance

### 2.2 EAG potentials([[= EAG - potentials]])
    
### 2.3 synovial fluid

### 2.4 intra-articular pressure


---

## 3. Future work

### 3.1. Knowledge gap

- 선행연구에서 보고되지 않았던 관절각도변화에 따른 EAG 관찰
- 

Maximal differences for 7 sec

Amplitude difference from 90 ->180

The amplitude of potentials changes at active extension versus passive extension

Amplitude difference from 180-> 90

Loading on knee cartilage phase (knee extension 90->180 versus squat 180->90)

Immediate difference to the inflection point in 1sec

Correlation between ultrasonographic parameters versus EAG signals

신호역전의 원인 탐색(역전횟수탐색?)

각 센서의 비율의 비교 - 개인에 따른 비율로 변환, 각 위치에서 측정되는 신호혹은 2번 노이즈의 절대값 크기나 방향, 3번 신호의 방향이 대충 예상 가능할지,

3번 신호의 상승하강량 조사

신호 유사성의 비교 - 센서의 개수를 줄이거나, 위치를 추가할 수 있는 가능성

Outlier의 기준?

### 3.2 Target journal

1.  [https://www.clinbiomech.com/](https://www.clinbiomech.com/) IF 2.034 Clinical Biomechanics is an international multidisciplinary journal of biomechanics with a focus on medical and clinical applications of new knowledge in the field.The science of biomechanics helps explain the causes of cell, tissue, organ and body system disorders, and supports clinicians in the diagnosis, prognosis and evaluation of treatment methods and technologies. Clinical Biomechanics aims to strengthen the links between laboratory and clinic by publishing cutting-edge biomechanics research which helps to explain the causes of injury and disease, and which provides evidence contributing to improved clinical management. Clinical Biomechanics explores all facets of body system, organ, tissue and cell biomechanics, with an emphasis on medical and clinical applications of the basic science aspects. The role of basic science is therefore recognized in a medical or clinical context. The readership of the journal closely reflects its multi-disciplinary contents, being a balance of scientists, engineers and clinicians.
2.  [https://onlinelibrary.wiley.com/page/journal/1554527x/homepage/productinformation.html](https://onlinelibrary.wiley.com/page/journal/1554527x/homepage/productinformation.html) IF 3.102 The Journal of Orthopaedic Research, a publication of the Orthopaedic Research Society (ORS), is the forum for the rapid publication of high quality reports of new information on the full spectrum of orthopaedic research, including life sciences, engineering, translational, and clinical studies.
3.  [https://journals.lww.com/clinorthop/pages/default.aspx](https://journals.lww.com/clinorthop/pages/default.aspx) IF 4.755 Research articles providing the latest in basic biological or engineering research on musculoskeletal diseases.
---


## 4. Method

- 능동신전/수동신전/스쿼트 에서 무릎관절의 각도변화에 따른 EAG를 측정하고자 함.
- 8군데에서 측정함, 4군데는 patellar 주변의 retinaculum,  나머지는 joint line 을 따라서
- 명료화해야하는 부분
	- 수동신전에서도 연골변형이 생기는지 - 논문찾기
	- cartilage, loading area 로 부터, outer cartilage 및 surface 까지의 거리에 따른 전위의 크기 및 역전
	- Synovial fluid 의 영향

### 4.1. Data analysis ([[= EAG - Data Analysis]])

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