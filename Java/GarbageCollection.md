## Garbage Collection

<br>

- **Garbage Collection**란, C/C++ 프로그래밍을 할 때 메모리 누수를 막기 위해 객체를 생성한 후 사용하지 않는 객체의 메모리를 프로그래머가 직접 해제해 주어야 했다.
- JAVA에서는 JVM(Java Virtual Machine)이 구성된 JRE(Java Runtime Environment)가 제공되며 그 구성요소 중 하나인 GC가 자동으로 사용하지 않는 객체를 파괴한다.

  <br>

### GC의 대상

1. 객체가 null일 경우 (ex. String str = null)
2. 블럭 실행 종료 후, 블럭 안에서 생성된 객체
3. 부모 객체가 null일 경우, 포함하는 자식 객체
