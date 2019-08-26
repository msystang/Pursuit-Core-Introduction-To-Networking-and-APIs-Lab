# Pursuit-Core-Introduction-To-Networking-and-APIs-Lab

# Part One

Status Code Scavenger Hunt!

Use Postman to find each of the following HTTP codes:


1. 200
1. 301
1. 400
1. 401
1. 403
1. 404
1. 418
1. 500


For each of the questions below, write:

1. The website which generated the HTTP status code
2. A description of what the status code means
3. If an app you were writing encountered this status code, what would you do (if anything) to resolve any issues?


For reference, see:

https://en.wikipedia.org/wiki/List_of_HTTP_status_codes (Links to an external site.)
https://http.cat

---
Answer:

1. 200
Website: https://httpstat.us/200
Code Description: OK: General success status for a HTTP request. Request was responded to with requested information.
Solution: N/A

1. 301
Website: https://httpstat.us/301
Code Description: Moved permanently: The destination of the URL has been moved permanently, and changes to the URI will be reflected in the new resource.
Solution: Automatically redirect the user to the new URL.

1. 400
Website: https://httpstat.us/400
Code Description: Bad request: The server can't perform the request because of a client error, such as bad syntax 
Solution: Double check that the syntax is correct.

1. 401
Website: https://httpstat.us/401
Code Description: Unauthorized: Client does not have the persmissions to access URL. 
Solution: Get necessary credentials.

1. 403
Website: https://httpstat.us/403
Code Description: Forbidden: Client does not have the right permissions. 
Solution: Get the CORRECT credentials.

1. 404
Website: https://httpstat.us/404
Code Description: Not Found: Server cannot find the URL the client is requesting.
Solution: Double check that the URL is correct!

1. 418
Website: https://httpstat.us/418
Code Description: I'm a teapot: Brewing coffe in a teapot.
Solution: Don't brew coffee in a teapot. :(

1. 500
Website: https://httpstat.us/500
Code Description: Internal server error: Error with the server that prevents it from performing requests.
Solution: Nothing we can do!

---

# Part Two

API Scavenger Hunt!

For each of the questions below, identify a website and search query that will give you the appropriate JSON.  Paste the url and the json below.  Googling the category + API will generally take you to where you need.  Ex. https://lmgtfy.com/?q=cat+fact+api

1. A random cat fact
Website URL: https://catfact.ninja/fact
JSON Body: 
```
[
{
"fact": "Some common houseplants poisonous to cats include: English Ivy, iris, mistletoe, philodendron, and yew.",
"length": 103
}
[
```

1. A list of 150 random users in English.
Website URL: https://randomuser.me/api/?results=150
JSON Body:  
```
{
"results": [
{
"gender": "male",
"name": {
"title": "mr",
"first": "derek",
"last": "carr"
},
"location": {
"street": "8458 thornridge cir",
"city": "adelaide",
"state": "northern territory",
"postcode": 1029,
"coordinates": {
"latitude": "-88.7728",
"longitude": "-37.7062"
},
"timezone": {
"offset": "+5:30",
"description": "Bombay, Calcutta, Madras, New Delhi"
}
},
"email": "derek.carr@example.com",
"login": {
"uuid": "42b6d04f-fce9-4043-81ed-40a927ed5654",
"username": "tinyswan342",
"password": "arkansas",
"salt": "7V4Kasmd",
"md5": "5927046e4db3775f73981eed9171cf62",
"sha1": "5745224b2b1b30e72745d006d527edec6418e329",
"sha256": "30249c25c9e5a326c886c30f3d92f46a9c36567ec90f6af859d4acf144069dbe"
},
"dob": {
"date": "1944-09-09T04:03:15Z",
"age": 74
},
"registered": {
"date": "2013-05-12T19:30:17Z",
"age": 6
},
"phone": "01-4983-4335",
"cell": "0473-800-692",
"id": {
"name": "TFN",
"value": "751450152"
},
"picture": {
"large": "https://randomuser.me/api/portraits/men/62.jpg",
"medium": "https://randomuser.me/api/portraits/med/men/62.jpg",
"thumbnail": "https://randomuser.me/api/portraits/thumb/men/62.jpg"
},
"nat": "AU"
}, //cont...
```
1. The current stock price of Microsoft. (IEX API)
Website URL: https://api.iextrading.com/1.0/tops/last?symbols=msft
JSON Body: 
```
[
{
"symbol": "MSFT",
"price": 134.81,
"size": 6,
"time": 1566843956854
}
]
```

