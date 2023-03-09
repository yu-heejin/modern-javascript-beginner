console.log의 출력 결과는 자바스크립트 실행 환경에 따라 달라질 수 있다.

```jsx
var obj = {};
obj[ Symbol("heart") ] = 3;
console.log(obj);

Object { }    // 파이어폭스 콘솔
Object {Symbol (heart) : 3}     // 크롬 콘솔
Object      // html 문서에 삽입하여 크롬에서 여는 경우
```

- 위 코드의 결과는 브라우저마다 보이는 모습이 다르다.
- 크롬 콘솔은 상세한 정보를 표시하지만, 다른 실행 환경은 정보를 간략히 표시한다.