# CJBlog - Spring Boot 博客项目

欢迎使用CJBlog，这是一个基于Spring Boot 3.2.0构建的博客系统。

## 项目特性

- 基于Spring Boot 3.2.0构建
- 使用Java 21开发
- 内置Tomcat服务器，默认端口8080
- RESTful API架构

## 项目结构

```
CJBlog/
├── src/
│   ├── main/
│   │   ├── java/cn/homecj/
│   │   │   ├── Main.java              # Spring Boot启动类
│   │   │   └── controller/
│   │   │       └── HelloController.java # 示例控制器
│   │   └── resources/
│   │       └── application.properties # 应用配置文件
├── pom.xml                            # Maven配置文件
└── README.md                          # 项目说明文档
```

## 快速开始

### 环境要求

- Java 21+
- Maven 3.6+

### 运行项目

1. 克隆项目到本地
2. 在项目根目录执行以下命令：
   ```bash
   mvn spring-boot:run
   ```

3. 访问以下地址验证服务：
   - 主页: http://localhost:8080
   - 示例API: http://localhost:8080/hello

### 构建项目

要构建可执行的JAR文件，请运行：
```bash
mvn clean package
```

构建完成后，在`target`目录下会生成可执行的JAR文件，可通过以下命令运行：
```bash
java -jar target/CJBlog-1.0-SNAPSHOT.jar
```

## 当前实现

- `/` - 返回欢迎信息
- `/hello` - 返回示例信息

## 技术栈

- Spring Boot 3.2.0
- Spring Web MVC
- Java 21
- Maven
- Embedded Tomcat

## 开发说明

此项目已配置为标准的Spring Boot项目，您可以继续添加新的控制器、服务、数据访问层等组件来扩展功能。