# ESM 문법 익히기
###### 2022-02-07
#react #ESM #es6모듈 #실전리액트프로그래밍1장
- - - -
```
//file1.js
export default function func1() {}
export function func2(){}
export const variable1 = 123;
export let variable2 = 'hello';

//file2.js
import myFunc1, {func2, variable1, variable2} from './file1.js'

//file3.js
import {func2 as myFunc2} from './file1.js'
```

- file1.js 모듈에서 코드를 내보낼 때,
*export* 키워드를 사용한다.

- 가져오는 쪽은 *import* 키워드를 사용한다.

- *default* 키워드는 모듈에서 한 번만 사용 가능하다.

- *default* 키워드가 없다면, 괄호를 사용하여 가져올 수 있다.

- *as* 키워드를 이용하여, 별칭으로 사용할 수 있다.

