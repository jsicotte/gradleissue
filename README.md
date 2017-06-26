# gradleissue
Repo to illustrate how Gradle 4.0 breaks a specific type of spring boot builds

## Reproducing the Issue ##
Execute the gradle build: ./gradlew --stacktrace build. The build will print the following stack trace:

> Caused by: java.lang.NoSuchMethodError: org.gradle.api.artifacts.ProjectDependency.getConfiguration()Ljava/lang/String;
>        at org.springframework.boot.gradle.repackage.ProjectLibraries.getLibrariesForFileDependencies(ProjectLibraries.java:132)
