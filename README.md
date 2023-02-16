# Bing Search Result Scraper

## What does Bing Search Result Scraper do?
Bing Search Result Scraper extracts the following data from Bing search results: 
- Organic results
- Related queries
- See results for
- Recommended searches
- People Also Ask
- Wiki results
- News, Image, Video results

## Why use Bing Search Result Scraper?
Extracting data from Bing search results can help you to:
- Consistently monitor how your website ranks on Bing SERPs for specific keywords.
- Monitor competition automatically: both organic results and Ads section.
- Analyze advertisement campaigns to sharpen the keyword targeting of your Bing Ads.
- Improve the performance of your website content by applying the SEO insights needed to top the Bing SERP rankings.
- Make data-backed decisions in your SEO strategy.
- Follow demand and predict new trends by scraping *recommended searches, *Related queries, *See results for* and *People Also Ask*

You can see our [industry pages](https://apify.com/industries) for more tangible ideas, use cases, or inspiration on how to use scraped Bing data in your business.

## Is scraping Bing legal?
Since scraping Bing and other search engines does not require a login, it is legal to scrape Bing search results as the data is publicly available. However, you may still be bound by the Bing terms of use. If you are unsure of the legal implications of your scraping, you can learn more in [Is web scraping legal?](https://blog.apify.com/is-web-scraping-legal/)

## How do you scrape Bing search results?
To understand how to set up and run Bing Search Result Scraper, check out our step-by-step guide on [how to scrape Bing](https://blog.apify.com/how-to-scrape-bing-search-results/#how-to-scrape-bing-search-results) with screenshots and examples.

## Integrations and Bing Search Result Scraper
Bing Search Result Scraper can be connected with almost any cloud service or web app thanks to [integrations on the Apify platform](https://apify.com/integrations). Integrate with Make, Zapier, Slack, Airbyte, GitHub, Google Sheets, Google Drive, and more. Or you can use webhooks to carry out an action whenever an event occurs, e.g. get a notification whenever Bing Search Result Scraper successfully finishes a run.

## Using Bing Search Result Scraper with the Apify API
The Apify API gives you programmatic access to the Apify platform. The API is organized around RESTful HTTP endpoints that enable you to manage, schedule, and run Apify actors. The API also lets you access any datasets, monitor actor performance, fetch results, create and update versions, and more.To access the API using Node.js, use the apify-client NPM package. To access the API using Python, use the apify-client PyPI package. Check out the [Apify API reference docs](https://docs.apify.com/api/v2) for full details or click on the [API tab](https://apify.com/spidoosho/bing-search-scraper/api#features) for code examples.

## Input parameters
The input for Bing Search Result Scraper should be JSON containing the search terms you want to scrape. Click on the [input tab](https://apify.com/spidoosho/bing-search-scraper/input-schema) for an input example.

## Results
Actor stores its result in the default dataset associated with the run, which you can export to various formats.

The results can be downloaded from the [Get dataset items](https://docs.apify.com/api/v2#/reference/datasets/item-collection/get-items) API endpoint:
```
https://api.apify.com/v2/datasets/[DATASET_ID]/items?format=[FORMAT]
```
where `[DATASET_ID]` is the ID of the dataset and `[FORMAT]` can be `csv`, `html`, `xlsx`, `xml`, `rss` or `json`.

For each Bing search results page, the dataset will contain a single record, which in JSON format looks as follows. Bear in mind that some fields have example values:
```json
{
  "url": "https://www.bing.com/search?q=restaurants+in+NYC&setmkt=en-US&setLang=en&count=20",
  "keyword": "restaurants in NYC",
  "pageNumber": "1",
  "topBorders": [
    {
      "type": "topborder",
      "title": "3 Restaurant Stocks to Buy as Portillo’s IPO Puts Food in Focus | M…",
      "description": "McDonald’s ( NYSE:MCD)Chipotle Mexican Grill ( NYSE:CMG)Shake Shack ( NYSE:SHAK)",
      "url": "https://markets.businessinsider.com/news/stocks/3-restaurant-stocks-to-buy-as-portillos-ipo-puts-food-in-focus-1030942104#:~:text=1%20McDonald%E2%80%99s%20%28%20NYSE%3AMCD%29%202%20Chipotle%20Mexican,Grill%20%28%20NYSE%3ACMG%29%203%20Shake%20Shack%20%28%20NYSE%3ASHAK%29"
    }
  ],
  "news": [],
  "images": [
    {
      "url": "https://www.bing.com/images/search?q=restaurants+in+nyc&id=2A4278536950043E64049BF31FF7EF10AE59890E&FORM=IQFRBA&tsc=ImageHoverTitle",
      "description": "The 8 Most Romantic Restaurants In New York City ..."
    },
    {
      "url": "https://www.bing.com/images/search?q=restaurants+in+nyc&id=CB6E30A74EE489542CAC44CC2AF03EADD002B5AD&FORM=IQFRBA&tsc=ImageHoverTitle",
      "description": "NYC’s Best Restaurants For Celebrity Sightings – CBS New York"
    }
  ],
  "videos": [
    {
      "url": "https://www.bing.com/videos/search?q=restaurants+in+NYC&docid=608027044097975381&mid=847D6D6E00C15262FE03847D6D6E00C15262FE03&view=detail&FORM=VIRE",
      "channel": "Sarah Funk",
      "date": "6 months ago",
      "title": "The Best Restaurants in NYC (the NEW 2021 dining guide)",
      "views": "79K views",
      "provider": "YouTube"
    },
    {
      "url": "https://www.bing.com/videos/search?q=restaurants+in+NYC&docid=608028478616464812&mid=9764CA38921564D86ABA9764CA38921564D86ABA&view=detail&FORM=VIRE",
      "channel": "Sarah Funk",
      "date": "Jun 21, 2018",
      "title": "Best Restaurants in NYC | A Culinary Tour with a local New Yorker",
      "views": "270K views",
      "provider": "YouTube"
    }
  ],
  "pages": [
    {
      "title": "THE 10 BEST Restaurants in New York City - Updated ...",
      "link": "https://www.tripadvisor.com/Restaurants-g60763-New_York_City_New_York.html",
      "desc": "Restaurants in New York City 1. Club A Steakhouse. 2. Mei Jin Ramen. 3. Boucherie Union Square. 4. Boucherie West Village. 5. Bua Thai Ramen & Robata Grill. 6. Olio e Piu. 7. Piccola Cucina. 8. Bleecker Street Pizza. 9. La Grande Boucherie. 10. …"
    },
    {
      "title": "THE BEST 10 Restaurants in New York, NY - Last Updated ...",
      "link": "https://www.yelp.com/search?cflt=restaurants&find_loc=new+york%2C+NY",
      "list": [
        "Thursday Kitchen. 1473. $$East Village. “I've been wanting to come to Thursday Kitchen for …",
        "The Cabin NYC. 349. $$East Village. Locally owned & operated. Outdoor seating. Waitlist …",
        "Raku. 552. $$South Village. Proof of vaccination required. “Raku is my favorite Udon in NYC! …",
        "Amélie. 2758. $$$Greenwich Village. “I love quirks; that's the secret to living with myself, and …",
        "Joe’s Shanghai. 6482. $$Chinatown. “The service was excellent, I got the shrimp lo mein-a …",
        "Raku. 1220. $$East Village. Proof of vaccination required. Waitlist opens at 12:00 pm. “FYI: …",
        "Wayla. 418. $$Lower East Side. “Service was above and beyond, shout out to our man / host …",
        "Jane. 3232. $$Greenwich Village. “Great Sunday brunch! Had a reservation for 5 people, we …",
        "Olio e Piú. 2867 $$ Proof of vaccination required. “This is my first time here at this restaurant …",
        "Da Andrea. 1004. $$Greenwich Village. “It was so nice to have a dinner in this wonderful …"
      ],
      "desc": ""
    },
    {
      "title": "New York Restaurants and Dining Guide | NYC.com ...",
      "link": "https://www.nyc.com/restaurants/",
      "desc": "Eleven Madison Park expresses the spirit of grand New York dining with a contemporary accent. Designed by architects Bentel & Bentel, with soaring 30-foot ceilings and windows overlooking beautiful Madison Square Park, the Art-Deco restaurant embodies an urbane sophistication that is at once relaxed and bustling."
    }
  ],
  "explore": [
    {
      "title": "New York City Restaurants",
      "imgUrl": "https://www.bing.com/images/search?q=New+York+City+Restaurants&FORM=IARSLK"
    },
    {
      "title": "Restaurant Modern NYC",
      "imgUrl": "https://www.bing.com/images/search?q=Restaurant+Modern+NYC&FORM=IARSLK"
    }
  ],
  "related": [
    {
      "text": "best trendy restaurants in nyc",
      "url": "https://www.bing.com/search?q=best+trendy+restaurants+in+nyc&FORM=QSRE1"
    },
    {
      "text": "best restaurants nyc 2021",
      "url": "https://www.bing.com/search?q=best+restaurants+nyc+2021&FORM=QSRE2"
    }
  ]
}
```
