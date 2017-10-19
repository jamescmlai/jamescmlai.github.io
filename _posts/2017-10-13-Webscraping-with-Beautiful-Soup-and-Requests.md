---
layout: post
title: Webscraping with Beautiful Soup and Requests
---

### What is web scraping?
The internet is a veritable treasure trove of informational that is at our finger tips.  If you're fortunate enough,  data will be all ready and packaged up in a tidy csv or via. an application programming interface (API). For other times, there's web scraping!

Unfortunately things are not always this easy and we're only able to access this information through directly interacting with a web page itself.  This is known as web scraping, whereby text information is extracted directly from the website HTML.

Thankfully Python has two fantastic tools to help with loading web pages as a string (requests), and parsing the HTML (beautiful soup) to extract the tidbits that you're after.

### Web scraping through a list of customer websites, a practical example
In the example below, a client wanted to scrape information from their customers' websites for further analysis to help get a better understanding of their near thirty thousand customers in their database.

The notebooks attached contains the process for capturing this in two seperate parts.

#### 1. DNS lookup
A quick DNS search was conducted first to separate live and expired sites to expedite the actual web scraping process.  The code in this notebook also captured the e-commerce platform based on client requirements.

Click [here](https://github.com/jamescmlai/github_portfolio/blob/master/webscraping/DNS_lookup.ipynb) to see this notebook.

#### 2. Web scraper 
Utilises Requests and Beautiful Soup to iterate through the customer list of websites and capture the HTML text for further analysis down the line.
- working through just shy of 30,000 sites and with inconsistent internet speed (thanks Australian NBN), the code automatically saves a csv file after every 200 websites scraped.
- this notebook was copied and run in parallel to expedite the process.

Click [here](https://github.com/jamescmlai/github_portfolio/blob/master/webscraping/Web_scraper.ipynb) to see this notebook.

After running these notebooks for a couple of hours, this captured a couple GB of HTML string data - you can be more efficient in only capturing interesting parts of the text, but the entirety of the text was captured in this instance.

This can now be analysed using Natural Language Processing and other interesting techniques, some of which will be covered in a separate post down the line.

