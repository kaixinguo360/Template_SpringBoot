# My Example
Template for building springboot applications

### Out of the box
* SpringBoot
* Kotlin
* MyBatis
* MyBatis Generator
* Some useful config files

### Example Content
You should remove or change them:

Documents
* [README.md](README.md)
* [HELP.md](HELP.md)

Paths
* [src/main/java/com/my/example](src/main/java/com/my/example)
* [src/test/java/com/my/example](src/test/java/com/my/example)

Gradle config file
* [settings.gradle](settings.gradle)
```
rootProject.name = 'MyExample'
```

SpringBoot config file
* [application.yml](src/main/resources/config/application.yml)
```
spring:
  application:
    name: MyExample
```

Example model
* [User.kt](src/main/java/com/my/example/bean/User.kt)
* [UserMapper.xml](src/main/resources/mapper/UserMapper.xml)
* [UserMapper.java](src/main/java/com/my/example/mapper/UserMapper.java)
* [UserMapperTest.java](src/test/java/com/my/example/mapper/UserMapperTest.java)
* [UserService.java](src/main/java/com/my/example/service/UserService.java)

Mybatis config file
* [mybatis.xml](src/main/resources/config/mybatis.xml)
```
<typeAliases>
    <typeAlias alias="User" type="com.my.example.bean.User" />
</typeAliases>
```

Mybatis generator config file
* [mybatis-generator.xml](src/main/resources/config/mybatis-generator.xml)
```
<table tableName="users" domainObjectName="User">
    <generatedKey column="user_id" sqlStatement="JDBC"/>
    <columnRenamingRule searchString="^user_" replaceString=""/>
</table>
```

