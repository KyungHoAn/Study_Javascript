# PJ 내용
- .js file 안에서는 <script>를 사용할 필요가 없다.

### alert() 함수
```
if(formField.getAttribute("required") != null && fieldValue == ""){
  alert(fieldTitle+" is a required field.");
  return PortalReturnFalse(formField);
}
```
```
alert('hi');  
```
- alert()은 이미지막스를 보여주는 창
<img src="https://www.everdevel.com/material/images/JavaScript/alert.png">

<hr/>
### RegExp (정규식 Regular Expressions)
- 정규식은 무낮열에 포함된 문자 조합을 위해 사요오디는 패턴
- 특정 패턴에 매칭되는 문자열을 쉽게 찾는 방식

### concat() 문자열 붙이기
```
  var s1 = "문자열1";
  var s2 = "문자열2";
  
  s3 = s1.concat(s2);
  document.writeln(s3+'<br>');  //문자열 1 문자열 2 출력
```

### 배열 필터 사용
- 그룹을 필터하거나 그룹에서 원소를 삭제하려고 할때 사용
```
const numbers = [1, 2, 3, 4, 5];
const modifiedArr = numbers.filter((el) => el !== 2);
console.log(modifiedArr); // [1, 3, 4, 5]
```
### 배열 forEach()
- 그룹을 순환하는데 사용
  ```
  const arr = [1, 2, 3, 4, 5];

arr.forEach((el, index, array) => console.log('element', el, 'index', index, 'arr', array);

// output
// element 1 index 0 arr (5) [1, 2, 3, 4, 5]
// element 5 index 4 arr (5) [1, 2, 3, 4, 5]
  ```
  ### 베열찾기 
  ```
  const arr = [2, 3, 5, 6, 8];

const val = arr.find((el) => el % 2 === 0)

console.log('val', val); // val 2
  ```
  
  ### 배열 reduce()
  현재 원소와 이전 원소를 사용하여 계산하는 방법
  ```
  const arr = [2, 2, 2, 2, 2];
const result = arr.reduce((prev, current) => prev * current);

console.log('result', result) // result 32
  ```
  
  
