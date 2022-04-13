# jQuery
- 제이쿼리는 자바스크립트 언어를 간편하게 사용할 수 있도록 단순화시킨 오픈소스 기반의 자바스크립트 라이브러리이다.
- 제이쿼리를 이용하면 문서 객체 모델(DOM)과 이벤트에 관한 처리를 손쉽게 구현할 수 있다.
- Ajax 응용 프로그램 및 플러그인도 제이쿼리를 활용하여 빠르게 개발할 수 있습니다.


### 문법
- 제이쿼리를 사용하면 아주 간편하게 HTML 요소를 선택하고, 그렇게 선택된 요소에 손쉽게 특정 동작을 설정할 수 있다.

```
$(선택자).동작함수();
```
- $ 기호는 제이쿼리를 의미하고, 제이쿼리에 접근할 수 있게 해주는 식별자

$() 함수<br/>
-$() 함수의 인수로는 HTML 태그 이름뿐만 아니라, CSS 선택자를 전달하여 특정 HTML 요소를 선택할 수 있습니다.

이러한 $() 함수를 통해 생성된 요소를 제이쿼리 객체(jQuery object)라고 합니다.

제이쿼리는 이렇게 생성된 제이쿼리 객체의 메소드를 사용하여 여러 동작을 설정할 수 있습니다.

```
function func() {

    addAttribute();  // 아이디가 "para"인 HTML 요소에 속성을 추가함.

    createElement(); // 아이디가 "para"인 HTML 요소를 생성함.

}

function createElement() {

    var criteriaNode = document.getElementById("text");

    var newNode = document.createElement("p") newNode.innerHTML = "새로운 단락입니다.";

    newNode.setAttribute("id", "para");

    document.body.insertBefore(newNode, criteriaNode);

}

function addAttribute() {

    document.getElementById("para").setAttribute("style", "color: red");

}
```
<a href="http://www.tcpschool.com/jquery/jq_basic_js">참고: TCPSCHOOL.com</a>

### CSS선택자를 이용한 선택
- 제이쿼리에서는 CSS선택자를 사용하여 HTML요소를 선택할 수 있다.
```
$(function() {

    $("p").on("click", function() {        // <p>요소를 모두 선택함.

        $("span").css("fontSize", "28px"); // <span>요소를 모두 선택함.

    });

});
```

