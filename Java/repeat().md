## Repeat
##### Java 11에서 도입된 String.repeat(int count) 메서드는 문자열을 지정된 횟수만큼 반복하여 새로운 문자열을 생성하는 기능을 제공합니다.
<br>

> 설명
- `repeat()` 메서드는 기존 문자열을 주어진 횟수만큼 반복하여 새로운 문자열을 반환합니다.
- 예를 들어, `"Hello ".repeat(3)`은 "Hello Hello Hello"와 같은 결과를 반환합니다.
- 이때, 주의할 점은 음수 값을 전달하면 `IllegalArgumentException`이 발생하며, 0을 전달하면 빈 문자열을 반환합니다.
- 이러한 예외 처리를 통해 메서드의 안정성을 보장합니다.

> 사용 이유
- 이전에는 반복을 위해 루프나 다른 방법을 사용해야 했던 번거로움을 덜어준다.

### Example
```java
String original = "Hello ";
String repeated = original.repeat(3);
System.out.println(repeated);
```
위의 코드는 "Hello " 문자열을 3번 반복하여 "Hello Hello Hello "문자열을 출력합니다.

```java
String empty = original.repeat(0); // 빈 문자열 반환
```
`repeat()` 메소드는 음수 값을 전달하면 `IllegalArgumentException`을 발생시킵니다. 또한 0을 전달하면 빈 문자열을 반환합니다.
