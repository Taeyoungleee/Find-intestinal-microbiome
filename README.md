# Find-intestinal-microbiome

[데이터 청년 캠퍼스](https://dataonair.or.kr/bigjob/)에서 진행한 심화 프로젝트
+ 2023.08.03 ~ 2023.08.28 기간동안 진행한 프로젝트  
+ 교수님의 코칭을 받아서 진행  
--------------------------------------------------------------------------------------------------------------------------------------------
## 데이터 설명
교수님이 연구하신 데이터를 받아서 진행  
쇼그렌 증후군 환자와 정상인의 박테리아 비율 데이터  
> ID  
> 박테리아 종류  
--------------------------------------------------------------------------------------------------------------------------------------------
## 분석 방법  
### 데이터 전처리  
1) tsv파일 처리: tsv형식의 파일을 읽어와 행과 열을 제대로 분리함  
2) genus level 처리: genus level의 박테리아 추출하기 위해 함수로 행 전처리  
3) 필요없는 행 처리: genus level이 없는 행 제거  

### 집단 간 비교분석 진행
Alpha diversity의 대표적인 방법으로 집단간 Shannon, Simpson 지수 확인  
-> 정상인 집단에 다양한 박테리아 종이 분포함을 확인  

Mann-Whitney 검정을 통해 유의미한 변수 추출  
-> 유의미한 변수와 전체변수를 활용해 다양한 시각화 진행  

Beta diversity 진행하여 시각화  
-> Alpha diversity 등고선에서 찾지못한 집단간 차이를 Beta 등고선에서 차이를 확인 할 수 있음  

--------------------------------------------------------------------------------------------------------------------------------------------
## 예측 모델 및 결과  
모델 평가지표로 f1-score 사용  
클래스간 개수 차이가 많이나 오버샘플링 통해 Data Imbalance 해결  
유의미한 변수만 사용해 모델 학습  
성능은 좋았으나 데이터가 매우 적어 신뢰하기엔 부족하다 판단  

모델의 Feature Importance 추출하여 인사이트 제공  

--------------------------------------------------------------------------------------------------------------------------------------------
## 결론
+ Feature Importance를 통해 나온 박테리아들의 정보를 수집  
+ 쇼그렌 증후군 환자의 외분비샘 기능 저하에 초점을 맞춰 외분비샘 기능을 향상 시켜주는 미생물 **부티르산**과 연결시킴  
+ Feature Importance를 통해 나온 박테리아들이 **부티르산**을 생성하는데 이로운지, 해로운지 구분  
  > 해당 박테리아가 부티르산에 어떤 영향을 주는지 논문을 통해 조사  
+ 해당 박테리아를 활용해 새로운 치료법 개발 및 식단 개발의 의의가 있었음  
