---
sidebar_position: 3
---

# 比赛/作业

主要用于显示比赛列表/作业列表

## 比赛/作业列表

用于显示本网站所举办的比赛或者教师发布的一些作业，对于每一条比赛/作业（由于二者非常相似，以下简称比赛），主要包含以下数据：

- 比赛名称（字符串）
- 比赛时间（包括开始时间和结束时间，时间可为空，若都为空则为长期比赛）
- 访问权限
- 比赛作者/管理员
- 参加人数（整数）

下面列出一条比赛的json数据作为例子：

```json
{
    "id": 702,
    "title": "《编程思维与实践》课程练习",
    "start_time": "2024-01-28T05:00:00Z",
    "end_time": "2024-01-28T08:00:00Z",
    "authors": [
        {
            "id": 92580,
            "username": "fenggwsx",
            "magic": "teal",
            "avatar": "https://xxx.example.com/avatar/92580.png"
        },
        {
            "id": 58681,
            "username": "Once",
            "magic": "grey",
            "avatar": "https://xxx.example.com/avatar/58581.jpg"
        }
    ],
    "access_level": 10,
    "status": 1,
    "participants_count": 19,
    "scoring_method": "oi"
}
```

## 分数排行榜（可选）

显示高分用户排行榜，一般显示前10名或前20名（Rating分数是通过比赛获得的），包含以下数据：

- 用户名称
- 分数（整数，一般在几千）

下面列出一位用户排名的json数据作为例子：

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
