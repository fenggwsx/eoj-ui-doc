# 排行榜

用于显示用户比赛积分和EMB余额的排名

## 积分排行榜/EMB排行榜

分别根据用户积分和EMB进行排名，每个用户包括以下数据：

- 排名（整数）
- 用户信息（包括用户名，头像和Magic）
- 拥有的积分/EMB
- 总通过题目数（整数，目前只有大富翁榜有这个字段）

下面列出一位用户积分排名的`json`数据作为例子：

```json
{
    "id": 2200,
    "username": "palayutm",
    "magic": "legendary",
    "avatar": "https://xxx.example.com/avatar/2200.png",
    "rating": 2184,
    "rank": 3
}
```

下面再列出一位用户EMB排名的`json`数据作为例子：

```json
{
    "id": 12997,
    "username": "fanqiexi",
    "magic": "orange",
    "avatar": "https://xxx.example.com/avatar/12997.png",
    "score": 5248.47284515354,
    "rank": 3,
    "ac_distinct_count": 1024
}
```
