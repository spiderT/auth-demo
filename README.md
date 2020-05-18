# 授权登录

本文以github和微信授权登录为例，学习相关授权登录知识

实质就是 OAuth 授权。用户想要登录 A 网站，A 网站让用户提供第三方网站的数据，证明自己的身份。获取第三方网站的身份数据，就需要 OAuth 授权。  

举例来说，A 网站允许 GitHub 登录，背后就是下面的流程。  

1. A 网站让用户跳转到 GitHub。
2. GitHub 要求用户登录，然后询问"A 网站要求获得 xx 权限，你是否同意？"
3. 用户同意，GitHub 就会重定向回 A 网站，同时发回一个授权码。
4. A 网站使用授权码，向 GitHub 请求令牌。
5. GitHub 返回令牌.
6. A 网站使用令牌，向 GitHub 请求用户数据。

## 1. github授权登录

### 1.1 应用登记

一个应用要求 OAuth 授权，必须先到对方网站登记，让对方知道是谁在请求。要先去 GitHub 登记一下。访问这个[网址](https://github.com/settings/applications/new)，填写登记表。

![登记](/images/github_1.png)

提交表单以后，GitHub 应该会返回客户端 ID（client ID）和客户端密钥（client secret），这就是应用的身份识别码。 
![登记](/images/github_2.png)

### 1.2  授权码

登录后，GitHub 询问用户，该应用正在请求数据，你是否同意授权。  

![授权](/images/github_3.png)


## 2. 微信授权登录


## 3. QQ登录

