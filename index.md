
# Summary / 개요<br>

## IOT(사물인터넷)

Internet of Things의 약자로 사물인터넷은 사물에 센서를 부착해 실시간으로 데이터를 인터넷으로 주고받는 기술이나 환경을 일컫는다.<br><br>
지금까진 인터넷에 연결된 기기들이 정보를 주고받으려면 인간의 ‘조작’이 개입돼야 했다. <br><br>
하지만 사물인터넷에 연결된 기기는 사람의 도움 없이 서로 알아서 정보를 주고 받으며 대화를 나눌 수 있다.<br><br>
블루투스나 근거리무선통신(NFC), 센서데이터, 네트워크가 이들의 자율적인 소통을 돕는 기술이 된다.<br><br>

## 기능설명
### WIFI을 이용해 자동으로 실시간 날씨 데이터를 이용하는 옷걸이<br>

아두이노 회로에 붙은 IOT모듈이 날씨데이터를 받아온다.<br><br>
받아온 데이터는 디스플레이에 표시되어 사용자에게 정보를 전달한다.<br><br>
데이터에 있는 온도를 이용해 구동계가 링이 움직여 옷걸이를 정렬한다.<br><br>
정렬을 마치면 오늘 날씨에 적당한 옷이 보기 편한 자리에 위치하게 된다.<br><br>

# Concept / 구상안<br>
## 3D모델링
![KakaoTalk_20201101_153744209](https://user-images.githubusercontent.com/73837890/97888691-c5f97480-1d6e-11eb-96a2-a50d110c40d9.jpg)
![KakaoTalk_20201101_153744209_01](https://user-images.githubusercontent.com/73837890/97888698-c7c33800-1d6e-11eb-87c4-0c50b8099cf7.jpg)

## 날씨 데이터 받아오기
[페이지](https://postpop.tistory.com/86)참고<br><br>
기상청 페이지에서 RSS(Really Simple Syndication, Rich Site Summary)를 받아올 수 있다. <br><br>
RSS를 활용하면 홈페이지에 일일이 방문하지 않아도 업데이트 될 때마다 빠르고 편리하게 확인할 수 있다.<br><br>
[용인시 기흥구 RSS 링크](http://www.kma.go.kr/wid/queryDFSRSS.jsp?zone=4146353000)<br><br>

## 구동계 동작
![바 시뮬레이션](https://user-images.githubusercontent.com/73837890/97899533-c4cf4400-1d7c-11eb-976c-aaf15b67564c.gif)

## IOT 보드
![iot모듈](https://user-images.githubusercontent.com/73837890/97905518-77a3a000-1d85-11eb-8484-61be44a0a5ca.PNG)

# Making / 제작과정<br>

## 모델링
![모델링 사진](https://user-images.githubusercontent.com/73837890/102479043-b83f4a80-40a1-11eb-9138-4575d8fbef1c.PNG)
![프린트 출력물](https://user-images.githubusercontent.com/73837890/102479026-b1b0d300-40a1-11eb-8970-a30cdf677296.jpg)


## 구동부 결합
![롤러 벨트 결합](https://user-images.githubusercontent.com/73837890/102479653-84185980-40a2-11eb-8b1b-a9fba78b42d8.JPG)
![베어링+슬라이더](https://user-images.githubusercontent.com/73837890/102479849-cb064f00-40a2-11eb-83ee-28ab6a104dd9.JPG)
![슬라이더 + 벨트](https://user-images.githubusercontent.com/73837890/102480052-1882bc00-40a3-11eb-8809-8e3cb1885c67.JPG)
![전체 결합](https://user-images.githubusercontent.com/73837890/102480073-20daf700-40a3-11eb-8949-91481c3862e3.JPG)

<iframe width="640" height="360" src="https://www.youtube.com/embed/eqg26JvUuXU" gesture="media" allowfullscreen="">
</iframe>

## 결선
![결선 사진](https://user-images.githubusercontent.com/73837890/102479722-9b574700-40a2-11eb-9080-fdef2bc2c8ec.jpg)

## 코딩
esp 코드[#](https://github.com/uyh1998/AdventureDesignProject/blob/main/code-esp)
우노 보드 코드[#](https://github.com/uyh1998/AdventureDesignProject/blob/main/code-uno)

# Output / 완성 작품

## 외관
![외관](https://user-images.githubusercontent.com/73837890/102483590-5209f600-40a8-11eb-848e-10d27c4a72b7.jpg)


## 작동방식
터치시하는 부분 , 디스플레이 부분 설명

## 온도별 구동부 움직임
<iframe width="640" height="360" src="https://www.youtube.com/embed/oV1YMRpGXe8" gesture="media" allowfullscreen="">
</iframe>
<iframe width="640" height="360" src="https://www.youtube.com/embed/rPrDkbB5mDc" gesture="media" allowfullscreen="">
</iframe>
<iframe width="640" height="360" src="https://www.youtube.com/embed/uElTN_Ac87A" gesture="media" allowfullscreen="">
</iframe>

## 작동예시
<iframe width="640" height="360" src="https://www.youtube.com/embed/I9r5AFO4quc" allowfullscreen="">
</iframe>




# Reference / 참고자료

날씨 데이터 받아오기[#1](https://postpop.tistory.com/86)[#2](https://m.blog.naver.com/PostView.nhn?blogId=compass1111&logNo=221133450681&proxyReferer=https:%2F%2Fwww.google.com%2F)<br>
기상청 날씨누리[#](https://www.weather.go.kr/w/weather/now.do)<br>
기상청 RSS 데이터[#](https://www.weather.go.kr/weather/lifenindustry/sevice_rss.jsp?sido=4100000000&gugun=4146300000&dong=4146353000&x=30&y=12)<br>
아두이노 IOT 활용 영상[#](https://www.youtube.com/watch?v=8rLFYjeFf_c&t=394s)<br>
Onshape 모델링[#](https://cad.onshape.com/documents/a7ac3f0235dd5f6b6191ebe7/w/da14889e2f97f6c179aa0c51/e/18bfe2a3db88af4022d3ebe9)<br>
RSS 데이터 정의[#](https://www.weather.go.kr/images/weather/lifenindustry/dongnaeforecast_rss.pdf)<br>
아두이노 WIFI 연결[#](https://postpop.tistory.com/23)
