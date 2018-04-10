---
class:
- line
rel:
- self
properties:
  name: Scraping
  sort: 1144
  level: 2
  description: Obtaining content through scraping of web pages, and then allowing
    for the transformation of data and contained obtained, and deliver as simpler
    web APIs.
  tools:
    - name: Scrapy
      description: An open source and collaborative framework for extracting the data you need from websites. In a fast, simple, yet extensible way.
      url: https://scrapy.org/
    - name: Apache Tika
      description: Apache TikaThe Apache Software Foundation Apache Tika - a content analysis toolkit The Apache Tika™ toolkit detects and extracts metadata and text from over a thousand different file types (such as PPT, XLS, and PDF). All of these file types can be parsed through a single interface, making Tika useful for search engine indexing, content analysis, translation, and much more.
      url: http://tika.apache.org/      
  services:
    - name: Scrapinghub
      description: Scrapinghub is a company that provides web crawling solutions, including a platform for running crawlers, a tool for building scrapers visually, data feed providers (DaaS) and a consulting team to help startups and enterprises build and maintain their web crawling infrastructures.
      url: http://scrapinghub.com/
    - name: ParseHub
      description: ParseHub is a free web scraping tool. With our advanced web scraper, extracting data is as easy as clicking the data you need.
      url: https://www.parsehub.com/   
    - name: Import.io
      description: Import.io is intuitive and highly capable. Simply point-and-click to show us the data of interest on a web page. Machine learning based – no coding required
      url: https://www.import.io/       
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Scraping
  links:
  - rel:
    - self
    href: deployment/scraping/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/scraping/
- rel:
  - parent
  href: deployment/
...
