# wikipedia-trends

## Example sites

Pageview Analysis https://pageviews.toolforge.org/?project=en.wikipedia.org&platform=all-access&agent=user&redirects=0&range=latest-20&pages=Cat|Dog

Page stats: https://xtools.wmflabs.org/articleinfo/en.wikipedia.org/Quibi


## Official Wikipedia API Documentation

Main page: https://www.mediawiki.org/wiki/API:Main_page

https://wikimedia.org/api/rest_v1/


## API info and properties

https://www.mediawiki.org/wiki/API:Properties


### Last 500 revisions

https://www.mediawiki.org/wiki/API:Revisions

https://en.wikipedia.org/w/api.php?action=query&prop=revisions&format=json&rvprop=timestamp|user|comment&rvlimit=500&titles=Donald_Trump




## API metrics




### Opensearch (autocompletion)

Reference: https://www.mediawiki.org/wiki/API:Opensearch

https://en.wikipedia.org/w/api.php?action=opensearch&format=json&formatversion=2&limit=10&namespace=0&profile=fuzzy&redirects=resolve&search=beyo


Result:

```json
[
  "beyo",
  [
    "Beyoncé",
    "Beyoncé discography",
    "Beyoncé (album)",
    "Beyond: Two Souls",
    "Beyond the Valley of the Dolls",
    "Beyond Good & Evil (video game)",
    "Beyond the Realm of Conscience",
    "Beyond the Clouds (2017 film)",
    "Beyonder",
    "Beyond Belief: Fact or Fiction"
  ],
  [
    "",
    "",
    "",
    "",
    "",
    "",
    "",
    "",
    "",
    ""
  ],
  [
    "https://en.wikipedia.org/wiki/Beyonc%C3%A9",
    "https://en.wikipedia.org/wiki/Beyonc%C3%A9_discography",
    "https://en.wikipedia.org/wiki/Beyonc%C3%A9_(album)",
    "https://en.wikipedia.org/wiki/Beyond:_Two_Souls",
    "https://en.wikipedia.org/wiki/Beyond_the_Valley_of_the_Dolls",
    "https://en.wikipedia.org/wiki/Beyond_Good_%26_Evil_(video_game)",
    "https://en.wikipedia.org/wiki/Beyond_the_Realm_of_Conscience",
    "https://en.wikipedia.org/wiki/Beyond_the_Clouds_(2017_film)",
    "https://en.wikipedia.org/wiki/Beyonder",
    "https://en.wikipedia.org/wiki/Beyond_Belief:_Fact_or_Fiction"
  ]
]
```




### daily page views by user, for 2016

Reference: https://wikimedia.org/api/rest_v1/#/Pageviews%20data




Example: https://wikimedia.org/api/rest_v1/metrics/pageviews/per-article/en.wikipedia/all-access/user/Barack_Obama/daily/2016010100/2016123100

```json
{
  "items": [
    {
      "project": "en.wikipedia",
      "article": "Barack_Obama",
      "granularity": "daily",
      "timestamp": "2016010100",
      "access": "all-access",
      "agent": "user",
      "views": 26166
    },
    { "...", "..."},
    {
      "project": "en.wikipedia",
      "article": "Barack_Obama",
      "granularity": "daily",
      "timestamp": "2017123000",
      "access": "all-access",
      "agent": "user",
      "views": 16821
    },
    {
      "project": "en.wikipedia",
      "article": "Barack_Obama",
      "granularity": "daily",
      "timestamp": "2017123100",
      "access": "all-access",
      "agent": "user",
      "views": 18294
    }
}
```


### Edits for a page

https://wikimedia.org/api/rest_v1/#/Edits%20data/get_metrics_edits_per_page__project___page_title___editor_type___granularity___start___end_
