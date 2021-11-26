# Gradle, Kotlin, Spring Skeleton ![main](https://github.com/mrclrchtr/gradle-kotlin-spring/workflows/CI/badge.svg)

Do you already know how to set up a Gradle multi-project / multi-module with Kotlin DSL and Spring Dependency
Management?

I have set up an example here, in which I have abstracted the most important logical components and packed them into
individual buildSrc modules. This makes the build very modular and also very clear. What do you think?

It has the following details:

- Gradle 7.2
  - buildSrc
  - Kotlin DSL
  - Version Catalog (libs.versions.toml)
- Kotlin 1.5.30
- Spring 2.5.4
- Spring Dependency-Management

Additionally, I added a POC how Maven Publishing could work. In another project, I got it to work like this without
Spring boot on Gitlab. Unfortunately it doesn't work with the spring boot plugin in this example yet. But I think it can
help others to reach their goals.

If there are any questions or suggestions for improvement, issues, discussions and PRs are welcome.

## Run it!

The factory:

    gradle :message-factory:bootRun

The Dashboard:

    gradle :message-dashboard:bootRun

And now visit <http://localhost:8080/dashboard/Mr.Bean>

You can enter every name in place of "Mr.Bean". 
