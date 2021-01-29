# 네이버 뉴스기사 크롤링
- AICT fake news detection 프로젝트 데이터 구축에 사용
- 참고 링크 : https://github.com/lumyjuwon/KoreaNewsCrawler

##### arciclecrawler.py
```python
from korea_news_crawler.articlecrawler import ArticleCrawler

Crawler = ArticleCrawler()  
Crawler.set_category("정치", "경제", "사회")  
Crawler.set_date_range(2019, 1, 2020, 12)  
Crawler.start()

```
__2019 ~ 2020 정치, 경제 , 사회 뉴스를 멀티프로세서를 이용한 병렬 크롤러__
