
## 峰值脚本压测
### 那个模块压测情况
| 模块    | 并发数据 | 
| :------- | :---- | 
| pivotor_iauth_api | summary = 57553848 in 05:55:19 = 2699.6/s Avg:    17 Min:     1 Max: 50594 Err:     0 (0.00%)
 | 
| pivotor_iauth_api_user    | summary = 92845566 in 06:06:19 = 4224.2/s Avg:    37 Min:     2 Max: 37042 Err:     0 (0.00%)|  
| incoming   |summary = 28776280 in 03:13:32 = 2478.2/s Avg:  3643 Min:     7 Max: 39316 Err:     0 (0.00%)|  
| callpermission     |summary = 466803 in 03:04:12 =   42.2/s Avg:  1424 Min:     0 Max: 92791 Err:  1749 (0.37%)| 
| dating压测     |summary = 13937378 in 03:10:24 = 1220.0/s Avg:  1087 Min:     0 Max: 199368 Err: 47414 (0.34%)| 
| dating压测_meetingDepts     |summary = 20009119 in 03:09:40 = 1758.3/s Avg:   768 Min:     0 Max: 214848 Err: 50278 (0.25%)| 
| datafact     |summary = 1635690 in 05:02:55 =   90.0/s Avg:    15 Min:     1 Max:  5043 Err:     0 (0.00%)| 
| liveAutoTest     |summary = 20334752 in 05:03:13 = 1117.7/s Avg:   165 Min:     0 Max: 31001 Err: 3401896 (16.73%)| 
| pre_buffet_3_interfaces     |summary = 13961967 in 05:03:49 =  765.9/s Avg:    30 Min:     4 Max: 301007 Err:     3 (0.00%)| 
| logserver_bigdata     |summary = 803951 in 04:57:45 =   45.0/s Avg:     3 Min:     2 Max:   520 Err:     0 (0.00%)
    | 
| meetingroomchargebill     |summary = 61549500 in 05:07:41 = 3334.0/s Avg:    29 Min:     1 Max:  4056 Err:     0 (0.00%)
    | 
| recording     |summary = 275947 in 05:06:37 =   15.0/s Avg:    73 Min:    14 Max:  3150 Err:     0 (0.00%)
| 
| Vote_Interface_Test     |summary = 4092927 in 01:59:28 =  571.0/s Avg:    52 Min:     2 Max: 11872 Err:     0 (0.00%)
    | 
| case1创建签到_linux     |summary =  51067 in 00:45:18 =   18.8/s Avg:  3190 Min:  1047 Max: 20152 Err:     0 (0.00%)
    | 
| case2创建答题_linux     |summary =  27233 in 00:44:28 =   10.2/s Avg:  5871 Min:  2299 Max: 29750 Err:     0 (0.00%)
    | 
| case3签到_linux     |summary =  51485 in 00:44:47 =   19.2/s Avg:  3127 Min:  1054 Max: 17199 Err:     0 (0.00%)
    | 
| case4答题_linux     |summary =  28292 in 00:45:30 =   10.4/s Avg:  5781 Min:  2192 Max: 26148 Err:     0 (0.00%)
    |   
| case4答题_linux     |summary =  28292 in 00:45:30 =   10.4/s Avg:  5781 Min:  2192 Max: 26148 Err:     0 (0.00%)
    | 
    

### 接口平均响应时间大于3s的接口

| 接口     | 平均响应时间 |
| :------- | :---- | 
| http://10.44.14.173:8080/api/rest/v1/en/vote    | 5680  |  
| http://10.44.14.173:8080/api/rest/v1/en/vote/sign     | 3017    |  
|http://10.44.14.173:8080/api/rest/v1/en/vote/answer     | 5658    | 

### 压力下实际终端显影情况

| 模块     | 响应s |
| :------- | :---- | 
| contact加载（客户端）   | 2-5  |  
|   选人组建（管理平台）   | 2-5    |  
|我的会议加载（客户端）     | 7-8    | 
|我的直播加载 （客户端）    | 7-8    | 
|预约会议，会控基本功能|正常|
|等管理平台基本操作|正常|


### 当前存在的问题

 1. presence服务有问题，未启动
 2. incoming脚本星影时间较长，并发上不去
 3. 会控的脚本并发上不去，接口平均响应时间2s+
 4. 直播模块脚本报错，具体问题未知，已反馈（和开发约好明天一起看一下）

    
    
    
    
    
    
    
    
    
    
    
    