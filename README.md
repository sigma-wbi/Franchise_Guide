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
<img width="80%" src="images\1.jpg"/>

2. 데이터 시각화 & 머신러닝 예측
    - 정제한 데이터를 분석 & 시각화
    - 선형 회귀 모델을 사용한 예상 수익 예측
<img width="80%" src="images\2.jpg"/>

3. 웹페이지 제작 & 대시보드/머신러닝 모델 연동
    

## 분석 결론
* 일본지역 게임 설계 전략과 그 외 지역(NA,EU,Other) 설계 전략을 따로 둔다.

* 일본지역은 Nintendo 계열 플렛폼에 충성도가 높고 롤플레잉 장르의 게임이 인기가 많다.
<br/>-> Nintendo 플랫폼을 활용한 Role-Palying 장르의 게임

* 그 외 지역(NA,EU,Other)은 PlayStation 플렛폼의 점유율이 가장 높고 액션, 스포츠 장르의 게임이 인기가 많다.

* 전체적으로 판매량이 급등한 2000년대 이후로 2006년 과 2009 년의 최고 장르가 스포츠인것으로 보아 4년마다 열리는 월드컵의 영향이 있을 것으로 보인다.

* 액션 장르는 확실히 1위 장르이지만 출고량 랭킹에서는 찾기 힘들었다. 이는 GTA 시리즈가 액션 장르의 대부분을 가지고 있었기 때문이다.

* 성공이 보장된 전작이 존재하는 시리즈 게임을 제작할시 GTA 시리즈와 유사한 엑션 장르 게임을 제작하는 것도 나쁘진 않지만 게임 하나를 제작하는 회사 입장에서는 판매량이 보다 고르게 분포되어 있고, 2위 장르였던 스포츠 장르를 선택하는 것이 더 좋다고 판단됨.

* 또한 2022년은 월드컵이 열리는 해 이므로 스포츠 장르를 택해야하는 이유에 좀 더 설득력을 준다고 생각한다.
<br/>-> NA,EU,Other 지역에는 PlayStation 기반의 스포츠 장르의 게임

<img width="80%" src="https://user-images.githubusercontent.com/81278907/232700899-10d90c04-458a-4f27-9a97-911a0d6812b5.png"/>


## Report
https://github.com/sigma-wbi/Franchise_Guide/blob/main/report/Franchise_Guide_report.pdf