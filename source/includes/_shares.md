# Share Count

> Example Request

```shell
curl http://alpha.donreach.com/shares?url=http://9gag.com/ \
  -H "Authorization: YOUR_API_KEY"
```

> Example Response

```json
{
  "url": "http://9gag.com/",
  "total": 11008159,
  "shares": {
    "facebook": 244770,
    "google": 88086,
    "linkedin": 658,
    "pinterest": 10552542,
    "twitter": 122103
  }
}
```

Retrieves share counts for a given URL from selected social networking platforms.

### Parameters

Parameter	| Default | Description
----------|---------|------------
url (required) | none | The URL of the page you want to fetch the social shares for.
format (optional) | json | The format of the output. Can be either json, jsonp or xml.
callback (optional) | processShares | The JavaScript callback to execute.
providers (optional) | facebook, twitter, google, linkedin, pinterest | Which social sharing providers to query. See [Provider Codes](#provider-codes) for full list.

### Provider Codes

<aside class="notice">
The providers' object key in the response is spelt the same as it is in the providers parameter.
</aside>

Provider Name | Provider Code
--------------|--------------
Facebook | facebook
Google+ | google
Twitter | twitter
LinkedIn | linkedin
Pinterest | pinterest
Tumblr | tumblr
Pocket | pocket
Buffer | buffer
Hacker News | hackernews
Reddit | reddit
StumbleUpon | stumbleupon
Scoop.it | scoopit
Xing | xing
Fancy | fancy
Yummly | yummly
Sina Weibo | weibo
Hatena | hatena
VK | vk
Mail.ru | mailru
Odnoklassniki | odnoklassniki
