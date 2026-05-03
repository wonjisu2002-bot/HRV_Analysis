# HRV_Analysis
Analysis of HRV based on sleep, heart rate, and exercise data
_Apple Watch 데이터를 활용한 개인 생리 데이터 분석 프로젝트_

**## Summary**
수면, 심박수, 운동 데이터를 기반으로 
HRV(심박변이도)에 영향을 미치는 생리적 요인을 분석하였다. 

**## Data Explanation**
_(Apple watch 기반 측정 데이터)_
- HRV(심박변이도)
- 평균 심박수
- 운동 시간
- 수면 시간
- 수면 질

**## Data Preprocessing**
- 날짜 기준 데이터 정렬
- 하루 평균 HRV 계산
- 다음날 HRV 생성 (shift 적용)

**## Results**


### 1. 운동 강도별 HRV 변화 (다음날 기준)

<img width="557" height="500" alt="Image" src="https://github.com/user-attachments/assets/bb338b01-6d81-4869-a05f-f9e2bb500ba4" />


운동 초기에는 HRV 감소가 일부 관찰되었으며,
지속적 운동 단계에서는 회복 패턴이 안정되는 경향을 보였다.


### 2. 수면시간 vs 다음날 HRV

<img width="567" height="452" alt="Image" src="https://github.com/user-attachments/assets/739fe7aa-6bde-42bc-a991-a67f3f96cdff" />


수면 시간과 HRV 간에는 뚜렷한 상관관계가 나타나지 않았다. 


### 3. 수면 질 vs 다음날 HRV

<img width="567" height="452" alt="Image" src="https://github.com/user-attachments/assets/c80bb465-0a08-4a2d-9fcc-59c663f91e0d" />


수면 질이 높을수록 HRV가 증가하는 경향이 관찰되었다. 


### 4. 심박수(HR) vs HRV

<img width="567" height="452" alt="Image" src="https://github.com/user-attachments/assets/a663059a-0034-477d-a18f-23782978a20c" />


강한 음의 상관관계가 나타났으며 (r ≈ -0.74)
심박수가 증가할수록 HRV가 감소하는 경향을 보였다. 



**## Conclusion**

**운동 분석**에서는 단기적으로 HRV 감소가 나타날 수 있으나, 
지속적인 운동 수행 시 회복 능력이 향상되는 패턴이 관찰되었다. 

**수면 시간**은 HRV에 큰 영향을 미치지 않았으며, 
**수면 질**은 HRV와 약한 양의 상관관계를 보였다.

반면, **심박수**는 HRV와 강한 음의 상관관계를 나타냈으며,
HRV가 자율신경계 상태를 반영하는 지표임을 확인할 수 있었다.

=> **HRV**는 단일 요인이 아닌, **다양한 생리적 요소가 복합적으로 작용하는 지표**이다.
