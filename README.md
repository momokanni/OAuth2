# OAuth2
OAuth2.0 授权协议

### 授权码许可类型  
![授权码许可类型图](https://github.com/momokanni/OAuth2/blob/master/images/%E6%8E%88%E6%9D%83%E7%A0%81%E8%AE%B8%E5%8F%AF%E7%B1%BB%E5%9E%8B.png)   

### 隐式许可类型（适用场景：内嵌在网站上的JavaScript应用）  
>1. 直接从授权端点返回令牌  
>2. 只使用前端信道和授权服务器通信  
>3. 不可用于获取刷新令牌，因为浏览器具有短暂运行的特点，只会在被加载到浏览器的期间保持会话，所以刷新令牌在这里的作用非常有限。  
>4. 客户端向授权服务器的授权码端点发送请求时，使用的方式和授权码流程相同，只不过response_type : 'token' 而不是code，这样会通知授权服务器直接生成令牌。  

