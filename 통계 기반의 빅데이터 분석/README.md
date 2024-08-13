### naver_news_crw.py
월드컵 주제에 관련된 네이버 뉴스 텍스트를 크롤링합니다.
<br><br>
| 작업 설계 | 사용할 코드 |
|:----|:---------|
|1. 검색어 지정하기|scrText='월드컵'|
|2. 네이버 뉴스 검색하기|getNaverSearch()|
|   2.1 url 구성하기|url = base + node + srcText|
|   2.2 url 접속과 검색 요청하기|urllib.request.urlopen()|
|   2.3 요청 결과를 응답 JSON으로 받기|json.load()|
|4. 응답 데이터를 정리하여 리스트에 저장하기|getPostData()|
|5. 리스트를 JSON 파일로 저장하기|json.dumps()|
