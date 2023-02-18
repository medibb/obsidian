-   `Title:` [[$ EAG by knee movement and loading - MOC]]
-   `Type:` [[$]]
-   `Tags:` #🧠️/📝️/🌞️ 
-   `organizer:`   
-   `meeting Date:` 
-   `Reviewed Date:` [[2023-02-11]]

This is the MOC about EAG by knee movement and loading

---
## 1. definition

EAG는 관절연골에서 발생하는 전위를 기록하는 것

임상에서 활용할 수 있다면 진단적 가치를 가질 수 있음

knee movment 는 다리펴기 / 스쿼트 에 해당하는 두가지 가장 흔한 운동 동작


### 1.1 Objectives
knee EAG가 무릎 운동에서 어떻게 측정되는 지 평가하고자 함.
이를 위해 최적의 센서 위치를 찾고 
운동 중 각도 변화에 따른 EAG 값의 변화를 측정하며,



---
## 2.  # Background knowledge


## 2.0 Introductive factors
- From related work: 기존 연구는 3가지로 나뉠 수 있다.
	1. Buschmann et al. 의 메인 연구그룹의 논문들
		1. OA 와 prosthetic knee 에서의 EAG 감소 및 소실보고
		2. TFL & GCM 등의 knee joint crossing muscle  들이 COG 의 변화에 따라 자세유지를 위해 수축하는 것과 관련
		3. 반복된 weight shift 에서 신호값이 줄어듦
		4. movement는 weight shift 사용 - 연골 부하 위치가 일정했을 것
		5. sensor point 는 joint line area - computer modeling하였음 - PF joint 의 정보는 없을 것
	2. Elbow EAG에 대해 1가지 논문을 발표한 인도 그룹
	3. 예전 cartilage streaming potential 및 strain-generated potential 에 대한 최신연구들
	- Tibiofemoral cartilage loading 에 따라서 joint line 에서 연골전위가 측정된다. Cartilage 는 SGP - strain generated potential 을 만든다.

