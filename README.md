# Bigdata_Webcrawling
유명 프랜차이즈 교촌치킨 매장을 찾습니다.

교촌치킨 매장 사이트를 통해, 매장 정보를 크롤링합니다. 

[지점명, 시도, 군구, 주소] 4가지 속성을 추출하여 kyochon.csv 로 저장합니다.



### 교촌치킨 매장 정보 수집
---
> 교촌치킨 매장찾기 : <http://www.kyochon.com/shop/domestic.asp?>

- 교촌치킨은 시/도, 구/군 별 Select 항목을 선택해야 해당 지역의 매장 결과가 출력됩니다. 

![image](https://user-images.githubusercontent.com/123874552/229308872-aba64f67-83bb-4e91-9813-103319a859da.png)

- url의 변화 규칙을 확인하고 이를 변경, 요청을 반복하여 모든 매장을 탐색합니다. 

![image](https://user-images.githubusercontent.com/123874552/229308996-05bf44ea-3715-41fc-aaed-cf36ad5e06e3.png)
![image](https://user-images.githubusercontent.com/123874552/229309017-5e771a65-6067-4eda-b11d-b640a20e9471.png)

- 웹 페이지의 HTML 코드를 확인하여 각 시/도에 따른 군/구의 매장 전체정보에서 존재하는 매장의 존재 유무에 따라 4가지 속성을 차례로 저장합니다.

![image](https://user-images.githubusercontent.com/123874552/229308956-cd7aaf27-dea5-4ec2-a64d-0ead38371c6d.png)