1. The 5 year history of Apple stock prices (IEX API)
Website URL: https://github.com/iexg/IEX-API/issues/791
JSON Body: "That data will not be available. Everything under /stock will no longer be available on the old API, but will be on IEX Cloud."

1. All the Swift language repos on Github with Pursuit in their name
Website URL: https://api.github.com/search/repositories?q=pursuit
JSON Body: 
```
{
"total_count": 1296,
"incomplete_results": false,
"items": [
{
"id": 22592439,
"node_id": "MDEwOlJlcG9zaXRvcnkyMjU5MjQzOQ==",
"name": "pursuit",
"full_name": "purescript/pursuit",
"private": false,
"owner": {
"login": "purescript",
"id": 6556677,
"node_id": "MDEyOk9yZ2FuaXphdGlvbjY1NTY2Nzc=",
"avatar_url": "https://avatars2.githubusercontent.com/u/6556677?v=4",
"gravatar_id": "",
"url": "https://api.github.com/users/purescript",
"html_url": "https://github.com/purescript",
"followers_url": "https://api.github.com/users/purescript/followers",
"following_url": "https://api.github.com/users/purescript/following{/other_user}",
"gists_url": "https://api.github.com/users/purescript/gists{/gist_id}",
"starred_url": "https://api.github.com/users/purescript/starred{/owner}{/repo}",
"subscriptions_url": "https://api.github.com/users/purescript/subscriptions",
"organizations_url": "https://api.github.com/users/purescript/orgs",
"repos_url": "https://api.github.com/users/purescript/repos",
"events_url": "https://api.github.com/users/purescript/events{/privacy}",
"received_events_url": "https://api.github.com/users/purescript/received_events",
"type": "Organization",
"site_admin": false
},
"html_url": "https://github.com/purescript/pursuit",
"description": "Website for hosting and searching PureScript API documentation",
"fork": false,
"url": "https://api.github.com/repos/purescript/pursuit",
"forks_url": "https://api.github.com/repos/purescript/pursuit/forks",
"keys_url": "https://api.github.com/repos/purescript/pursuit/keys{/key_id}",
"collaborators_url": "https://api.github.com/repos/purescript/pursuit/collaborators{/collaborator}",
"teams_url": "https://api.github.com/repos/purescript/pursuit/teams",
"hooks_url": "https://api.github.com/repos/purescript/pursuit/hooks",
"issue_events_url": "https://api.github.com/repos/purescript/pursuit/issues/events{/number}",
"events_url": "https://api.github.com/repos/purescript/pursuit/events",
"assignees_url": "https://api.github.com/repos/purescript/pursuit/assignees{/user}",
"branches_url": "https://api.github.com/repos/purescript/pursuit/branches{/branch}",
"tags_url": "https://api.github.com/repos/purescript/pursuit/tags",
"blobs_url": "https://api.github.com/repos/purescript/pursuit/git/blobs{/sha}",
"git_tags_url": "https://api.github.com/repos/purescript/pursuit/git/tags{/sha}",
"git_refs_url": "https://api.github.com/repos/purescript/pursuit/git/refs{/sha}",
"trees_url": "https://api.github.com/repos/purescript/pursuit/git/trees{/sha}",
"statuses_url": "https://api.github.com/repos/purescript/pursuit/statuses/{sha}",
"languages_url": "https://api.github.com/repos/purescript/pursuit/languages",
"stargazers_url": "https://api.github.com/repos/purescript/pursuit/stargazers",
"contributors_url": "https://api.github.com/repos/purescript/pursuit/contributors",
"subscribers_url": "https://api.github.com/repos/purescript/pursuit/subscribers",
"subscription_url": "https://api.github.com/repos/purescript/pursuit/subscription",
"commits_url": "https://api.github.com/repos/purescript/pursuit/commits{/sha}",
"git_commits_url": "https://api.github.com/repos/purescript/pursuit/git/commits{/sha}",
"comments_url": "https://api.github.com/repos/purescript/pursuit/comments{/number}",
"issue_comment_url": "https://api.github.com/repos/purescript/pursuit/issues/comments{/number}",
"contents_url": "https://api.github.com/repos/purescript/pursuit/contents/{+path}",
"compare_url": "https://api.github.com/repos/purescript/pursuit/compare/{base}...{head}",
"merges_url": "https://api.github.com/repos/purescript/pursuit/merges",
"archive_url": "https://api.github.com/repos/purescript/pursuit/{archive_format}{/ref}",
"downloads_url": "https://api.github.com/repos/purescript/pursuit/downloads",
"issues_url": "https://api.github.com/repos/purescript/pursuit/issues{/number}",
"pulls_url": "https://api.github.com/repos/purescript/pursuit/pulls{/number}",
"milestones_url": "https://api.github.com/repos/purescript/pursuit/milestones{/number}",
"notifications_url": "https://api.github.com/repos/purescript/pursuit/notifications{?since,all,participating}",
"labels_url": "https://api.github.com/repos/purescript/pursuit/labels{/name}",
"releases_url": "https://api.github.com/repos/purescript/pursuit/releases{/id}",
"deployments_url": "https://api.github.com/repos/purescript/pursuit/deployments",
"created_at": "2014-08-04T04:57:54Z",
"updated_at": "2019-08-13T20:44:13Z",
"pushed_at": "2019-07-15T17:44:14Z",
"git_url": "git://github.com/purescript/pursuit.git",
"ssh_url": "git@github.com:purescript/pursuit.git",
"clone_url": "https://github.com/purescript/pursuit.git",
"svn_url": "https://github.com/purescript/pursuit",
"homepage": "https://pursuit.purescript.org/",
"size": 1252,
"stargazers_count": 109,
"watchers_count": 109,
"language": "Haskell",
"has_issues": true,
"has_projects": true,
"has_downloads": true,
"has_wiki": true,
"has_pages": false,
"forks_count": 42,
"mirror_url": null,
"archived": false,
"disabled": false,
"open_issues_count": 53,
"license": {
"key": "other",
"name": "Other",
"spdx_id": "NOASSERTION",
"url": null,
"node_id": "MDc6TGljZW5zZTA="
},
"forks": 42,
"open_issues": 53,
"watchers": 109,
"default_branch": "master",
"score": 108.295784
}, 
//cont...
```