- 관절전도 전위의 크기, 방향에 대하여
	- 관절 전도의 크기는 Buschmann  논문에서  0.25mv 로 관찰되었으며, 퍼듀대학 의공학 교실[bobb2022](babbsOriginElectroarthrogramStreaming) 에서 수학적 모델링으로 0.175mv일 것으로 예상했다.
	- 내부의 electrostatic potential 로 diapole 이 형성되어서 해당 전위를 외부에서 측정하는 것으로 해석하고 모델링 하였다.
	- ![[babbsOriginElectroarthrogramStreaming#img]]

- 무릎의 biokinematics에 대하여 
	- 관절연골은 세군데 있다.
		- 슬개골(무릎 뼈) 연골 : Patellar cartilage 
		- 대퇴골 연골 ( 좌 / 우)
		- 경골 연골 (좌 / 우)
	- 관절은 두군데서 일어난다
		- 대퇴 - 슬개 관절
		- 대퇴 - 경골 관절
		  
	- 다리펴기 (leg extension, Q-setting)
		- 대퇴사두근의 수축으로 대퇴사두골에 포함되어 있는 슬개골연골이 대퇴골 연골을 누르면서 rolling contact 를 하게 되면서 미끄러져 올라가고 경골이 따라 올라옴
		- 주로 대퇴-슬개 관절에 부하가 많이 걸리며, quadriceps muscles 이 약하면 부하가 더 많이 걸리고, full extension 에서 부하가 제일 많이 생긴다.
		  
	- 스쿼트
		- 무릎이 앞으로 나가는 경우와 나가지 않는 경우의 차이가 존재 - 무릎 앞을 물체로 차단하는 방법도 있다.
		- 무릎이 많이 나가지 않으면, 즉 발목이 많이 굴곡되지 않으면, 앉는 깊이에 따라 즉 무릎의 굴곡각도에 따라 loading 이 증가함
		- 주로 대퇴-경골 관절의 부하가 일어남
- 
	- 수동관절운동에서도 연골부하는 일어난다
		- 근육의 activation(motor unit firing)은 없어도, 근육과 그외 연조직은 viscoelastic tissue 이므로 lengthening & shortening 에 의한 tension이 발생
			- muscle intringic tension 및 수동굴곡시 loading 에 대한 ==기존 문헌조사==
			- 선행연구의 finding 인 관절 각도의 변화에 따른 전위 차가 발생에 대한 설명
		- 가설1: 수동 굴곡시에도 loading에 따른 strain 은 나타날 가능성
		- 수동굴곡 / 능동굴곡 / 스쿼트에 걸리는 strain값은?


### 2.1 Related work
- Buschmann et al. 등의 EAG 연구
- Knee kinetics 와 biomechanis 연구
	- loading 의 크기와 위치에 대한 배경지식으로 가설 정립
- EMG, EEG 등 bioelectric potential 관련 연구
	- biologic tissue 들의 신체 표면으로 전도되는 것에 관련된 연구
	- Streaming potential 등 기존 cartilage potential 에 대한 연구
		- EAG potentials([[= EAG - potentials]])
- 그 외 synovial fluid or intra-articular pressure 의 작용

---

## 3. Future work

### 3.1. Knowledge gap

- 기존 연구에서 보고되지 않았던 운동에 따른, 즉 관절부하 + 관절각도변화에 따른 EAG 변화를 관찰한다.
- 무릎 관절연골에서 발생하고 활액과 무릎 주변 연조직을 통해 표면전극 까지 전달되는 전위는 사전 연구에서 보고하는 streaming potential 이외의 요소들이 많이 작용할 것이다.
- 특히 운동 중에는 표면 전극과 내부 연골 사이의 상대적인 위치가 지속적으로 변화하므로, EAG측정의 특징이 달라질 것이다.
	- 가설1 : 표면전극으로 부터 연골의 상대적 위치 변화가 제일 적은 위치에서는 연골의 부하에 따른 전위를 가장 일관되게 보여줄 수 있다.
	- 가설 2: 상대적위치가 변하지만, 운동의 진행을 잘 알려주는 위치를 특정할 수 있다.
- 능동신전에서 부하가 가해진 연골의 전위는 수동신전에서 관절각도 변화와 그에 따른 수동적인 부하만 있는 연골보다 더 큰 전위 변화를 일으킬 것이다.
	- 하지만 관절의 운동중에 발생하는 복합적인 관절연골 접촉면의 이동과 전극과의 상대거리 변화는 관찰에 어려움을 만들 수 있다.
	- 관절연골의 deformation이 unloading 이후에도 사라지지 않는다면 electrostatic potential 이 남아있을 수 있겠지만, 기존연구와 선행연구에서 모두 unloading 과함께 즉시 potential 이 사라지는 것이 관찰됨
		- unloading 과 함께 cartilage ECM에서 convection 되었던 Na 등 cation 들이 즉시 이동되면서 electrostatic field 가 없어진다고 해석해야함.
		- cartilage 높이가 줄어든다는 내용은 국소적인 deformation이 지속된다기 보다 cartilage 자체에서 fluid 가 빠져나가는 것으로 해석할 수 있겠다.
	  ![[poillotStraingeneratedElectricalPotential2021#^ab5369]]

- 일단 수동관절운동과 능동관절운동의 차이가 있는 지 확인해보자
	- 가설 3: 수동과 능동 관절 각도변화는 EAG 차이가 있다. 추가로 각도 변화를 EAG를 통해 측정할 수 있다. 접촉면의 rolling 과 그에 따른 전위의 변화

- EAG를 streaming potential 의 측정에 국한하지 않고, joint motion에 따른 knee joint의 electric potential 을 모두 평가하는 큰범위에서의 EAG로 이야기 할 수 있음
	- 이렇다면, early OA 의 평가에 국한되지 않을 수 있다.
	- digital goniometer로서의 활용, 무릎의 굴곡 mechanism 의 문제의 발견, patellar gliding 에 대한 평가를 시행할 수 있다.
		- 다만 가설과 근거를 robust 하게 만들어야함
	- 실제 관절각도 변화에 따른 전위 변화는 SGP로 발생가능한 크기에 비해 매우 크다.
		- 가설 4: 자세를 유지하는 동안의 적은량의 전위변화가 SGP 가능성
		- 관절운동에 따른 변화는 또 다른 mechanotransduction 이 일어나는 것일 수도 있다. - synovial fluid의 이동?
		- 
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