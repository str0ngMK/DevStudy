## Annotation
##### Annotation(어노테이션)은 프로그램에 메타데이터를 추가하는 방법 중 하나로, 소스 코드에 특별한 주석 형식으로 정보를 초함시키는 것입니다. 이러한 주석을 사용하여 컴파일러, 런타임 환경 또는 다른 개발 도구에게 특정 작업을 수행하거나 특정 정보를 제공할 수 있습니다. Java 언어에서 Annotation은 JDK 5부터 도입되었으며, 주로 코드 문서화, 컴파일 타임 검사 및 런타임 동작을 지정하는 데 사용됩니다.
<br>

> @AnnotationName
- Annotation은 `@`기호를 사용하여 정의하며, 어노테이션 이름이 됩니다.
- 예를 들어, `@Override` 또는 `@Deprecated`와 같은 내장 어노테이션들이 있습니다.
<br>

> 컴파일 타임 검사
- 어노테이션을 사용하면 컴파일러가 코드를 분석하고 오류를 감지할 수 있습니다.
- 예를 들어, `@Override` 어노테이션은 메서드가 부모 클래스의 메서드를 재정의하는 것을 나타내며, 부모 클래스에 해당 메서드가 없는 경우 컴파일 오류를 발생시킵니다.
<br>

> 런타임 정보
- 어노테이션은 런타임 환경에서 리플렉션(reflection)을 사용하여 읽을 수 있습니다.
- 이를 통해 클래스나 메서드의 정보를 동적으로 가져올 수 있습니다.
<br>

> 사용자 정의 어노테이션
- Java에서는 사용자가 직접 어노테이션을 정의할 수 있습니다.
- `@interface`키워드를 사용하여 사용자 정의 어노테이션을 만들고 필요한 속성과 값을 추가할 수 있습니다.
<pre>
import java.lang.annotation.*;
  
@Retention(RetentionPolicy.RUNTIME)
@Target(ElementType.METHOD)
public @interface MyAnnotation {
    String value() default "";
    int count() default 0;
}
</pre>
