---
layout: page
title: Get Started
subtitle: Start using the footApi API
---

The data is grouped by competition (Ligue 1, Premier League...) and season (2014-2015...).  
So to start you can ask the API which competitions are available with a simple endpoint.

## Request
The API only accepts GET requests.

```
{{ site.url }}/competition
```

### Curl
```
curl -X GET "{{ site.url }}/competition" -H "accept: application/json; charset=utf-8"
```

## Response
```javascript
[
  {
    "_id": 1,
    "data": {
      "country": "fr",
      "competition": "ligue 1"
    },
    "links": {
      "self": "footApi.com/competition/1",
      "season": "footApi.com/season/competition/1",
      "table": "footApi.com/table/competition/1",
      "game": "footApi.com/game/competition/1"
    }
  },
  {
    "_id": 2,
    "data": {
      "country": "fr",
      "competition": "ligue 2"
    },
    "links": {
      "self": "footApi.com/competition/2",
      "season": "footApi.com/season/competition/2",
      "table": "footApi.com/table/competition/2",
      "game": "footApi.com/game/competition/2"
    }
  }
]
```

## Rate limit
You can ask for an API Key to increase your Rate limit, it's totally free.  
See : [API Key]({{ site.baseurl }}{% link apikey.md %})

## Endpoints
To see the full API Endpoints and ressources availables you can check the documentation.  
See : [API Key]({{ site.baseurl }}{% link apikey.md %})