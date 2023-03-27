## Spring과 SpringBoot의 차이

<br>

- Spring Framework는 기존에 EJB를 대신에 자바 애플리케이션을 더 쉽게 만들 수 있게 해주고, SpringBoot Framework는 Spring보다 개발자가 더욱 개발에만 집중할 수 있도록 도와주는 프레임워크이다.

<br>

### Spring Framework의 특징

1. DI(Dependency Injection)

- **DI**란, 개발자가 Spring 프레임워크에 의존성을 주입하면서 객체 간 결합을 느슨하게 하는 것이다.
- 객체 간 결합이 느슨하면 코드의 재사용성이 증가하고, 단위 테스트가 용이해진다.

<br>

2. IoC(Invesion of Control)

- **IoC**란, 제어의 역전이란 의미로 컨트롤의 제어권이 개발자에게 있는 것이 아닌 프레임워크가 대신해서 해주는 것이다.
- Servlet이나 Bean 같은 코드를 개발자가 직접 작성하지 않고, 프레임워크가 대신 수행해준다.
- 기존에는 자바 코드를 작성할 때 객체의 생성, 의존관계 설정 등을 개발자가 해줘야 했지만, 프레임워크가 대신 해준다.

<br>

3. AOP(Aspect Oriented Programming)

- **AOP**란, 핵심기능을 제외한 부수적인 기능을 프레임워크가 제공한다는 것이다.
- 예를 들어 Spring 프로젝트에 security를 적용하거나, logging 등을 추가하고 싶을 때 기존 비즈니스 로직을 건들지 않고 AOP로 추가할 수 있다.

<br>

4. 중복 코드 제거

- JDBC 같은 템플릿을 사용할 때 중복되는 코드가 많이 발생하고 복잡하지만 이를 모두 제거해 준다.

<br><br>

### SpringBoot Framework와 Spring Framework의 차이점

1. Dependency

- Spring의 경우, 의존성을 설정해줄 때 설정 파일이 매우 길고, 모든 dependency에 대해 버전 관리도 하나하나 해줘야 한다.

```
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-web</artifactId>
    <version>5.3.5</version>
</dependency>
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-webmvc</artifactId>
    <version>5.3.5</version>
</dependency>
```

- SpringBoot의 경우, dependency를 Spring보다 쉽게 설정해 줄 수 있다. 버전 관리도 자동으로 해준다.
- 빌드 툴을 gradle을 사용하는 경우 build.gradle 파일에 dependency를 추가해주면 SpringBoot로 웹 개발을 할 때 필요한 모든 dependency를 자동으로 추가하고 관리해준다.

```
implementation 'org.springframework.boot:spring-boot-starter-web'
```

<br>

2. Configuration

- Spring의 경우, configuration 설정을 할 때도 매우 길고, 모든 어노테이션 및 빈 등록을 설정해줘야 한다.
- SpringBoot의 경우는 application.properties 파일이나 application.yml 파일에 설정하면 된다.

<br>

3. 편리한 배포

- Spring으로 개발한 애플리케이션의 경우, war 파일을 Web Application Server에 담아 배포해야 한다.
- SpringBoot는 Tomcat이나 Jetty 같은 내장 WAS를 가지고 있기 때문에 jar 파일로 간편하게 배포할 수 있다.
