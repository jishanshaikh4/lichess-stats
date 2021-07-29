## lichess-stats
Get your lichess.org player's data (periodically updated) into a JSON.

### Use

- Fork this repository.
- Generate lichess.org personal token and store at your forked repository's secrets.
- Update your personal/username text in ```.github/workflows/blank.yml```
- Your updated data will now update at ```_data/lichess-stats.json```on every push and daily at 5 AM UTC.


### Use on a Website

The content of `_data/lichess-stats.json` can be rendered into Jekyll site (md pages) as:

```
{{ site.data.lichess-stats.username }}
{{ site.data.lichess-stats.perfs.bullet.rating }}
```

### Template
The data will formatted into following template JSON:

```
{
    "id":"jishanshaikh4",
    "username":"jishanshaikh4",
    "online":true,
    "perfs":{
        "chess960":{
            "games":245,
            "rating":1794,
            "rd":58,
            "prog":-1
        },
        "antichess":{
            "games":13,
            "rating":1201,
            "rd":125,
            "prog":-47,
            "prov":true
        },
        "puzzle":{
            "games":3212,
            "rating":2052,
            "rd":68,
            "prog":0
        },
        "atomic":{
            "games":18,
            "rating":1118,
            "rd":112,
            "prog":-135,
            "prov":true
        },
        "racingKings":{
            "games":2,
            "rating":1406,
            "rd":276,
            "prog":0,
            "prov":true
        },
        "ultraBullet":{
            "games":819,
            "rating":1655,
            "rd":72,
            "prog":-8
        },
        "blitz":{
            "games":5046,
            "rating":2057,
            "rd":45,
            "prog":-8
        },
        "kingOfTheHill":{
            "games":50,
            "rating":1804,
            "rd":73,
            "prog":-4
        },
        "crazyhouse":{
            "games":25,
            "rating":1514,
            "rd":98,
            "prog":-3
        },
        "threeCheck":{
            "games":10,
            "rating":1335,
            "rd":141,
            "prog":0,
            "prov":true
        },
        "bullet":{
            "games":20193,
            "rating":2083,
            "rd":45,
            "prog":-4
        },
        "correspondence":{
            "games":1,
            "rating":1429,
            "rd":305,
            "prog":0,
            "prov":true
        },
        "classical":{
            "games":66,
            "rating":1765,
            "rd":79,
            "prog":17
        },
        "rapid":{
            "games":126,
            "rating":1907,
            "rd":62,
            "prog":-8
        },
        "storm":{
            "runs":49,
            "score":40
        },
        "streak":{
            "runs":109,
            "score":76
        }
    },
    "createdAt":1537866860821,
    "profile":{
        "country":"_united-nations",
        "firstName":"Jishan",
        "lastName":"Shaikh",
        "links":"https://www.facebook.com/zishan.shhaikh/\r\nhttps://www.quora.com/profile/jishan-shaikh-11/"
    },
    "seenAt":1625752140629,
    "playTime":{
        "total":3982556,
        "tv":4457
    },
    "language":"en-US",
    "url":"https://lichess.org/@/jishanshaikh4",
    "nbFollowing":124,
    "nbFollowers":53,
    "completionRate":100,
    "count":{
        "all":27424,
        "rated":26614,
        "ai":10,
        "draw":1297,
        "drawH":1297,
        "loss":13032,
        "lossH":13023,
        "win":13095,
        "winH":13094,
        "bookmark":12,
        "playing":0,
        "import":0,
        "me":0
    },
    "followable":true,
    "following":false,
    "blocking":false,
    "followsYou":false
}
```

