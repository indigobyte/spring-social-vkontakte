### Spring Social VKontakte
[![Build Status](http://fugru.com/jenkins/buildStatus/icon?job=spring-social-vkontakte)](http://fugru.com/jenkins/job/spring-social-vkontakte/)

To check out the project and build from source, do the following:

```
git clone git://github.com/vkolodrevskiy/spring-social-vkontakte.git
cd spring-social-vkontakte
./gradlew build
```

To generate Eclipse metadata (.classpath and .project files), do the following:

```
./gradlew eclipse
```

Once complete, you may then import the projects into Eclipse as usual:
 `File -> Import -> Existing projects into workspace`

To generate IDEA metadata (.iml and .ipr files), do the following:

```
./gradlew idea
```

To build the JavaDoc, do the following from within the root directory:

```
./gradlew :docs:api
```

The result will be available in `'docs/build/api'`.

For more details go to project wiki https://github.com/vkolodrevskiy/spring-social-vkontakte/wiki

To create maven artifact:

Create new empty directory `maven-temp` in the project root.

Checkout spring-social-vkontakte into maven-temp.

Switch to branch mvn-repo. You should have directory structure like this:

```
c:\projects\spring-social-vkontakte\maven-temp\spring-social-vkontakte\org\springframework\social\spring-social-vkontakte\2.0.0.CUSTOM\maven-metadata.xml
```

Go to root project dir (`c:\projects\spring-social-vkontakte`).

run command

```
./gradlew clean build publish
```

Go back to `maven-temp\spring-social-vkontakte` folder:

```
c:\projects\spring-social-vkontakte\maven-temp\spring-social-vkontakte\org\springframework\social\spring-social-vkontakte\
```

Commit and push mvn-repo branch.