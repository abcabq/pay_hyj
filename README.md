# pay_hyj

## 相关文档

* [蚂蚁金服开放平台](https://openhome.alipay.com/platform/appManage.htm)
* [支付宝支付](https://docs.open.alipay.com/204/105051/)
* [支付宝登录](https://docs.open.alipay.com/218/105329/)
* [应用签名工具](https://opendocs.alipay.com/open/common/104062)

## 开始使用

### Android

```
# 不需要做任何额外接入工作
# 混淆已打入 Library，随 Library 引用，自动添加到 apk 打包混淆
```
 
 

### iOS

```
# 不需要做任何额外接入工作
# 配置已集成到脚本里
```

* UTDID冲突的问题解决方案

```diff
alipay_kit:
+  ios: noutdid # 默认 utdid
```


* 安装（仅iOS）

```shell
# step.1 安装必要依赖
sudo gem install plist
# step.2 切换工作目录，插件里为 example/ios/，普通项目为 ios/
cd example/ios/
# step.3 执行脚本
pod install
```

## 示例

[示例](./example/lib/main.dart)