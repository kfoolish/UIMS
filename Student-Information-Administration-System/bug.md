#### Logging bug be shown as followed :
```
26-Jul-2019 10:55:23.635 SEVERE [RMI TCP Connection(3)-127.0.0.1] org.apache.catalina.core.StandardContext.startInternal Context [/mavenTemplate_war] startup failed due to previous errors
log4j:WARN No appenders could be found for logger (org.springframework.web.context.support.XmlWebApplicationContext).
log4j:WARN Please initialize the log4j system properly.
log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
26-Jul-2019 10:55:23.717 WARNING [RMI TCP Connection(3)-127.0.0.1] org.apache.catalina.loader.WebappClassLoaderBase.clearReferencesJdbc The web application [mavenTemplate_war] registered the JDBC driver [com.alibaba.druid.proxy.DruidDriver] but failed to unregister it when the web application was stopped. To prevent a memory leak, the JDBC Driver has been forcibly unregistered.
```

#### SQL error be shown ad followed : 
```
org.springframework.jdbc.UncategorizedSQLException: 
### Error querying database.  Cause: java.sql.SQLException: The user specified as a definer ('root'@'%') does not exist
### The error may exist in file [E:\Intellij IDEA\workbench-github\ssm project\Student-Information-Administration-System\target\xiayan1\WEB-INF\classes\com\springmvc\mapper\StudentMapper.xml]
### The error may involve defaultParameterMap
### The error occurred while setting parameters
### SQL: {       call count_stu_percent(?,?,?)     }
### Cause: java.sql.SQLException: The user specified as a definer ('root'@'%') does not exist
; uncategorized SQLException for SQL []; SQL state [HY000]; error code [1449]; The user specified as a definer ('root'@'%') does not exist; nested exception is java.sql.SQLException: The user specified as a definer ('root'@'%') does not exist
```

#### Unknown error be shown as followed : 
```
26-Jul-2019 12:40:59.684 INFO [Abandoned connection cleanup thread] org.apache.catalina.loader.WebappClassLoaderBase.checkStateForResourceLoading Illegal access: this web application instance has been stopped already. Could not load []. The following stack trace is thrown for debugging purposes as well as to attempt to terminate the thread which caused the illegal access.
 java.lang.IllegalStateException: Illegal access: this web application instance has been stopped already. Could not load []. The following stack trace is thrown for debugging purposes as well as to attempt to terminate the thread which caused the illegal access.
	at org.apache.catalina.loader.WebappClassLoaderBase.checkStateForResourceLoading(WebappClassLoaderBase.java:1383)
	at org.apache.catalina.loader.WebappClassLoaderBase.getResource(WebappClassLoaderBase.java:1036)
	at com.mysql.cj.jdbc.AbandonedConnectionCleanupThread.checkContextClassLoaders(AbandonedConnectionCleanupThread.java:96)
	at com.mysql.cj.jdbc.AbandonedConnectionCleanupThread.run(AbandonedConnectionCleanupThread.java:69)
	at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1128)
	at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:628)
	at java.base/java.lang.Thread.run(Thread.java:834)
```

#### Page size error 
```
用户信息修改面板尺寸不正常,是固定值,无法动态变化 ..
暂时方案 : style = "z-index: 19891015; width: 680px; height: 550px; top: 5px; left: 16.5px;"
```