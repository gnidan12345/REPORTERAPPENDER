# REPORTERAPPENDER

<dependency>
 <groupId>org.testng</groupId>
 <artifactId>reportng</artifactId>
 <version>1.2.2</version>
 <scope>test</scope>
</dependency>


appenders = tesng
rootLogger.level = DEBUG
rootLogger.appenderRefs = r_testng
rootLogger.appenderRef.r_testng.ref = ReporterAppender

appender.tesng.type = Reporter
appender.tesng.name = ReporterAppender
appender.tesng.layout.type = PatternLayout
appender.tesng.layout.pattern = [%-5level] %d{yyyy-MM-dd HH:mm:ss.SSS} [%t] %c{1} - %msg%n
