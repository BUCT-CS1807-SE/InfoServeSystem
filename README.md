# InfoServeSystem

信息服务子系统，周记、文档在WiKi里。用于提供数据服务，并针对用户特征作个性化推送(说不定整不出来)。

## 后台管理

记录用户活跃轨迹，统计应用日活数。


## 信息接口

没有数据，不知道咋写接口


## 返回数据格式

JSON：
```json
{
  "status":"OK|ERR",
  "response-time":"2021-04-04 22:50"
  "data":{
    "arr-data":[],
    "obj-data":{},
    "string-data:"",
    "num-data":1,
  },
}
```

请求方式为get

data内相应参数为返回数据，命名格式为小写加'-'。

返回的时间为String类型

## 提交数据格式

JSON：
```json
{
  "request-uuid":用户凭证,
  "data":{
    "arr-param":[],
    "obj-param":{},
    "string-param:"",
    "num-param":1,
  },
}
```

用户凭证为用户登录后下发的登录凭证，没有凭证就是没有登陆用户，需要后台组提供接口验证用户凭证是否合法有效



