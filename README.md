GesturePassword
====================
iOS手势密码
------------------------
一个ios手势密码功能实现

ipad/iphone 都可以用

没有使用图片，里面可以通过view自己添加

keychain做的数据持久化，利用苹果官方KeychainItemWrapper类

**keychain存储的数据不会因为删除app而清除记录，请调用`-(void)clear`清除储存密码。**

### 简单使用方式

下载后直接把 GesturePassword 下的GesturePassword文件丢到项目中去

**在 TARGETS - Build Phases - "KeychainItemWrapper.m" - Compiler Flags (-fno-objc-arc)**

在需要的地方直接可以调用ViewController

第一次的时候会两次验证密码

以后便会以这个密码进行确认

清空密码可以调用 `- (void)clear`

`- (void)verify` 验证手势密码在这里

`- (void)reset` 重置手势密码在这 （第一次回调用到这里进行第一次设置


### TODO
* ~~*完善提示标签*~~
* ~~*添加头像*~~
* ~~*添加忘记按钮*~~

