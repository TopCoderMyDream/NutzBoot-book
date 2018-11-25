# 配置Maven

###  配置Maven国内镜像

- 打开maven下的conf\settings.xml,在

```xml
		<dependency>
			<groupId>org.nutz</groupId>
			<artifactId>nutz</artifactId>
			<version>1.r.60</version>
		</dependency>
		<dependency>
			<groupId>com.alibaba</groupId>
			<artifactId>druid</artifactId>
			<version>1.0.26</version>
			<exclusions>
				<exclusion>
					<artifactId>jconsole</artifactId>
					<groupId>com.alibaba</groupId>
				</exclusion>
				<exclusion>
					<artifactId>tools</artifactId>
					<groupId>com.alibaba</groupId>
				</exclusion>
			</exclusions>
		</dependency>
		<dependency>
			<groupId>mysql</groupId>
			<artifactId>mysql-connector-java</artifactId>
			<version>5.1.40</version>
		</dependency>
```

### 关于Log4j

```
log4j.rootLogger=debug,Console

log4j.appender.Console=org.apache.log4j.ConsoleAppender
log4j.appender.Console.layout=org.apache.log4j.PatternLayout
log4j.appender.Console.layout.ConversionPattern=[%-5p] %d{HH:mm:ss.SSS} %l - %m%n
```

