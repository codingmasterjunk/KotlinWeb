[2024.08.18 KotlinWebApplication]
1. OS : Window
2. Framework : SpingFramework.boot => 3.2.1
3. plugin.spring => 1.9.21
4. Dependency : Spring-Dependency.management => 1.1.4
5. JVM : 1.9.21
6. Build : build.gradle.kts

[# settings.gradle.kts]
모든 gradle 프로젝트의 진입점이 되는 파일로, 주목적은 root project와 함께 빌드할 subproject를 추가하는 것임.
그래서 root project만 존재하는 single project의 경우에는 선택사항이며, multi-project에서는 필수적으로 포함되어야하는 파일임.
root project를 명시하고, 사용될 subproject를 include 시켜줌.


[# build.gradle.kts]
하나 이상의 파일이 필요하며, 일반적으로 build 환경구성이나 task, plugin을 기술하며, 의존성 선언을 하는 파일임.
gradle 혹은 build script에서 필요한 라이브러리나 플러그인, 소스 코드 상에서 필요한 라이브러리 의존성을 포함함.
Gradle의 기능을 확장시킬 수 있는 plugin을 추가함.
plugin를 선언하면 task 뿐 아니라 property, method도 추가할 수 있음.


## Gradle 공식사이트에 예시 참조
https://docs.gradle.org/current/userguide/kotlin_dsl.html