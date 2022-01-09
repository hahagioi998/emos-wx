记录下学习进度

慕课网课程地址：
https://coding.imooc.com/class/485.html

项目名：SpringBoot 在线协同办公小程序开发 全栈式项目实战

开发工具：微信小程序开发工具 + HBuilderX + IDEA

技术栈：

![202201092237_29](http://cdn.xiongsihao.com/202201092237_29.png)

主流程逻辑图：

![202201092237_29](http://cdn.xiongsihao.com/202201092239_719.png)

![](http://cdn.xiongsihao.com/202201092243_656.png)

- 签到页面利用微信API实现签到自拍和重拍功能，并且封装检测用户是否可以签到的函数。企业签到的难点在于经常有换休和调休的工作日和节假日，判定某员工可否签到既要考虑特殊节假日和调休，还要结合考勤时间。

- 利用人脸识别技术为新员工创建人脸模型数据，签到的时候根据人脸模型数据比对签到人是否是员工本人，并且根据签到人所在GPS定位，智能判断该地区的新冠疫情风险等级。如果是高风险地区就自动发送告警邮件，安排人员隔离。

- 使用可视化VUE图形页面统计员本周工正常、迟到和旷工的考勤数据。

- 利用RabbitMQ缓存消息数据，用户登陆的时候，使用异步线程向数据库写入未读消息，错峰实现消息加载。

- 利用Activiti工作流实现会议的审批和管理，工作流的发起、流转和回退。结合消息通知模块，每次增减会议人员的时候，都需要动态计算前后人员交集和补集。交集人员不需要重复通知，补集人员还要区分哪些人不需要参会，哪些人是新增参会人员，然后发出不同的通知消息。

- 微信小程序上面视频会议只有腾讯云的TRTC这唯一的方案，开通TRTC服务，利用SDK程序包，在小程序上面实现在线会议功能，并且对参会迟到人员生成罚款单。

- 利用腾讯云CVM、COS、数据库等服务，部署Emos在线办公系统

  