1. A list of all Pokemon
Website URL: https://pokeapi.co/api/v2/pokemon/
JSON Body: 
```
{
"count": 964,
"next": "https://pokeapi.co/api/v2/pokemon/?offset=20&limit=20",
"previous": null,
"results": [
{
"name": "bulbasaur",
"url": "https://pokeapi.co/api/v2/pokemon/1/"
},
{
"name": "ivysaur",
"url": "https://pokeapi.co/api/v2/pokemon/2/"
},
{
"name": "venusaur",
"url": "https://pokeapi.co/api/v2/pokemon/3/"
//cont...
```

1. A list of all items in Fortnite
Website URL: https://fortnite-api.theapinetwork.com/store/get
JSON Body: 
```
{
"data": [
{
"itemId": "2fad344-834e456-dcf643d-91f9712",
"lastUpdate": 1553386039,
"store": {
"isFeatured": true,
"isRefundable": true,
"cost": "1500"
},
"item": {
"name": "Beastmode",
"description": "Gassed up and ready to roar.",
"type": "outfit",
"rarity": "epic",
"images": {
"icon": "https://fortnite-public-files.theapinetwork.com/outfit/c567e52c290292c99c7c9b44dd36827c.png",
"featured": "https://fortnite-public-files.theapinetwork.com/featured/2fad344-834e456-dcf643d-91f9712.png",
"background": "https://fortnite-public-files.theapinetwork.com/image/2fad344-834e456-dcf643d-91f9712.png",
"information": "https://fortnite-public-files.theapinetwork.com/image/2fad344-834e456-dcf643d-91f9712/icon.png"
},
"obtained_type": "vbucks",
"ratings": {
"avgStars": 3.66,
"totalPoints": 597,
"numberVotes": 163
}
}
},
//cont...
```

1. A list of all Game of Thrones Episodes.
Website URL: https://api.got.show/api/map/episodes
JSON Body: 
```
{
"message": "Success",
"data": [
{
"characters": [
"Viserys Targaryen",
"Catelyn Stark",
"Cersei Lannister",
"Jaime Lannister",
"Eddard Stark",
"Robert Baratheon",
"Jorah Mormont",
"Daenerys Targaryen",
"Jon Snow",
"Petyr Baelish",
"Arya Stark",
"Sansa Stark",
"Bran Stark",
"Robb Stark",
"Joffrey Baratheon",
"Tyrion Lannister",
"Jeor Mormont",
"Alliser Thorne",
"Jory Cassel",
"Barristan Selmy",
"Rodrik Cassel",
"Benjen Stark",
"Yoren",
"Renly Baratheon",
"Maester Aemon",
"Syrio Forel",
"Grenn",
"Irri",
"Pypar",
"Rakharo",
"Lancel Lannister"
],
"_id": "5cc0743604e71a0010b85729",
"director": "Tim Van Patten",
"airDate": "2011-04-24T04:00:00.000Z",
"totalNr": 2,
"season": 1,
"nr": 2,
"name": "The Kingsroad",
"predecessor": "Winter Is Coming",
"successor": "Lord Snow",
"createdAt": "2019-04-24T14:35:34.594Z",
"updatedAt": "2019-04-24T14:35:34.594Z",
"__v": 0
}, 
//cont...
```

