# React Assignment - Fake Twitter

> Inspired by [ThaddeusJiang/react-assignments/fake-twitter](https://github.com/ThaddeusJiang/react-assignments/tree/main/fake-twitter#react-assignment---fake-twitter).

## 1. 目标
使用React创建一个简化版的twitter web app。

## 2. 功能需求
- [ ] 注册
- [ ] 登陆
- [ ] CRUD tweets

## 3. 项目要求
### 3.1 API Mock
对于react components所使用的后端API，无需开发具体的逻辑，请使用[msw](https://mswjs.io/)（或其他mock服务）进行mock，详见msw的[参考文档](https://mswjs.io/docs/getting-started/mocks/rest-api)。

下面列举了此项目所需要使用的API，以供参考。您可以根据自身的设计进行调整。
* login
* register
* fetchTweets
* createTweet
* updateTweet
* deleteTweet

### 3.2 用户流程
1. 用户打开APP后，在未登陆的状态下，首先进入登陆页面；
2. 在登陆页面，用户输入用户名、密码进行登录；
3. 对于未注册用户，可以在登陆页面点击链接跳转到注册页面；
4. 在注册页面，用户输入用户名、密码进行注册；
5. 在登陆成功或注册成功后，用户进入主页;

### 3.3 CRUD tweets
1. 用户在主页可以进行三类操作
   1. 查看10条tweets（由fetchTweets api返回）
   2. 创建一个新的tweet（调用createTweet api）
   3. 点击10条tweets中的一个，进入该tweet的详细页面
2. 在tweet详细页面，用户可以进行编辑（并保存）和删除该tweet的操作
   * 删除该条tweet后将自动返回到主页

## 4. 视觉效果
1. 对于一个tweet的呈现，只需呈现tweet的文字内容即可，tweet的发布时间、发布人等信息，无需呈现
2. 对于tweet的创建、编辑以及删除，设计一个简单的视觉效果即可
3. 此项目中视觉效果不是考察重点，**前端逻辑的实现**是考察重点

## 5. Frameworks
使用开源的框架进行开发是完全OK的！

除了传统的视觉框架[Bootstrap](https://getbootstrap.com/)，我们也推荐使用React框架，包括但不限于，

* [Next.js](https://nextjs.org/)
* [RedwoodJS](https://redwoodjs.com/)
* [Create React App](https://create-react-app.dev/)
* [Gatsby](https://www.gatsbyjs.com/)
* [Blitz](https://blitzjs.com/)

## 6. 其他说明
1. 除项目完成度外，**代码质量**也是我们的考察重点
2. tweet crud操作中，无需考虑用户权限，包括但不限于什么用户可以查看什么tweets
3. 项目提交方式是将您的code push到一个我们可以访问的repo中，并通过邮件告知我们repo的地址