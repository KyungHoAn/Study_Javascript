# JavaScript

## 자바 스크립트의 역할
- 사용자의 입력 및 계산
  - hltml은 보이는 창만 존재할 뿐 계산 처리 불가, 키나 마우스의 입력과 계산은 오직 자바스크립트로 처리
- 웹 서버와의 통신
  - 웹 페이지가 웹 서버와 데이터를 주고받을 때 활용

## 자바 스크립트 코드의 위치
- <script></script>내에 작성
- 자바스크립트 파일에 작성
- URL부분에 작성
- <script></script>

## 화면단 출력 document.write() / document.writeln()
- 자바스크립트 코드로 브라우저에 출력되게 할 수 있는 코드
```
<script>
document.write("wellcome");
</script>
```

## 변수
- 자바스크립트는 변수에 데이터 타입을 정하지 않는다
* 변수 선언
```
var score;  //변수 score선언
var year, month, day //year,month, day의 3개의 변수 선언
var address ="서울시"; //서울시로 address초기화
```
```
let i; // i선언
let sum =0; // 선언과 동시에 초기화
let i, sum;
```

* let vs var
- let은 변수가 선언된 블록, 구문, 또는 표현힉 내에서만 사용할 수 있는 변수
- var는 전역변수 또는 지역 변수

## 상수 const(block scope)
- 자바와 같이 대문자를 사용하여 선언
```
const NUM = 6;
```

## 객체 생성
```
<script>
  let today = new Date();   //시간정보 저장되어있는 Date타입의 객체 생성
  document.write("현재시간:"+today.toLocaleString()+"<br>");  //Data안의 메소드 호출
  
  let mystr = new String("자바스크립트");
  document.writeln("mystr:"+mystr);
  document.writeln("mystr:"+mystr.length);
</script>
```
<img src="https://github.com/KyungHoAn/Study_Javascript/blob/master/%EC%BA%A1%EC%B3%90/1.png" width="50%" height="50%">
<img src="https://github.com/KyungHoAn/Study_Javascript/blob/master/%EC%BA%A1%EC%B3%90/2.png" width="80%" height="80%">
