#### Metadata 
-   `Title:`ย [[= EAG - Data Analysis]]
-   `Type:`ย [[=]]
-   `Tags:` #๐ง ๏ธ/๐๏ธ/๐ฑ๏ธ 
-   `Formation Date:`ย [[2023-02-01]]
---

# EAG - Data Analysis
>The data was colleced following the [[= Knee - biomechanics]].  After collection, the data was anlysed following a multi-stageinductive analysis of the data.

The results of each stage are available below:



# Data processing
 - Env: ํ์ด์ฐธ, AWS(ID: sense0906@gmail.com / PW: )
 - code(setting.py & main.py) ์คํ
 - ์ธก์ ์์.txt์์ ๊ฐ ๋์ ํ์ธ
 - GUI ์ฌ์ฉ
	 - ๋ฅ๋์ ์  =   leg stretch(1) (7-14)
	 - ์๋์ ์  (์์ ๊ตด๊ณกํฌํจ) = leg bend(2) (by each angle) (28-35)
	 - ์ค์ฟผํธ = squat (14-21)
	 - ํ์คํธ์ถ์ถ(Win + Shift + T) & paste to ์์ํ์ผ
	 - 

์ค์ฟผํธ (14-21) squat


# Stage 3
# Stage 2

# Stage 1 Interpretation of signals by components
## stage 1.1 Analysis of initial & end noise potentials

## stage 1.2 Analysis of Signal reversal


# Stage 0 Analysis of amplitude
## stage 0.1 Analysis of Maximal diff.

### Potential values versus movement 
  - whole data look-up
  - raw data ๋ถ์์์ move๋ณ boxplot ๊ฒน์ณ๊ทธ๋ฆฌ๊ธฐ
  - outlier - ์ ๊ฑฐ ์ฝ๋์ฌ์ฉ 1.5 IQR  ์ฌ์ฉํ๊ธฐ์๋ ๋ง์ด ํ๋ ๊ฐ ๋จผ์  ์ ๊ฑฐ

### Potential values versus channel in same movments

### Absolute value versus movement
  - AP ๋ฐ์ดํฐ์์ move ๋ณ boxplot ๊ฒน์ณ๊ทธ๋ฆฌ๊ธฐ
  - raw data & AP ๋ฐ์ดํฐ์์ ๊ฐ move๋ณ๋ก channel ๋ค์ ์ ์ํ ์ฐจ์ด ํต๊ณ
  - absolute & outlier ์ ๊ฑฐ ์ฝ๋(ํ์ฌ ์๋ฌ๋จ) ๋ก๋ ๊ตฌํด๋ณด๋ ๊ฒ ์ข์

### Propotional values versus movement

### Absolute & propotional values versus movement


## stage 0.2 Analysis of Hypothetical diff.


# Previous findings
1.  Flexion - extension ์ผ๋ก ์ธํ ์ ์ ๋ณํ  
    : ๋ฌด๋ฆ๊ฐ๋๊ฐ 90๋์์๋ ์์น, ์์ ์ ์ (0๋), ์์ ๊ตด๊ณก(130~150)์์๋ ํ๊ฐํ๋ ๊ฒฝํฅ์ฑ, ์์นํ๋ ๊ฒฝ์ฐ, ์ฆ signal reversal ์ด ๋๋ ๊ฒฝ์ฐ์ ํ์ ํ์ - ์ ๋๊ฐ์ด ํต๊ณ์  ์ ์ฌ์ฑ์ด ๋ ํฌ๋ค๋ฉด ์ ํธ์ญ์ ์ ๋ฐฉํฅ์ ๋ฌธ์ ์ผ ์ ์๋ค.(์์ธก ๊ฒฝ๊ณจ์ฐ๊ณจ์ค์ ๋์ฑ ๋ถํ๋ฅผ ๋ง์ด(=์ ํธ๋ฅผ๋ง์ด) ๋ด๋ ์ฐ๊ณจ์ด ๋ค๋ฅธ ๊ฒฝ์ฐ์ ๊ฐ๋ฅ์ฑ?  
    : ๋งค์ฐ ํฐ๊ฐ์ผ๋ก ๊ด์ฐฐ๋๋ ๊ฒฝ์ฐ ์์  
    : ๋ฅ๋์ ์ ๊ณผ ์๋์ ์ ์์ ํฌ๊ธฐ ์ฐจ์ด๋ฅผ ๋ณด์ด๋ ๊ฒฝ์ฐ ์์. - 2๋ฒ๊ณผ ์ฐ๊ด์ฑ  
    : 2๋ฒ์ ๋ฐ์๊ณผ 3๋ฒ์ ์งํ ์ฌ์ด์์ ์์ํ๊ฒ ๊ฐ๋๋ณํ๋ง์ ๋ํ๋ด๋ ์ ์?
2.  Flexion - extension ์ ์์ํ๊ณ  ๋ง์น ๋ ์๊ธฐ๋  
    :๋์ฒด์ ์ผ๋ก positive(upward) ๋ฐฉํฅ์ ์ ์์์น - ๊ธ๊ฒฉํ fluid ์ด๋?
3.  ๋ฑ์ฅ์ฑ ์์ถ์ (์ค๋ ฅ ๋ถํ์๋ํ ์์ธ์ ์ง์)์ด ์ ์ ๋ณํ: ๋์ฒด์ ์ผ๋ก ์ ์ง์ ์ธ ํ๊ฐ(ํ๋ฐฉ์ผ์์์๋ ์ ์ง์  ์์น), 1๋ฒ๊ณผ 3๋ฒ์ฌ์ด๋ฅผ ๋๋๋ point labeling & 2๋ฒ์ ์ํฅ๋ถ์?  
    : ์ค์ฟผํธ๋ ์ ํ์ฒด ๊ทผ์ก, ๋ฅ๋์ ์ ์ ๋ํด์๊ทผ์ก๋ง ์์ถํ๋ ๊ฒ์ ๋ฐ๋ฅธ ์ฐจ์ด?  
    : ์ค์ฟผํธ์์ ๋ฐ์ํ๋ fibrillar pattern noise


๐LINKS TO THIS PAGE
[[& EAG by knee movement - draft]]