
# 天气预报软件说明书 #


 ## 项目介绍 ##


> 摘要：本设计使用Android设计技术开发了一种运用在Android系统上的手机天气预报软件，通过该软件可选择地区来获得天气，温度等信息。
> 功能介绍：
1. 遍历全国省市县数据
2. 显示天气信息
3. 手动切换城市
4. 后台自动更新天气

## 我的模块 ##
### 显示天气信息 ###
>先定义GSON实体类，再在Utility类中添加handleWeatherResponse（）方法用于解析天气JSON数据，最后通过fromJSon（）方法将JSON数据转化成Weather对象。在WeatherActivity类中，通过onGreate（）方法获得一些控件的事例，然后尝试从本地缓存中读取天气数据。如果没有从Intent中取出天气id，并调用requestWeather（）方法从服务器请求天气数据。
