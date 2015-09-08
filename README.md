# zhihu
仿の知乎Web。
OMG，功能以及细节太多了。我只能页面模仿一下，功能挑最主要的做先。

## 问题
* 抓了知乎登录的包，发现是明文账号密码。。但是我这个demo就不用https了。
* RESTful,表单提交不支持put,delete,就用post代替，用ajax的时候满足RESTful风格。
* 目前响应式支持很糟糕。
* js/css都没有压缩，sass只用了简单的嵌套功能，js没有模块化
* 做完这个项目，学习一个gulp构建工具
* 想找个实习，想要团队合作，想要与牛人为伍。
* 聚合索引，排序~~~Topic那里要改。

## 功能-我喜欢的小细节
* 注册登录
    * 密码md5简单加盐加密
    * cookie签名，防篡改
    * 邮箱或手机号任意注册
    * 记住密码，可注销。
    * 权限中间件------------还要完善
* 提问
* 评论
    * 点赞！！
* 首页
    * 点击回答 会跳到该问题该回答处，页面被黄色覆盖渐变效果
* 问题页面
    * 日期（根据提交时间，格式：今天的显示【20:00】，昨天的显示【昨天20:00】，之前的显示【2015-08-31】）
* 404小彩蛋--最后加在app.js

## 正在做
* 登录页-md5 √
* 主页
    * top栏-user
* 提问
    * 提问 √
    * 评论 √
    * 点赞和顶下去
    * tag /tag/:tag
* 回答
* 话题 /topic
* 发现 /explore
* 消息 /message


## 没处理好、要改的细节
* 话题页
* 注册、登录、提交问题都改成ajax
* 把权限登录改成中间件的形式 √
* 提问、回答没有换行-编辑器的锅！
* 注册错误，重定向回来的时候，没有切换到注册Tab √
* index顶部navbar，用户下拉菜单的宽度 √   
* 记住密码，还没做！√


## 将要做的
* 富文本编辑器-先搁置，等基本功能都实现了再来完成这个
* 社交账号登录