#### Metadata 
-   `Title:` [[= EAG - Data Analysis]]
-   `Type:` [[=]]
-   `Tags:` #🧠️/📝️/🌱️ 
-   `Formation Date:` [[2023-02-01]]
---

# EAG - Data Analysis
>The data was colleced following the [[= Knee - biomechanics]].  After collection, the data was anlysed following a multi-stageinductive analysis of the data.

The results of each stage are available below:



# Data processing
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


# Stage 3
# Stage 2

# Stage 1 Interpretation of signals by components
## stage 1.1 Analysis of initial & end noise potentials

## stage 1.2 Analysis of Signal reversal


# Stage 0 Analysis of amplitude
## stage 0.1 Analysis of Maximal diff.

### Potential values versus movement 
  - whole data look-up
  - raw data 분석에서 move별 boxplot 겹쳐그리기
  - outlier - 제거 코드사용 1.5 IQR  사용하기에는 많이 튀는 값 먼저 제거

### Potential values versus channel in same movments

### Absolute value versus movement
  - AP 데이터에서 move 별 boxplot 겹쳐그리기
  - raw data & AP 데이터에서 각 move별로 channel 들의 유의한 차이 통계
  - absolute & outlier 제거 코드(현재 에러남) 로도 구해보는 것 좋을

### Propotional values versus movement

### Absolute & propotional values versus movement


## stage 0.2 Analysis of Hypothetical diff.


# Previous findings
1.  Flexion - extension 으로 인한 전위 변화  
    : 무릎각도가 90도에서는 상승, 완전신전(0도), 완전굴곡(130~150)에서는 하강하는 경향성, 상승하는 경우, 즉 signal reversal 이 되는 경우의 파악 필요 - 절대값이 통계적 유사성이 더 크다면 신호역전은 방향의 문제일 수 있다.(양측 경골연골중에 더욱 부하를 많이(=신호를많이) 내는 연골이 다른 경우의 가능성?  
    : 매우 큰값으로 관찰되는 경우 있음  
    : 능동신전과 수동신전에서 크기 차이를 보이는 경우 있음. - 2번과 연관성  
    : 2번의 발생과 3번의 진행 사이에서 순수하게 각도변화만을 나타내는 전위?
2.  Flexion - extension 을 시작하고 마칠때 생기는  
    :대체적으로 positive(upward) 방향의 전위상승 - 급격한 fluid 이동?
3.  등장성 수축시 (중력 부하에대한 자세유지시)이 전위 변화: 대체적으로 점진적인 하강(후방센서에서는 점진적 상승), 1번과 3번사이를 나누는 point labeling & 2번의 영향분석?  
    : 스쿼트는 전하체 근육, 능동신전은 대퇴앞근육만 수축하는 것에 따른 차이?  
    : 스쿼트에서 발생하는 fibrillar pattern noise


🔗LINKS TO THIS PAGE
[[& EAG by knee movement - draft]]