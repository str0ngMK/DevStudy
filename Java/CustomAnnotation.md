## Custom Annotation
##### 사용자 정의 어노테이션(Custom Annotation)은 Java 프로그래머가 자신만의 어노테이션을 정의할 수 있는 기능입니다. 이러한 어노테이션은 코드에 메타데이터를 추가하고, 컴파일러, 런타임 환경 또는 다른 도구로부터 특별한 동작을 지시하거나 정보를 제공하는 데 사용됩니다. 사용자 정의 어노테이션은 `@interface`키워드를 사용하여 정의됩니다.
<br>

> @interface 키워드
- 어노테이션을 정의하기 위해 `@interface`키워드를 사용합니다.
<br>

> 요소(Element)
- 어노테이션 내부에는 요소(Elements)를 선언할 수 있습니다.
- 요소는 어노테이션의 속성이며, 이름과 반환 유형을 가집니다.
- 요소에 대한 기본값을 지정할 수도 있습니다.
<br>

> 유지 정책(RetentionPolicy)
- 어노테이션의 유지 정책을 지정할 수 있습니다.
- 유지 정책은 어노테이션 정보가 언제까지 유지되는지를 결정합니다.
- 주로 `RetentionPolicy.SOURCE`, `RetentionPolicy.CLASS`, 또는 `RetentionPolicy.RUNTIME`중 하나를 선택합니다.
- `RetentionPolicy.RUNTIME`을 선택하면 런타임에 리플렉션을 통해 어노테이션 정보를 읽을 수 있습니다.
<br>

> 대상(Target)
- 어노테이션을 어디에 적용할 수 있는지를 명시합니다.
- 예를 들어, 클래스, 메서드, 필드 등 다양한 대상에 어노테이션을 적용할 수 있습니다.
