## JAVA

<br>

- **JAVA JVM**란, 자바로 작성된 프로그램을 실행하는 데 사용되는 가상머신이다.
- JVM은 자바 어플리케이션을 바이트코드로 변환하고, 이 바이트코드를 OS에 상관없이 실행할 수 있게 한다.
- 이로써 자바는 플랫폼에 독립적인 특성을 가진다.

<br><br>

**장점**

1. 플랫폼 독립적
   - 자바 어플리케이션은 한 번 작성하면 어떤 플랫폼에서든 실행될 수 있다.
   - 타 언어의 경우에는 맞는 환경에 따라 빌드를 다르게 해야 하지만 자바는 JVM이 여러 OS에서 구현될 수 있기 때문에 jar, war 파일을 OS에 상관없이 JVM 위에서 동작 가능하다.
2. 메모리 관리
   - JVM은 가비지 컬렉션(GC)을 통해 메모리 관리를 수행하기에 개발자가 메모리를 직접 관리할 필요가 없다.
3. 보안
   - JVM은 클래스 로더와 바이트 코드 검증을 통해 안전한 실행 환경을 제공한다.
   - 악성코드로부터 시스템을 보호할 수 있다.

<br>

**단점**

1. 느린 실행 속도
   - JVM을 사용하면 추가적인 오버헤드가 발생하여 네이티브 코드에 비해 상대적으로 느린 실행 속도를 보인다.
2. 더 많은 메모리 소비
   - JVM이 가비지 컬렉션과 같은 메모리 관리 기능을 수행하면서 더 많은 메모리를 사용할 수 있다.
3. 추가적 시간 소요
   - JVM을 시작하고 클래스를 로드하는 과정에서 추가적인 시간이 소요된다.
