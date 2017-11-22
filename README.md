# JAVA WAR APP buildpack

云帮为了让您更方便的部署项目，特推出识可别 **WAR包** 的构建模式- **JAVA WAR APP buildpack** 。

## 工作原理

当buildpack在您的代码根目录检测到格式为`<文件名>.war`的 **WAR包** 文件，该应用被识别为WAR项目，我们称为Java-war。

## 文档

以下文章了解更多：

- [云帮支持Java](https://www.rainbond.com/docs/stable/user-lang-docs/java/lang-java-overview.html)
- [云帮部署WAR包应用](https://www.rainbond.com/docs/stable/user-lang-docs/java/lang-java-war.html)

## 配置

### 默认环境

buildpack构建环境默认使用 **JDK 1.8**版本。

默认启动程序为 **webapp-runner-7.0.57.2  (tomcat)**

### Procfile文件内容

```
web: java -cp config/:lib/*.jar:bin/.class Example
```

## 授权

根据 MIT 授权证获得许可。 请参阅LICENSE文件
