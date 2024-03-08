1.说一下jvm的类加载机制？
jvm的类加载采用双亲委派机制，加载一个类时首先请求父类加载器进行加载，如果父加载器无法加载该类，再尝试使用子加载器进行加载。

2.类加载器名称和双亲委派模型？
启动类加载器rt.jar、扩展类加载器 jre lib、应用类加载器 程序相关的类、自定义类加载器。

3.如何打破双亲委派模型？ 
自定义类加载器在实现加载方法时，不要首先调用父加载器的加载方法super.loadClass(ClassName)。

4.如何实现自定义的类加载器？ 
继承ClassLoader类，实现findClass方法。

5.常见框架的类加载器设计？ 
Tomcat 为每个webapp单独创建了一个独立的类加载器，并先尝试加载应用自己的类，失败后再请求父加载器。避免多个web应用之间类冲突问题。
Spring 提供了基于优化类型匹配的依赖注入的性能。
ResolvableType缓存了类的类型信息 beanDefinitionMap缓存了Bean定义的信息，加快了Bean定义的性能。

6.JDBC加载过程？
加载JDBC驱动类、创建JDBC驱动类实例并将实例注册到DriverManager中、提供数据库的相关信息获取连接。

7.什么是SPI机制？ 
Service Provider Interface是JAVA提供的服务发现加载机制
