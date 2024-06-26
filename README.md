由于时间问题，本次设计只做了后端的部分接口



#### 注册功能

![image-20240114211349038](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114211349038.png)

若注册成功返回![image-20240114211454858](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114211454858.png)

并且数据库生成对应数据并对密码加密处理![image-20240114211527155](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114211527155.png)

若注册已经被使用过的用户名则返回![image-20240114211600024](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114211600024.png)





#### 登录功能

![image-20240114211636006](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114211636006.png)

若登录成功则返回![image-20240114211703606](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114211703606.png)

其中data是登录后生成的令牌



若密码错误则返回![image-20240114211743958](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114211743958.png)



若用户名不存在则返回![image-20240114211800897](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114211800897.png)



#### 获取用户信息

![image-20240114211838331](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114211838331.png)

此接口可返回当前用户信息

![image-20240114211937098](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114211937098.png)





#### 更新用户基本信息

![image-20240114212059100](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114212059100.png)

更新完成后当前用户信息为![image-20240114212126244](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114212126244.png)





#### 更新用户金额

主要用于完成充值和消费

![image-20240114212429338](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114212429338.png)

更新完成后当前用户信息为：

![image-20240114212507078](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114212507078.png)







#### 添加菜品

![image-20240114212642963](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114212642963.png)

操作完成后数据库![image-20240114212705673](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114212705673.png)





#### 按类分类查看菜单

![image-20240114212853130](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114212853130.png)

结果：

![image-20240114212909645](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114212909645.png)

-----------------------------------------------------------------------------------------------------------------

![image-20240114212947051](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114212947051.png)

结果：





![image-20240114212935161](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114212935161.png)







#### 选菜

![image-20240114213211943](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213211943.png)

操作完成后对应表数据：

![image-20240114213236758](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213236758.png)





#### 查看目前已点菜品



![image-20240114213303518](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213303518.png)

结果：

![image-20240114213318864](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213318864.png)





#### 提交订单并支付

![image-20240114213400001](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213400001.png![image-20240114213452659](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213452659.png)

由于金额不够提示返回

![image-20240114213516746](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213516746.png)

充值后再提交订单

![image-20240114213557122](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213557122.png)

原表中的数据转移到订单表中

![image-20240114213626994](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213626994.png)

![image-20240114213643578](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213643578.png)





#### 查看订单

![image-20240114213711974](C:\Users\16006\AppData\Roaming\Typora\typora-user-images\image-20240114213711974.png)