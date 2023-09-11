1. 제출파일 목록
  1) README.txt : 코드 실행 방법 설명
  2) 01.Preprocessing.ipynb : 기본 raw 데이터로 시각화를 위한 데이터를 생성하는 파일
  3) 02.Visualization.ipynb : 전처리된 데이터로 여러 시각화를 해본 파일
  4) 03.Modeling.ipynb : 전처리된 데이터로 쇼그렌증후군 환자 분류모델을 돌려보는 파일
  5) table_lv7_rf_silva.tsv : 쇼그렌 환자 20명, 정상인 56명에 대한 otu id 데이터

2. Data 획득 방법
 -  01.Preprocessing.ipynb 를 실행시키면 df_genus_3 파일이 생성된다
 -  02.Visualization.ipynb 를 실행시키면 df2 파일과 significant_df.pkl 파일이 생성된다

3. 실행 필요 프로그램과 라이브러리
  1) python
  2) jupyter notebook 혹은 jupyter lab
  3) 코드 실행에 필요한 파이썬 라이브러리
     - sklearn
     - pandas
     - numpy
     - seaborn
     - matplotlib.pyplot
     - scikit-bio
    (scikit-bio 별도 설치 필요, 코드에 포함되어있음)

4. 실행방법
  1) 제출한 압축 파일의 압축을 푼다.
  2) 코드 파일(*.ipynb)과 데이터 파일(table_lv7_rf_silva.tsv)이 같은 작업 폴더 안에 위치한지 확인한다
  3) jupyter notebook을 실행하고,
      - 01.Preprocessing.ipynb
      - 02.Visualization.ipynb
      - 03.Modeling.ipynb
     을 차례로 실행한다.
 
