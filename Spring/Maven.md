### Maven과 Gradle의 차이

스프링 부트 프로젝트를 하려고 하는데 gradle를 설치하라고 한다.

전에 스프링에서는 Maven을 했었던 기억이 나는데 둘은 각각 무엇이고 어떠한 차이가 있을까?

---

우선, 이 둘은 **빌드 관리 도구**이다.

프로젝트 내에서 작성한 자바코드와 프로젝트 내 필요한 각종 xml, properties, jar파일 등등을 JVM이나 WAS가 인식할수 있도록 패키징 해주는 역할을 한다. 애플리케이션을 개발하면서 여러가지 외부 라이브러리들을 가져다 사용할텐데 사용자가 직접 관리할 필요 없이 필요한 라이브러리들을 자동으로 관리해준다. 프로젝트 생성, 테스트 빌드, 배포등의 작업을 수행한다.

---

## **Maven**



Maven은 프로젝트관리 도구이다. Project object model (POM)개념의 기반으로 만들어져있으며 빌드 중인 프로젝트, 빌드 순서, 다양한 외부 라이브러리의 종속성 관계들을 pom.xml파일에 명시한다. 외부저장소에서 필요한 라이브러리와 플러그인들을 다운로드 한 다음, 로컬시스템의 캐시에 모두 저장한다.

## **Gradle**


Gradle은 Grooby를 이용한 빌드 자동화 시스템이다. Ant와 Maven의 장점을 모아 출시 됐으며 Maven의 후속주자인 만큼 Maven보다 장점이 더 많다. Ant처럼 유연한 범용 빌드 도구, Maven을 사용할 수 있는 변환 가능 컨벤션 프레임 워크등등의 장점이 있다.

---

## **Maven VS Gradle**

볼 것도 없이 Gradle의 압승이다. Gradle공식 홈페이지에서 Maven과의 성능을 비교하고 있거든.

-   Build라는 동적인 요소를 XML의 정의하기에 따른 어려움
-   Groovy를 사용함으로써, 동적인 빌드 호출에 용이함. 즉 빌드시간이 훨씬 단축
-   concurrent에 안전한 캐시 사용

정보를 더욱 얻고싶다면 [gradle.org/maven-vs-gradle/](https://gradle.org/maven-vs-gradle/)

[

Gradle | Gradle vs Maven Comparison

High-level performance and feature comparison between Gradle and Maven

gradle.org



](https://gradle.org/maven-vs-gradle/)

---

## **결론**

Maven보다 Gradle훨씬 더 좋음. 간단하고 빠른데 안 쓸이유가 하나도 없다고 생각함.

더군다나 나는 Maven이 익숙한것도 아니니.
