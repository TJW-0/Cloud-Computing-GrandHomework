# springboot基于SSM的简单的仓库管理系统

#### 介绍
springboot基于SSM的简单的仓库管理系统

#### 技术栈
基于spring boot的SSM的项目，前端：thymeleaf＋bootstrap　光年模板改的
后端是SSM那一套；引入了druid做数据库连接池并可以监控数据库SQL执行时间等等
 
#### 系统功能
登录：通过前端页面表单提交数据到后端相应接口处，并进行调用后端方法执行相应程序；程序自上而下执行，将从前端拿到的数据以对象的形式传入，在sql中进行查询操作，以对象的形式返回数据，进行判断是否登录成功，并如果登录成功，则控制页面跳转，并将数据保存到session中。
前端页面上做了一些js判断操作，比如 用户名，密码不能为空，最少几位。
这样就不符合前后端分离的思想，上一个项目，采用的AJAX做的前端控制页面跳转，后端只关注于数据。

注册：就是插入数据，返回int 受影响的行数，进行判断是否注册成功。

查询个人信息：通过session获取用户名 然后通过用户名查询一整条数据,并通过model的方式将数据返回前端进行页面渲染。

修改个人信息：修改的信息传到后端对象中，sql通过ID来进行更新操作。

修改密码：通过传入新密码和旧密码在在sql中通过ID来进行密码的修改，逻辑为先通过session拿到对应用户,然后匹配是否原密码，然后得到ID进行修改操作，如果匹配错误，将modal中的错误消息传输渲染到前端页面。
#### 安装教程

1.  xxxx
2.  xxxx
3.  xxxx

#### 使用说明

1.  xxxx
2.  xxxx
3.  xxxx

#### 参与贡献

1.  Fork 本仓库
2.  新建 Feat_xxx 分支
3.  提交代码
4.  新建 Pull Request


#### 特技

1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
