# 네이버 뉴스기사 크롤링
- AICT fake news detection 프로젝트에 사용
- 참고 링크 : https://github.com/lumyjuwon/KoreaNewsCrawler
- 위 링크에서 기사 감정표현, 수정시간 등 추가 + 정규표현식 약간의 수정

##### arciclecrawler.py
```python
from korea_news_crawler.articlecrawler import ArticleCrawler

Crawler = ArticleCrawler()  
Crawler.set_category("정치", "경제", "사회")  
Crawler.set_date_range(2019, 1, 2020, 12)  
Crawler.start()

```
__2019 ~ 2020 정치, 경제 , 사회 뉴스를 멀티프로세서를 이용한 병렬 크롤러__