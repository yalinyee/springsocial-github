# Github社交联合登录

# 步骤

### 1. 创建开发者应用

登录GitHub,【Settings】--> 【Developer settings】-->【OAuth Apps】-->【New Oauth App】，然后填写应用信息。

**注意：Authorization callback URL** 填写【**<http://localhost:8080/connect/github>**】

### 2. 在github上注册开发者应用获取Client Credentials

获取Client ID 和Client Secret 

### 3. 更新social-github应用配置文件

根据上一步获得的Client Credentials替换你的**app-id**和**app-secret**

```
spring.social.github.app-id=YOUR_APP_ID
spring.social.github.app-secret=YOUR_APP_SECRET
```

