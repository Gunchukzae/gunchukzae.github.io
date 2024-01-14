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
_Italic
```

- *single asterisks*
- _single underscores_
- **double asterisks**
- __double underscores__
- ~~cancelline~~
_Italic

```> 문장 중간에 사용할 경우, **띄어쓰기**를 사용하는 것이 좋다.```
> 문장 중간에 사용할 경우, **띄어쓰기**를 사용하는 것이 좋다.

## 이미지

```
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")
```

![Alt text](/path/to/img.jpg)
![Alt text](/git/to/img.jpg "Optional title")

- 사이즈 조절

```
<img src="/path/to/img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<img src="/path/to/img.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>
```


참고글: [ihoneymon](https://gist.github.com/ihoneymon/652be052a0727ad59601)