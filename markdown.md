# 마크다운 문법정리


헤더
=============

```
헤더
=============
```


작은제목
-------------

```
작은제목
-------------
```


## 글머리: 1~6까지만 지원

# 글머리1
## 글머리2
### 글머리3
#### 글머리4
##### 글머리5
###### 글머리6
```
# 글머리1
## 글머리2
### 글머리3
#### 글머리4
##### 글머리5
###### 글머리6
```

## 블럭인용문자
> 첫번째 블럭인용
>	> 두번째 블럭인용
>	>	> 세번째 블럭인용

```
> 첫번째 블럭인용
>	> 두번째 블럭인용
>	>	> 세번째 블럭인용
```

## 목록
### 순서있는 목록(번호)
순서는 무조건 번호의 내림차순으로만 작성 가능함.
1. 첫번째
2. 세번째
3. 두번째

```
1. 첫번째
2. 세번째
3. 두번째
```

### 순서없는 목록(글머리 기호:*,+,- 지원)
혼합해서 사용 가능함.

* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑

    ```
    * 빨강
        * 녹색
            * 파랑

    + 빨강
        + 녹색
            + 파랑

    - 빨강
        - 녹색
            - 파랑
    ```

## 코드

### 들여쓰기
4개의 공백 또는 하나의 탭으로 들여쓰기를 만나면 변환되기 시작하여 들여쓰지 않은 행을 만날때까지 변환이 계속된다.

### 코드블럭
아래 2가지 방식으로 사용 가능함.
- ```<pre><code>{code}</code></pre>``` 이용방식
```
<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }

}
</code>
</pre>
```

- 코드블럭코드( ``` ) 이용방식
<pre>
<code>
```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
</code>
</pre>

깃헙에서는 코드블럭코드(```) 시작점에 사용하는 언어를 선언하여 문법강조(Syntax highlighting)이 가능함.

<pre>
<code>
```C++
int main(){
    cout << "Hello World!";
}
```
</code>
</pre>

아래처럼 C++ 문법이 강조됨
```C++
int main(){
    cout << "Hello World!";
}
```

## 수평선 ```<hr/>```
아래 줄은 모두 수평선을 만든다. 마크다운 문서를 미리보기로 출력 시, 페이지 나누기 용도로 많이 활용됨.

```
* * *

***

*****

- - -

---------------------------------------

```

- 적용예시

* * *

***

*****

- - -

---------------------------------------

## 링크
- 참조링크
```
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"

```
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"

- 외부링크
```
[Google](https://google.com, "google link")
```
[Google](https://google.com, "google link")

- 자동연결
```
일반적인 URL 혹은 이메일주소인 경우 적절한 형식으로 링크를 형성한다.
* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>
```

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>


## 강조

```
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
_Italic_
<u>Underline: use `u`</u>
```

- *single asterisks*
- _single underscores_
- **double asterisks**
- __double underscores__
- ~~cancelline~~
_Italic_
<u>Underline: use `u`</u>

```> 문장 중간에 사용할 경우, **띄어쓰기**를 사용하는 것이 좋다.```
> 문장 중간에 사용할 경우, **띄어쓰기**를 사용하는 것이 좋다.

## 이미지

```
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")
```

![Alt text](./img.jpg)

- 사이즈 조절

```
<img src="./img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<img src="./img.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>
```
<img src="./img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="lauraadai"></img><br/>
<img src="./img.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="lauraadai"></img>

## 줄바꿈
엔터키(\n)만으로는 줄바꿈이 되지 않으므로, 문장 마지막에서 2칸 띄어쓰기 후 엔터키를 눌러야함.
```
줄바꿈\n (엔터)
줄바꿈__\n (띄어쓰기 2칸 후 엔터)
줄바꿈
```
줄바꿈
줄바꿈  
줄바꿈

## 표
### 일반적인 표
- 테이블 안에 ```|``` 파이프 기호를 사용하려면 파이프 기호 대신에 ```&#124;```를 입력
```
|제목|&#124;내용&#124;|설명|
|------|---|---|
|테스트1|테스트2|테스트3|
|테스트1|테스트2|테스트3|
|테스트1|테스트2|테스트3|
```
|제목|&#124;내용&#124;|설명|
|------|---|---|
|테스트1|테스트2|테스트3|
|테스트1|테스트2|테스트3|
|테스트1|테스트2|테스트3|

### 셀 정렬
- ```:``` 문자로 정렬을 정의
```
|제목|내용|설명|
|:---|---:|:---:|
|왼쪽정렬|오른쪽정렬|중앙정렬|
|왼쪽정렬|오른쪽정렬|중앙정렬|
|왼쪽정렬|오른쪽정렬|중앙정렬|
```
|제목|내용|설명|
|:---|---:|:---:|
|왼쪽정렬|오른쪽정렬|중앙정렬|
|왼쪽정렬|오른쪽정렬|중앙정렬|
|왼쪽정렬|오른쪽정렬|중앙정렬|

### 셀 확장
- 사이가 비어있으면 자동으로 확장
```
|제목|내용|설명|
|:---|:---:|---:|
||중앙에서확장||
|||오른쪽에서 확장|
|왼쪽에서확장||
```
|제목|내용|설명|
|:---|:---:|---:|
||중앙에서확장||
|||오른쪽에서 확장|
|왼쪽에서확장||

### 셀 강조
- 일반적인 text와 마찬가지로 ```*``` 와 ```**``` 를 통해 이탤릭/강조를 표시할 수 있습니다. ```span tag를``` 사용하면 컬러도 표시 가능

```
|제목|내용|설명|
|---|---|---|
|테스트1|*강조1*|테스트3|
|테스트1|**강조2**|테스트3|
|테스트1|<span style="color:red">강조3</span>|테스트3|
```

|제목|내용|설명|
|---|---|---|
|테스트1|*강조1*|테스트3|
|테스트1|**강조2**|테스트3|
|테스트1|<span style="color:red">강조3</span>|테스트3|

## 참고 문서

[ihoneymon : [공통] 마크다운 markdown 작성법](https://gist.github.com/ihoneymon/652be052a0727ad59601)  
[gparkkii  : 마크다운 markdown 사용법 총정리 - 기본편](https://gparkkii.github.io/tech/markdown/)  
[Unsplash  : laura adai](https://unsplash.com/ko/@lauraadaiphoto?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash)