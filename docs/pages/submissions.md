---
sidebar_position: 3
---

# 提交记录

用户可在此查看自己或所有人的提交

## 提交记录列表

用于显示用户提交代码的历史记录和相应的评测结果，需要支持根据`题目名称`、`用户名`、`自己/所有人`、`编程语言`、`评测状态`进行筛选，对于每一条提交记录，包含以下数据：

- 用户信息（包括用户名，头像）
- 提交时间（精确到秒）
- 题目名称（格式为：题目ID.题目名称）
- 所使用的编程语言
- 测评序号
- 测评状态/结果
- 测评数据（包括耗时和内存使用量）
- 来自的比赛（如果来自题目集则为null）*
- 是否可见（不可见则不显示，与UI设计无关）

注*：一条提交记录可能产生自题目集中，也可能产生自比赛，原来获取提交记录详情的接口是分开的，因此需要这个数据进行判断，但是现在接口已经合并，这个字段已经失去作用了

下面列出一条提交记录的json数据作为例子：

```json
{
    "id": 3394236,
    "create_time": "2024-04-17T14:27:31.750983Z",
    "author": {
        "id": 92580,
        "username": "fenggwsx",
        "magic": "teal",
        "avatar": "http://api.aiecnu.cn/avatar/avatar_Yt072gn.png"
    },
    "problem": {
        "id": 4951,
        "title": "查找整数"
    },
    "lang": "cc20",
    "lang_name": "C++20",
    "status": -1,
    "status_test": 1,
    "status_time": 0.0,
    "status_memory": 1.082,
    "contest": null,
    "contest_time": null,
    "status_percent": 0.0,
    "judge_end_time": "2024-04-17T14:27:32.074311Z",
    "visible": true
}
```
