# Web-Scraping using Scrapy

**Pre-requisites:**
```pip install scrapy```

**Remember before scraping:**
* There is a robot.txt file for each website for what they allow. Check that out before you scrape so that you don't scrape endpoints which are not allowed.
* If there is any API available for getting the same info. Use that instead of scraping.


**Performed Activities:**
* Learnt using scrapy shell ```scrapy shell```
    * Fetch Command ```fetch(<put_your_scraping_url_here/endpoint>)```
    * The Crawler returned response can be viewed using. ```view(response)```
      This will open the raw HTML in the default browser.
    * Print received response ```print(response.text)```
    * Extracting element using css selector ```response.css(".value::text").extract()```
    * Using XPath to get the elements. ```response.xpath("//div").extract()```
* Creating a Scrapy project and custom Spider
    * ```scrapy startproject aliexpress```
    * The command to create a spider ```scrapy genspider aliexpress_tablets <url>```


**References:**
* Rules before scraping: https://towardsdatascience.com/scraping-the-internets-most-popular-websites-a4c6f0be382d
* Learn about XPath here: https://www.datacamp.com/courses/web-scraping-with-python
* Excellent article for starting: https://www.datacamp.com/community/tutorials/making-web-crawlers-scrapy-python
* Get data from following pages: https://www.tutorialspoint.com/scrapy/scrapy_following_links.htm










