# DOM\( Document Object Model\)

> 문서 객체 모델 \(Dom\)

브라우저랜더링 엔진이 HTML를 파싱하여 브라우저가 이해할 수 있는 구조로 메모리에 올리는데 이것을 DOM이라고 한다. 모든 요소를 객체로 만들고 부모자식 관계를 표현할 수 있는 트리구조로 구성한다. 

DOM트리는 노드로 구성된다. 루트를 제외하고 모든노드에 부모가 있으며 자식노드 있어도 되고 없어도 된다. 루트노드는 document이며 자식노드는 html요소이다. 이하 자식노드로 head, body가 있으며 body노드 아래로 여러 자식노드가 존재한다.

DOM트리의 모든 노드는 Node 클래스의 인스턴스이다. 부모와 자식노드 자신을 나타내는 프로퍼티인 parentNode, childNodes, nodeName, nodeType이 있다.

DOM은 자신을 변경가능할 수 있게 API를 제공한다. 이를 DOM API라고 한다. document.getElementById\(\) 이런 메서드들이 DOM API 이다. 요소에 접근하고 객체를 가져오고 변경이 가능하다.



> DOM tree 종류

* 문서노드 \(Document Node\)

트리의 최상위에 존재하며 각 요소, 어트리뷰트, 텍스트 노드에 접근하려면 문서노드로 접근한다.

* 요소노드 \(Element Node\)

HTML 요소를 표현한다. 부자관계를 가지며 문서의 구조를 표현한다. HTMLElement 객체를 상속한 객체이다.

* 어트리뷰트 노드 \(Attribute Node\)

HTML 요소의 어트리뷰트를 표현한다. 특정요소의 접근하여 어트리뷰트를 참조할 수 있다.

* 텍스트 노드 \(Text Node\)

HTML 요소의 텍스트를 표현하며 요소노드의 자식이다. 자식노드를 가질수 없고 DOM tree의 최종단이다.

react, vue 등 라이브러리를 사용한다면 직접 쓰일일은 많지 않지만 라이브러리 없이 순수자바스크립트로 조작하는 법은 알고있어야 한다고 생각한다.
