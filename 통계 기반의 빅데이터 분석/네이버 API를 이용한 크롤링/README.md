### naver_news_crw.py
월드컵 주제에 관련된 네이버 뉴스 텍스트를 크롤링합니다.
<br><br>
| 작업 설계 | 사용할 코드 |
|:----|:---------|
|1. 검색어 지정하기|scrText='월드컵'|
|2. 네이버 뉴스 검색하기|getNaverSearch()|
|&nbsp;&nbsp;&nbsp;&nbsp;2.1 url 구성하기|url = base + node + srcText|
|&nbsp;&nbsp;&nbsp;&nbsp;2.2 url 접속과 검색 요청하기|urllib.request.urlopen()|
|&nbsp;&nbsp;&nbsp;&nbsp;2.3 요청 결과를 응답 JSON으로 받기|json.load()|
|4. 응답 데이터를 정리하여 리스트에 저장하기|getPostData()|
|5. 리스트를 JSON 파일로 저장하기|json.dumps()|

### UML
![naver_news_crw drawio (2)](https://github.com/user-attachments/assets/fcb21bf8-3e3b-449b-a6e7-ed6b91bf878f)

### urllib
https://www.notion.so/urllib-7861e6160b5246b6a897e1b5945a6f86

### json
https://www.notion.so/Json-ebd4a3c0c7ff4f75a98c7010cdd33ef1

### velog
https://velog.io/@ellcoding/%EB%84%A4%EC%9D%B4%EB%B2%84-API%EB%A5%BC-%EC%9D%B4%EC%9A%A9%ED%95%9C-%ED%81%AC%EB%A1%A4%EB%A7%81
