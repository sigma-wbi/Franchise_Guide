# 프랜차이즈 선택 가이드


## 프로젝트 소개
요식업에 처음 도전하는 창업자들을 위한 사이트 제작하였습니다. <br>
현재 수도권에 어떤 프렌차이즈 매물들이 있는지 확인할 수 있습니다.<br>
원하는 프렌차이즈 브랜드가 있다면 검색할 수 있습니다. <br>
내 창업 조건에 따른 한달 예상 수익을 예측할 수 있습니다.<br>

## 프로젝트 의의
* Selenium을 사용하여 데이터를 얻고자 하는 사이트에서 데이터를 추출하였습니다. 
* 크롤링을 통한 데이터를 분석에 용이하도록 정제하고, 정제한 데이터를 선형 회귀 모델을 사용하여 예상 수익을 예측하였습니다.
* 사용자가 알아보기 쉽도록 데이터셋을 사용하여 대시보드를 제작하였습니다.
* 대시보드와 예상 수익을 함께 확인할 수 있는 웹 사이트를 Flask를 사용하여 제작하였습니다. 

## 📚Stack
![badge](https://img.shields.io/badge/Selenium-21B352?style=flat-square&logo=selenium&logoColor=white)
![badge](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![badge](https://img.shields.io/badge/Metabase-509EE3?style=flat-square&logo=metabase&logoColor=white)
![badge](https://img.shields.io/badge/scikit-learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![badge](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)

## About Data Crawling
* Crawling site : http://www.changupmedia.com/cumedia/index.asp
* Data Cleaning : https://github.com/sigma-wbi/Franchise_Guide/blob/main/flask_app/DataCleaning.ipynb
* Data Analysis : https://github.com/sigma-wbi/Franchise_Guide/blob/main/flask_app/analysis.ipynb
* Final Data : https://github.com/sigma-wbi/Franchise_Guide/blob/main/flask_app/datafinal.csv
* Linear Regression Data : https://github.com/sigma-wbi/Franchise_Guide/blob/main/flask_app/modelData.csv

## 프로젝트 과정

1. 데이터 크롤링 & 정제
    - 데이터를 얻을 사이트(http://www.changupmedia.com/cumedia/index.asp)에서 Selenium을 사용하여 데이터 크롤링
    - 크롤링한 데이터를 대시보드와 선형 회귀 모델에 사용할수 있도록 정제 -> modelData.csv, datafinal.csv
<img width="80%" src="images\5.jpg"/>

2. 데이터 시각화 & 머신러닝 예측
    - 정제한 데이터를 분석 & 시각화
    - 선형 회귀 모델을 사용한 예상 수익 예측
<img width="80%" src="images\6.jpg"/>

3. 웹페이지 제작 & 대시보드/머신러닝 모델 연동
<img width="80%" src="images\3.jpg"/>
<img width="80%" src="images\4.jpg"/>
<img width="80%" src="images\7.jpg"/>
<img width="80%" src="images\8.jpg"/>


## Report
https://github.com/sigma-wbi/Franchise_Guide/blob/main/report/Franchise_Guide_report.pdf