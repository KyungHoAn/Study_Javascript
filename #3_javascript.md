# 02.Model2MVCShop(addProductView)
### calendar설정의 javascript
```
<script type="text/javascript" src="../javascript/calendar.js">
</script>
```
- calender를 누르면 calender를 보여주는 js로 연결시켜주는 역할 수행

### name=detailForm값에서의 javascript
```
function fncAddProduct(){
	//Form 유효성 검증
 	var name = document.detailForm.prodName.value;
	var detail = document.detailForm.prodDetail.value;
	var manuDate = document.detailForm.manuDate.value;
	var price = document.detailForm.price.value;

	if(name == null || name.length<1){
		alert("상품명은 반드시 입력하여야 합니다.");
		return;
	}
	if(detail == null || detail.length<1){
		alert("상품상세정보는 반드시 입력하여야 합니다.");
		return;
	}
	if(manuDate == null || manuDate.length<1){
		alert("제조일자는 반드시 입력하셔야 합니다.");
		return;
	}
	if(price == null || price.length<1){
		alert("가격은 반드시 입력하셔야 합니다.");
		return;
	}

	document.detailForm.action='/addProduct.do';
	document.detailForm.submit();
}

function resetData(){
	document.detailForm.reset();
}
```
### 함수(function)
- 하나의 특별한 목적의 작업을 수행하도록 설계된 독립적인 블록
```
function fncAddProduct(){
}
```
- fncAddProduct() 라는 특별한 목적의 작업을 수행하도록하는 함수 작성

### 변수 선언 및 초기화
- document 는 DOM 트리의 최상위 객체이다
- document의 뜻 : 현재 문서
- DOM (Document Object Model) 트리란?
<img src="https://miro.medium.com/max/1088/1*NA2VKR09ECb8PEgYDteR3w.gif">

  - xml 및 html 문서를 응용프로그램에서 사용하기 위한 API규격
  - DOM이란 문서의 각 부분들을 객체로 표현한 API
  - 넓은 의미로 웹 브라우저가 HTML페이지를 인식하는 방식을 의미하며 좁은 의미로는 document객체와 관련된 객체의 집합
  - 웹 페이지의 모든 요소를 Document객체가 관리

```
 	var name = document.detailForm.prodName.value;
	var detail = document.detailForm.prodDetail.value;
	var manuDate = document.detailForm.manuDate.value;
	var price = document.detailForm.price.value;
```
- var name은 document객체의 detailForm(form으로 설정된 name값)의 prodName이란 name으로 설정된 value값을 가져와 var name으로 초기화
- detail / menuData / price도 같은 의미

### javascript form.폼_이름.action 컨트롤
```
	document.detailForm.action='/addProduct.do';
	document.detailForm.submit();
```
- 할당된 값을 action 컨트롤을 통하여 properties에 선언되어 있는 name값인 addProdut.do에서 value값으로 이동한다.
- submit : 제출하다

### reset() input초기화
```
function resetData(){
	document.detailForm.reset();
}
```
- document.detailForm.reset() : 현재문서의 detailForm(form이름)의 값들을 초기화시킨다.
- resetData함수를 설정해 놓고 해당 함수를 사용한다면 해당 문서의 form이름이 있는 구역의 값들을 초기화 시키는 역할을 수행한다.
