### Spring Cloud





![img](https://spring.io/img/homepage/icon-spring-cloud.svg)



## 协调任何事项：简化分布式系统

构建分布式系统不需要复杂且容易出错。 Spring Cloud为最常见的分布式系统模式提供了简单易用的编程模型，帮助开发人员构建弹性，可靠和协调的应用程序。 Spring Cloud构建于Spring Boot之上，使开发人员可以轻松入门并快速提高工作效率。

![img](https://spring.io/img/homepage/diagram-distributed-systems.svg)



[ Spring Cloud Reference Manual](https://cloud.spring.io/spring-cloud-static/current/)(Spring Cloud参考手册)

入门指南

[ Config(配置)](https://spring.io/guides/gs/centralized-configuration/)

[ Registry](https://spring.io/guides/gs/service-registration-and-discovery/)(注册)

[Breakers](https://spring.io/guides/gs/circuit-breaker/)(断路器)

[Load Balancing](https://spring.io/guides/gs/client-side-load-balancing/)(负载均衡)

[ Routing](https://spring.io/guides/gs/routing-and-filtering/)(路由)

Spring Cloud为开发人员提供了快速构建分布式系统中一些常见模式的工具（例如配置管理，服务发现，断路器，智能路由，微代理，控制总线，一次性令牌，全局锁定，领导选举，分布式 会话，集群状态）。 分布式系统的协调导致锅炉板模式，使用Spring Cloud开发人员可以快速站起来实现这些模式的服务和应用程序。 它们适用于任何分布式环境，包括开发人员自己的笔记本电脑，裸机数据中心和Cloud Foundry等托管平台。

#### 特征

Spring Cloud专注于为典型用例提供良好的开箱即用体验，并为其他用户提供可扩展性机制。



- 分布式/版本化配置
- 服务注册和发现
- 路由
- 服务到服务的调度
- 负载均衡
- 断路器
- 全局锁
- 领导选举和集群国家
- 分布式消息

Spring Cloud采用非常声明的方法，通常只需更改类路径和/或注释即可获得许多功能。 作为发现客户端的示例应用程序：

```java
@SpringBootApplication
@EnableDiscoveryClient
public class Application {
	public static void main(String[] args) {
		SpringApplication.run(Application.class, args);
	}
}
```

### 主要项目

### [Spring Cloud Config](https://cloud.spring.io/spring-cloud-config)

由git存储库支持的集中式外部配置管理。 配置资源直接映射到Spring Environment，但如果需要，可以由非Spring应用程序使用。

### [Spring Cloud Netflix](https://cloud.spring.io/spring-cloud-netflix)

与各种Netflix OSS组件集成（Eureka，Hystrix，Zuul，Archaius等）。

### [Spring Cloud Bus](https://cloud.spring.io/spring-cloud-bus)

用于将服务和服务实例与分布式消息传递链接在一起的事件总线 用于跨群集传播状态更改（例如，配置更改事件）。

### [Spring Cloud Cloudfoundry](https://cloud.spring.io/spring-cloud-cloudfoundry)

将您的应用程序与Pivotal Cloud Foundry集成。 提供服务发现实现，还可以轻松实现受SSO和OAuth2保护的资源。

### [Spring Cloud Open Service Broker](https://cloud.spring.io/spring-cloud-open-service-broker)

提供构建实现Open Service Broker API的服务代理的起点。

### [Spring Cloud Cluster](https://github.com/spring-cloud/spring-cloud-cluster)

领导者选举和共同的有状态模式与Zookeeper，Redis，Hazelcast，Consul的抽象和实现。

### [Spring Cloud Consul](https://cloud.spring.io/spring-cloud-consul)

Hashicorp Consul的服务发现和配置管理。

### [Spring Cloud Security](https://cloud.spring.io/spring-cloud-security)

为Zuul代理中的负载平衡OAuth2 rest客户端和身份验证头中继提供支持。

### [Spring Cloud Sleuth](https://cloud.spring.io/spring-cloud-sleuth)

Spring Cloud应用程序的分布式跟踪，与Zipkin，HTrace和基于日志（例如ELK）的跟踪兼容。

### [Spring Cloud Data Flow](https://cloud.spring.io/spring-cloud-dataflow)

适用于现代运行时的可组合微服务应用程序的云本机编排服务。 易于使用的DSL，拖放式GUI和REST-API共同简化了基于微服务的数据管道的整体编排。

### [Spring Cloud Stream](https://cloud.spring.io/spring-cloud-stream)

轻量级事件驱动的微服务框架，可快速构建可连接到外部系统的应用程序。 在Spring Boot应用程序之间使用Apache Kafka或RabbitMQ发送和接收消息的简单声明模型。

### [Spring Cloud Stream App Starters](https://cloud.spring.io/spring-cloud-stream-app-starters)

Spring Cloud Stream App Starters是基于Spring Boot的Spring Integration应用程序，可提供与外部系统的集成。

### [Spring Cloud Task](https://cloud.spring.io/spring-cloud-task)

一种短命的微服务框架，用于快速构建执行有限数据处理的应用程序。 用于向Spring Boot应用程序添加功能和非功能功能的简单声明。

### [Spring Cloud Task App Starters](https://cloud.spring.io/spring-cloud-task-app-starters)

Spring Cloud Task App Starters是Spring Boot应用程序，可能是任何进程，包括不能永久运行的Spring Batch作业，它们在有限的数据处理期后结束/停止。

### [Spring Cloud Zookeeper](https://cloud.spring.io/spring-cloud-zookeeper)

使用Apache Zookeeper进行服务发现和配置管理。

### [Spring Cloud AWS](https://github.com/spring-cloud/spring-cloud-aws)

与托管的Amazon Web Services轻松集成。 它提供了一种使用众所周知的Spring习语和API（如消息传递或缓存API）与AWS提供的服务进行交互的便捷方式。 开发人员可以围绕托管服务构建应用程序，而无需关心基础结构或维护。

### [Spring Cloud Connectors](https://github.com/spring-cloud/spring-cloud-connectors)

使各种平台中的PaaS应用程序可以轻松连接到数据库和消息代理（该项目以前称为“Spring Cloud”）等后端服务。

### [Spring Cloud Starters](https://github.com/spring-cloud/spring-cloud-starters)

Spring Boot风格的入门项目，可以简化Spring Cloud用户的依赖管理。 （作为项目停产并在Angel.SR2之后与其他项目合并。）

### [Spring Cloud CLI](https://github.com/spring-cloud/spring-cloud-cli)

Spring Boot CLI插件，用于在Groovy中快速创建Spring Cloud组件应用程序

### [Spring Cloud Contract](https://cloud.spring.io/spring-cloud-contract)

Spring Cloud Contract是一个总体项目，其中包含帮助用户成功实施消费者驱动合同方法的解决方案。

### [Spring Cloud Gateway](https://cloud.spring.io/spring-cloud-gateway)

Spring Cloud Gateway是一款基于Project Reactor的智能可编程路由器。

### [Spring Cloud OpenFeign](https://cloud.spring.io/spring-cloud-openfeign)

Spring Cloud OpenFeign通过自动配置和Spring环境以及其他Spring编程模型习惯用法提供Spring Boot应用程序的集成。

### [Spring Cloud Pipelines](https://cloud.spring.io/spring-cloud-pipelines)

Spring Cloud Pipelines提供了一个固定意见的部署管道，其中包含确保您的应用程序可以零停机方式部署并轻松回滚出错的步骤。

### [Spring Cloud Function](https://github.com/spring-cloud/spring-cloud-function)

Spring Cloud Function通过函数促进业务逻辑的实现。 它支持无服务器提供商之间的统一编程模型，以及独立运行（本地或PaaS）的能力。

## Release Trains

Spring Cloud是一个由独立项目组成的总体项目，原则上具有不同的发布节奏。 为了管理投资组合，发布了BOM（物料清单），其中包含一组针对单个项目的依赖关系（见下文）。 发布列车有名称而不是版本，以避免与子项目混淆。 这些名称是一个字母序列（所以你可以按时间顺序排序）伦敦地铁站的名称（“天使”是第一个版本，“布里克斯顿”是第二个版本）。 当各个项目的点数累积到临界质量时，或者其中一个项目中存在一个需要每个人都可用的关键错误时，发布列车将推出名称结尾为“.SRX”的“服务发布”， 其中“X”是一个数字。

| Release Train | Boot Version |
| ------------- | ------------ |
| Greenwich     | 2.1.x        |
| Finchley      | 2.0.x        |
| Edgware       | 1.5.x        |
| Dalston       | 1.5.x        |

| Component                 | Edgware.SR5    | Finchley.SR2  | Finchley.BUILD-SNAPSHOT |
| ------------------------- | -------------- | ------------- | ----------------------- |
| spring-cloud-aws          | 1.2.3.RELEASE  | 2.0.1.RELEASE | 2.0.1.BUILD-SNAPSHOT    |
| spring-cloud-bus          | 1.3.3.RELEASE  | 2.0.0.RELEASE | 2.0.1.BUILD-SNAPSHOT    |
| spring-cloud-cli          | 1.4.1.RELEASE  | 2.0.0.RELEASE | 2.0.1.BUILD-SNAPSHOT    |
| spring-cloud-commons      | 1.3.5.RELEASE  | 2.0.2.RELEASE | 2.0.2.BUILD-SNAPSHOT    |
| spring-cloud-contract     | 1.2.6.RELEASE  | 2.0.2.RELEASE | 2.0.2.BUILD-SNAPSHOT    |
| spring-cloud-config       | 1.4.5.RELEASE  | 2.0.2.RELEASE | 2.0.2.BUILD-SNAPSHOT    |
| spring-cloud-netflix      | 1.4.6.RELEASE  | 2.0.2.RELEASE | 2.0.2.BUILD-SNAPSHOT    |
| spring-cloud-security     | 1.2.3.RELEASE  | 2.0.1.RELEASE | 2.0.1.BUILD-SNAPSHOT    |
| spring-cloud-cloudfoundry | 1.1.2.RELEASE  | 2.0.1.RELEASE | 2.0.1.BUILD-SNAPSHOT    |
| spring-cloud-consul       | 1.3.5.RELEASE  | 2.0.1.RELEASE | 2.0.2.BUILD-SNAPSHOT    |
| spring-cloud-sleuth       | 1.3.5.RELEASE  | 2.0.2.RELEASE | 2.0.2.BUILD-SNAPSHOT    |
| spring-cloud-stream       | Ditmars.SR4    | Elmhurst.SR1  | Elmhurst.BUILD-SNAPSHOT |
| spring-cloud-zookeeper    | 1.2.2.RELEASE  | 2.0.0.RELEASE | 2.0.1.BUILD-SNAPSHOT    |
| spring-boot               | 1.5.16.RELEASE | 2.0.6.RELEASE | 2.0.7.BUILD-SNAPSHOT    |
| spring-cloud-task         | 1.2.3.RELEASE  | 2.0.0.RELEASE | 2.0.1.BUILD-SNAPSHOT    |
| spring-cloud-vault        | 1.1.2.RELEASE  | 2.0.2.RELEASE | 2.0.2.BUILD-SNAPSHOT    |
| spring-cloud-gateway      | 1.0.2.RELEASE  | 2.0.2.RELEASE | 2.0.2.BUILD-SNAPSHOT    |
| spring-cloud-openfeign    |                | 2.0.2.RELEASE | 2.0.2.BUILD-SNAPSHOT    |
| spring-cloud-function     | 1.0.1.RELEASE  | 1.0.0.RELEASE | 1.0.1.BUILD-SNAPSHOT    |

Finchley构建并使用Spring Boot 2.0.x，预计不会与Spring Boot 1.5.x一起使用。

注意：

- Dalston发布列车将于2018年12月达到使用寿命.Edgware将遵循Spring Boot 1.5.x的生命周期结束周期。

-  卡姆登发布列车标志着寿命终结。

-   Camden发布系列基于Spring Boot 1.4.x构建，但也经过1.5.x测试。
- Brixton和Angel发布列车于2017年7月标志着寿命终止（EOL）。Brixton版本系列基于Spring Boot 1.3.x构建，但也经过了1.4.x的测试。

​    Angel版本系列基于Spring Boot 1.2.x构建，在某些方面与Spring Boot 1.3.x不兼容。 Brixton构建于Spring Boot 1.3.x之上，与1.2.x同样不兼容。 一些基于Angel构建的库和大多数应用程序都可以在Brixton上正常运行，但是在使用spring-cloud-security 1.0.x的OAuth2功能的任何地方都需要进行更改（它们大部分都转移到1.3.0中的Spring Boot）。

使用依赖关系管理工具来控制版本。 如果您正在使用Maven，请记住声明的第一个版本获胜，因此按顺序声明BOM，第一个通常是最新版本（例如，如果您想使用带有Brixton.RELEASE的Spring Boot 1.3.6，请放置引导BOM 第一）。 如果您使用Spring依赖关系管理插件，则同样的规则适用于Gradle。

注意 :
版本系列包含spring-cloud-dependencies以及spring-cloud-starter-parent。 您可以像使用spring-boot-starter-parent一样使用父级（如果您使用的是Maven）。 如果您只需要依赖关系管理，那么“依赖关系”版本是同一事物的仅限BOM的版本（它只包含依赖关系管理，没有插件声明或直接引用Spring或Spring Boot）。 如果您使用的是Spring Boot父POM，则可以使用Spring Cloud中的BOM。 相反的情况并非如此：使用Cloud父级使得使用Boot BOM更改Spring Boot及其依赖项的版本变得不可能或至少不可靠。

## Talks and Videos

- [Beginner’s Guide To Spring Cloud](https://www.youtube.com/watch?v=aO3W-lYnw-o)


## Quick start

使用 [Spring Initializr](https://start.spring.io/) 引导你的应用程序

## Getting Started

### Centralized Configuration(集中配置)

本指南将引导您完成 [Spring Cloud Config Server](https://cloud.spring.io/spring-cloud-config/spring-cloud-config.html)的启动和消费配置过程



### 你要建造什么

您将设置一个Config Server，然后构建一个在启动时使用该配置的客户端，然后刷新配置而不重新启动客户端。

### 你需要什么

- 大约15分钟
- 最喜欢的文本编辑器或IDE
- [JDK 1.8](http://www.oracle.com/technetwork/java/javase/downloads/index.html) or later
- [Gradle 4+](http://www.gradle.org/downloads) or [Maven 3.2+](https://maven.apache.org/download.cgi)
- 您还可以将代码直接导入IDE:
  - [Spring Tool Suite (STS)](https://spring.io/guides/gs/sts)
  - [IntelliJ IDEA](https://spring.io/guides/gs/intellij-idea/)

### 如何完成本指南

与大多数Spring入门指南一样，您可以从头开始并完成每个步骤，或者您可以绕过您已熟悉的基本设置步骤。 无论哪种方式，您最终都会使用工作代码。

从头开始, 请继续使用 [Build with Gradle](https://spring.io/guides/gs/centralized-configuration/#scratch).

要跳过基础知识，请执行以下操作：

- [Download](https://github.com/spring-guides/gs-centralized-configuration/archive/master.zip) 并解压缩本指南的源存储库，或使用它进行克隆 [Git](https://spring.io/understanding/Git): `git clone https://github.com/spring-guides/gs-centralized-configuration.git`
- cd到gs-centralized-configuration / initial
- 跳转到 [ Config Server](https://spring.io/guides/gs/centralized-configuration/#initial).

完成后，您可以根据gs-centralized-configuration / complete中的代码检查结果。

## Build with Gradle



## Build with Maven



## Build with your IDE

### 启动Config Server

首先，您需要一个Config Service作为Spring应用程序和典型版本控制的配置文件存储库之间的一种中介。 您可以使用Spring Cloud的@EnableConfigServer来支持其他应用程序可以与之通信的配置服务器。 这是一个常规的Spring Boot应用程序，添加了一个注释以启用配置服务器。

```
configuration-service/src/main/java/hello/ConfigServiceApplication.java
```

```java
package hello;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.cloud.config.server.EnableConfigServer;

@EnableConfigServer
@SpringBootApplication
public class ConfigServiceApplication {

    public static void main(String[] args) {
        SpringApplication.run(ConfigServiceApplication.class, args);
    }
}
```

Config Server需要知道要管理的存储库。 这里有几种选择，但我们将使用基于Git的文件系统存储库。 您也可以轻松地将Config Server指向Github或GitLab存储库。 在文件系统上，创建一个新目录git init。 然后将名为a-bootiful-client.properties的文件添加到Git存储库。 确保也git commit它。 稍后，您将使用Spring Boot应用程序连接到Config Server，该应用程序的spring.application.name属性将其标识为Config Server的a-bootiful-client。 这就是Config Server将如何知道要发送给特定客户端的配置集。 它还将从Git存储库中名为application.properties或application.yml的任何文件发送所有值。 更具体命名文件中的属性键（如a-bootiful-client.properties）会覆盖application.properties或application.yml中的属性键。

添加一个简单的属性和值, message = Hello world, 到新创建的 a-bootiful-client.properties到新创建的文件，然后 git commit变更.

通过在configuration-service / src / main / resources / application.properties中指定spring.cloud.config.server.git.uri属性来指定Git存储库的路径。 确保在同一台计算机上同时运行此服务器和另一个Spring Boot应用程序时，还要指定不同的server.port值以避免端口冲突。

`configuration-service/src/main/resources/application.properties`

```properties
server.port=8888

spring.cloud.config.server.git.uri=${HOME}/Desktop/config
```

在此示例中，我们在$ {HOME} / Desktop / config中使用基于文件的git存储库。 您可以通过创建一个新目录并将git提交属性和YAML文件轻松创建一个。 例如 E.g

```
$ cd ~/Desktop/config
$ find .
./.git
...
./application.yml
```

或者您可以使用远程git存储库，例如 在github上，如果您将应用程序中的配置文件更改为指向该文件。

### 使用Config Client从Config Server读取配置

现在我们已经启动了一个Config Server，让我们启动一个新的Spring Boot应用程序，该应用程序使用Config Server加载自己的配置并刷新其配置以反映Config Server的需求变化，而无需重新启动JVM。 添加org.springframework.cloud:spring-cloud-starter-config依赖项以连接到Config Server。 Spring将看到配置属性文件，就像从application.properties或application.yml或任何其他PropertySource加载的任何属性文件一样。

在引导阶段，必须先读入配置Config Client的属性，然后才能从Config Server读取其余的应用程序配置。 将客户端的spring.application.name指定为a-bootiful-client，并在configuration-client / src / main / resources / bootstrap.properties中指定配置服务器spring.cloud.config.uri的位置，它将在此时加载 任何其他配置。

configuration-client/src/main/resources/bootstrap.properties

```properties
spring.application.name=a-bootiful-client
# N.B. this is the default:
spring.cloud.config.uri=http://localhost:8888
```

我们还希望启用/ refresh端点，以便我们可以演示动态配置更改：

configuration-client/src/main/resources/application.properties

```properties
management.endpoints.web.exposure.include=*
```

客户端可以使用传统机制（例如@ConfigurationProperties，@ Value（“$ {...}”）或通过环境抽象来访问Config Server中的任何值。 创建一个Spring MVC REST控制器，它返回已解析的消息属性的值。 请参阅 [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)指南，以了解有关使用Spring MVC和Spring Boot构建REST服务的更多信息。

默认情况下，配置值在客户端的启动时读取，而不是再次读取。 您可以通过使用Spring Cloud Config @RefreshScope注释MessageRestController然后触发刷新事件来强制bean刷新其配置 - 从Config Server中提取更新的值。

configuration-client/src/main/java/hello/ConfigClientApplication.java

```java
package hello;

import org.springframework.beans.factory.annotation.Value;
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.cloud.context.config.annotation.RefreshScope;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

@SpringBootApplication
public class ConfigClientApplication {

    public static void main(String[] args) {
        SpringApplication.run(ConfigClientApplication.class, args);
    }
}

@RefreshScope
@RestController
class MessageRestController {

    @Value("${message:Hello default}")
    private String message;

    @RequestMapping("/message")
    String getMessage() {
        return this.message;
    }
}
```

### 测试应用程序

首先启动配置服务，然后在加载后启动客户端，测试端到端结果。 访问浏览器中的客户端应用程序<http://localhost:8080/message>。 在那里，您应该看到响应中反映的字符串 Hello world。

将Git存储库中a-bootiful-client.properties文件中的消息密钥更改为不同的东西（Hello Spring！，也许？）。 您可以通过访问确认Config Server看到更改<http://localhost:8888/a-bootiful-client/default> 您需要调用刷新Spring Boot Actuator端点，以强制客户端刷新自身并绘制新值.Spring Boot的Actuator公开有关应用程序的操作端点，如运行状况检查和环境信息。 为了使用它，您必须将org.springframework.boot：spring-boot-starter-actuator添加到客户端应用程序的CLASSPATH中。 您可以通过向客户端的刷新端点发送空HTTP POST来调用刷新Actuator端点，<http://localhost:8080/actuator/refresh> 然后通过查看 http:// localhost:8080/message 端点确认它是否有效。

```
$ curl localhost:8080/actuator/refresh -d {} -H "Content-Type: application/json"
```

> 我们在客户端应用程序中设置management.endpoints.web.exposure.include = *以使其易于测试（默认情况下，因为Spring Boot 2.0默认情况下不会公开Actuator端点）。 默认情况下，如果未设置标志，仍可以通过JMX访问它们。

### 摘要

恭喜！ 您刚刚使用Spring集中配置所有服务，首先启动然后动态更新配置。

### 也可以看看

以下指南也可能有所帮助：

- [Building an Application with Spring Boot](https://spring.io/guides/gs/spring-boot/)
- [Creating a Multi Module Project](https://spring.io/guides/gs/multi-module/)

想要撰写新指南或为现有指南做出贡献？ 查看我们的[contribution guidelines](https://github.com/spring-guides/getting-started-guides/wiki).

> 所有指南均附有代码的ASLv2许可证，以及 [Attribution, NoDerivatives creative commons license](https://creativecommons.org/licenses/by-nd/3.0/) 创作公共许可证。