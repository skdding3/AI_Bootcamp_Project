# FIFA 21 Data Analysis Web Service


## 개요

축구게임 FIFA 21 선수 능력치 데이터를 조회하여 게임에 들어가지 않아도 웹에서 능력치를 확인하고 분석하는 서비스를 제공.

종합적인 수치를 한눈에 제공하는 방향성으로 작업을 진행

데이터는 피파21 SOFIFA 사이트에서 데이터를 발췌하였음.


## SKILL

Python (Flask) 웹 프레임 워크 동작

Java Script : 레이더 차트, QTIPS 등 동적개체 작동 (Jquery)

HTML5/CSS : fonts, 페이지 배경 등 구성

Docker : form container 


## 내부 디렉토리 구조
```
data
┖ static
  ┖ image
  ┖ css
  ┖ fonts
  ┖ jss
┖ templates
  ┖ base.html
  ┖ home.html
  ┖ player.html
.gitignore			
app.py # 플라스크 실행 파일 
Dockerfile # 폼 컨테이너화
form.py	# 폼 정의
requirements.txt # 필요한 라이브러리 모음
readme.md	# 설명
```


## 서비스 구성

### HOME

검색화면과 함께 선수이름 일부만 입력해도 검색 자동완성 기능 제공

원하는 선수에 대한 자료 선택 가능


### PLAYER_NAME PAGE

선수에 대한 능력치 분석을 시각적인 자료과 함께 분석자료 제공

HELP -> 반응형 객체로 구성하여 포인터를 올릴시 안내를 볼수있음.

RADER CHART -> 선수 세부차트를 종합하여 한눈에 볼수있는 시각적 분석 자료 제공. 마우스포인터로 자세한 세부 수치를 확인 가능

STATUS -> 게이머들이 즐겨 찾는 선수가 가진 각 특징적인 부분을 텍스트로 제공. 5점만점 수치는 별 등으로 표기.



### 향후 개선 방향

데이터에 대한 실시간 수집이 아닌 피파21 게임 발매 당시 자료로 최신화에 대한 한계가 있음.

매번 선수 성적에 따른 능력치 변화나 이적 등 유동적 변화에 대한 실시간 업데이트 기능 구현 검토.

선수 얼굴이나 소속 클럽 로고 , 포지션 별 능력등 더 세부적인 데이터를 제공할 여지가 있음.
