## IOC容器和Beans介绍
IOC(inversion of control)也叫依赖注入(DI, dependency injecton).对象仅仅通过构造器参数、工厂方法参数、设置由构造或者工厂方法返回的实例的属性来定义与其它对象的依赖关系。

核心包org.springframework.beans与org.springframework.context。BeanFactory 接口提供了一种能够管理任何类型对象的高级配置机制。ApplicationContext 是 BeanFactory 的一个子接口。 
它新增了：1、Easier integration with Spring’s AOP features  2、Message resource handling (for use in internationalization)  3、Event publication  4、Application-layer specific contexts such as the WebApplicationContext for use in web applications.


## 容器概述
元数据的配置主要有XML和注解，要使用注解需要再在XMLV中开启
对于org.springframework.context.ApplicationContext，spring,spring提供了若干实现，在独立应用程序中，通常创建 ClassPathXmlApplicationContext 或 FileSystemXmlApplicationContext 的实例。
<img width="1271" alt="截屏2021-11-19 下午3 57 12" src="https://user-images.githubusercontent.com/63908432/142586353-525d4076-51b7-44ea-b829-9db9b975fd8f.png">

### Configuration Metadata
