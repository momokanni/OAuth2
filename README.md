# OAuth2
OAuth2.0 定位：一个框架而不是单个协议  

### 授权码许可类型  
![授权码许可类型图](https://github.com/momokanni/OAuth2/blob/master/images/%E6%8E%88%E6%9D%83%E7%A0%81%E8%AE%B8%E5%8F%AF%E7%B1%BB%E5%9E%8B.png)   

### 隐式许可类型（适用场景：内嵌在网站上的JavaScript应用）  
![隐式许可类型](https://github.com/momokanni/OAuth2/blob/master/images/%E9%9A%90%E5%BC%8F%E8%AE%B8%E5%8F%AF%E7%B1%BB%E5%9E%8B%20(1).jpg)  
>1. 直接从授权端点返回令牌  
>2. 只使用前端信道和授权服务器通信  
>3. 不可用于获取刷新令牌，因为浏览器具有短暂运行的特点，只会在被加载到浏览器的期间保持会话，所以刷新令牌在这里的作用非常有限。  
>4. 客户端向授权服务器的授权码端点发送请求时，使用的方式和授权码流程相同，只不过response_type : 'token' 而不是code，这样会通知授权服务器直接生成令牌。  

### 客户端凭据许可类型  
![客户端凭据许可类型](https://github.com/momokanni/OAuth2/blob/master/images/%E5%AE%A2%E6%88%B7%E7%AB%AF%E5%87%AD%E6%8D%AE%E8%AE%B8%E5%8F%AF%E7%B1%BB%E5%9E%8B.jpg)  

### 资源拥有者凭据许可类型（密码流程） 不推荐！！！   
![资源拥有者凭据许可类型](https://github.com/momokanni/OAuth2/blob/master/images/%E8%B5%84%E6%BA%90%E6%8B%A5%E6%9C%89%E8%80%85%E5%87%AD%E6%8D%AE%E8%AE%B8%E5%8F%AF%E7%B1%BB%E5%9E%8B.jpg)  

### 断言许可类型  
![ 断言许可类型](https://github.com/momokanni/OAuth2/blob/master/images/%E6%96%AD%E8%A8%80%E8%AE%B8%E5%8F%AF%E7%B1%BB%E5%9E%8B_UML.jpg)  