1. A list of all songs with "Love" in the title.
Website URL: 
JSON Body: 

1. All information about Petyr Baelish from the Game of Thrones books
Website URL: https://www.anapioficeandfire.com/api/characters/823
JSON Body: 
```
{
"url": "https://anapioficeandfire.com/api/characters/823",
"name": "Petyr Baelish",
"gender": "Male",
"culture": "Valemen",
"born": "In 268 AC, at the Fingers",
"died": "",
"titles": [
"Master of coin (formerly)",
"Lord Paramount of the Trident",
"Lord of Harrenhal",
"Lord Protector of the Vale"
],
"aliases": [
"Littlefinger"
],
"father": "",
"mother": "",
"spouse": "https://anapioficeandfire.com/api/characters/688",
"allegiances": [
"https://anapioficeandfire.com/api/houses/10",
"https://anapioficeandfire.com/api/houses/11"
],
"books": [
"https://anapioficeandfire.com/api/books/1",
"https://anapioficeandfire.com/api/books/2",
"https://anapioficeandfire.com/api/books/3",
"https://anapioficeandfire.com/api/books/5",
"https://anapioficeandfire.com/api/books/8"
],
"povBooks": [],
"tvSeries": [
"Season 1",
"Season 2",
"Season 3",
"Season 4",
"Season 5",
"Season 6"
],
"playedBy": [
"Aidan Gillen"
]
}
```

1. All the movies Leonardo Dicaprio has acted in
Website URL: http://api.themoviedb.org/3/discover/movie?with_people=6193
JSON Body: 
```
{
"page": 1,
"total_results": 62,
"total_pages": 4,
"results": [
{
"popularity": 91.4,
"vote_count": 591,
"video": false,
"poster_path": "/8j58iEBw9pOXFD2L0nt0ZXeHviB.jpg",
"id": 466272,
"adult": false,
"backdrop_path": "/kKTPv9LKKs5L3oO1y5FNObxAPWI.jpg",
"original_language": "en",
"original_title": "Once Upon a Time in Hollywood",
"genre_ids": [
28,
35,
80,
18,
37
],
"title": "Once Upon a Time in Hollywood",
"vote_average": 7.7,
"overview": "A faded television actor and his stunt double strive to achieve fame and success in the film industry during the final years of Hollywood's Golden Age in 1969 Los Angeles.",
"release_date": "2019-07-26"
},
{
"popularity": 38.401,
"vote_count": 22905,
"video": false,
"poster_path": "/qmDpIHrmpJINaRKAfWQfftjCdyi.jpg",
"id": 27205,
"adult": false,
"backdrop_path": "/s2bT29y0ngXxxu2IA8AOzzXTRhd.jpg",
"original_language": "en",
"original_title": "Inception",
"genre_ids": [
28,
12,
878
],
"title": "Inception",
"vote_average": 8.3,
"overview": "Cobb, a skilled thief who commits corporate espionage by infiltrating the subconscious of his targets is offered a chance to regain his old life as payment for a task considered to be impossible: \"inception\", the implantation of another person's idea into a target's subconscious.",
"release_date": "2010-07-16"
},
{
"popularity": 42.491,
"vote_count": 1385,
"video": false,
"poster_path": "/AiRfixFcfTkNbn2A73qVJPlpkUo.jpg",
"id": 375588,
"adult": false,
"backdrop_path": "/axjFiijtxdfK3CD9dMwrdgLwblD.jpg",
"original_language": "en",
"original_title": "Robin Hood",
"genre_ids": [
28,
12,
53
],
"title": "Robin Hood",
"vote_average": 5.8,
"overview": "A war-hardened Crusader and his Moorish commander mount an audacious revolt against the corrupt English crown.",
"release_date": "2018-11-21"
},
//cont...
```
