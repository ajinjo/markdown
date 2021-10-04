# markdown

마크다운이란
일반 텍스트 기반의 경량 마크업 언어로 Github의 README에서 퍼져나가 현재는 Notion, Velog, Tistory 등 여러 곳에서 마크다운을 지원하니 한번 익혀두면 웬만한 곳에서 사용할 수 있다.

1. 헤더
마크다운 형식
#의 개수로 H1부터 H6까지 가능하다.

# H1
## H2
### H3
#### H4
##### H5
###### H6
HTML 형식
<>로 열고 </>으로 닫아주는 HTML의 태그도 사용이 가능하다.

<h1>H1</h1>
<h2>H2</h2>
<h3>H3</h3>
<h4>H4</h4>
<h5>H5</h5>
<h6>H6</h6>
H1
H2
H3
H4
H5
H6
==와 --으로 H2까지 표현할 수 있다. (개수 상관 없음.)

header1
=======
header2
-------
H1
H2
Notion은 ### header3까지만 지원한다.
여기로 넘어온 이유 중 하나.

2. 텍스트 스타일링
마크다운 형식
**볼드체**, __볼드체__
*이탤릭체*, _이탤릭체_
~~취소선~~
HTML 형식
<b>Bold</b>는 안된다.

<strong>Bold</strong>
<i>이탤릭체</i>, <em>이탤릭체</em>
<del>취소선</del>, <strike>취소선</strike>
<u>밑줄</u>, <ins>밑줄</ins>
<sup>윗첨자</sup>
<sub>아래첨자</sub>
<small>작은 글자</small>
<big>큰 글자</big>
볼드체
이탤릭체
취소선
밑줄
여기의윗첨자
여기의아래첨자
작은 글자
큰 글자

미리보기 화면에는 잘 나오는데 작성완료를 누르면 볼드체, 이텔릭체, 취소선만 적용이 된다.


2.1 공백
Velog에서는 아무리 스페이스바를 눌러 띄어쓰기를 해도 결과는 하나의 띄어쓰기만 적용된다. &nbsp;를 사용하면 공백을 넣을 수 있다.

이런식&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;으로
이런식     으로

3. 인용
마크다운 형식
>으로 인용문을 작성할 수 있다.

HTML 형식
<Blockquote>
인용
</Blockquote>
인용

>의 개수에 따라 >>, >>> 중첩도 가능하다.

한 개

두 개

세 개

4. 링크
마크다운 형식
인라인 링크
[링크 설명](http://www.google.co.kr)

url 링크
<http://www.google.co.kr>
HTML 형식
<a href="http://www.google.co.kr">HTML 링크 설명</a>
새 탭으로 띄우기
<a href="http://www.google.co.kr" target="_blank">링크이름</a>
링크 설명
http://www.google.co.kr
HTML 링크 설명
새 탭

5. 이미지
마크다운 형식
인라인 링크 앞에 ! 를 붙여주면 이미지 링크가 된다.

![이미지 설명](이미지 링크)
![google](https://www.google.co.kr/images/branding/googlelogo/2x/googlelogo_color_160x56dp.png)


이미지 클릭시 해당 url로 연결

[![이미지 설명](이미지 링크)](클릭시 연결될 url)
[![google](https://www.google.co.kr/images/branding/googlelogo/2x/googlelogo_color_160x56dp.png)](http://www.google.co.kr)


HTML 형식
<img src="https://www.google.co.kr/images/branding/googlelogo/2x/googlelogo_color_160x56dp.png" alt="google">

링크 태그 안에 이미지 태그를 넣어주면 된다.

<a href="http://www.google.co.kr">
<img src="https://www.google.co.kr/images/branding/googlelogo/2x/googlelogo_color_160x56dp.png" alt="google">
</a>


6. 코드 블럭
마크다운 형식
```　
백틱(`)을 위, 아래 세 개로 감싸서 사용할 수 있다.
```　
이렇게 세 개로 감싸서 사용할 수 있다.
6.1 인라인 코드
백틱으로 양 옆을 감싸면 인라인 코드를 사용할 수 있다.

7. 하이라이팅
다양한 언어 하이라이팅을 지원하는데

```html 백틱 옆에 해당 언어를 소문자로 적어주면 자동으로 하이라이팅을 해준다.
HTML

<!DOCTYPE html>
<html>
<head>
<title>hello</title>
</head>
<body>
   Hello World!
</body>
</html>
JAVA

public class hello {
   public static void main(String[] args) {
      System.out.println("Hello, world!");
   }
}
Python

def hello():
    print('Hello, world!')
hello()
8. 리스트
마크다운 형식
- 하이픈, * 별표, + 더하기 모두 순서가 필요없는 같은 서브 리스트 기호다.

1. 순서가 필요한 리스트
   2. 순서가 필요한 서브 리스트
      2.1 순서가 필요한 서브 리스트
      
1. 순서가 필요한 목록
   - 순서가 필요없는 서브 리스트
   - 순서가 필요없는 서브 리스트
  
- 순서가 필요없는 서브 리스트 기호
   - 하이픈
   * 별표
   + 더하기

- 같은 기호라도
   - 탭(Tab)으로
      - 다른 기호를 낼 수 있다.
순서가 필요한 리스트
1.1 순서가 필요한 서브 리스트
순서가 필요한 리스트
순서가 필요없는 서브 리스트
순서가 필요없는 서브 리스트
순서가 필요없는 서브 리스트 기호
하이픈
별표
더하기
같은 기호라도
탭(Tab)으로
다른 기호를 낼 수 있다.
HTML 형식
<ol>
  <li>순서가 필요한 리스트</li>
  <li>순서가 필요한 리스트</li>
</ol>

<ul>
  <li>순서가 필요없는 서브 리스트</li>
  <li>순서가 필요없는 서브 리스트</li>
    <ol>
      <li>순서가 필요한 리스트</li>
      <li>순서가 필요한 리스트</li>
    </ol>
</ul>
순서가 필요한 리스트
순서가 필요한 리스트
순서가 필요없는 서브 리스트
순서가 필요없는 서브 리스트
순서가 필요한 리스트
순서가 필요한 리스트
9. 체크박스
마크다운 형식
[] 대괄호의 앞, 뒤로 띄어쓰기를 주어야 한다.

- [ ] : false
- [x] : true


텍스트 스타일링과 같이 미리보기 결과에는 이렇게 잘 뜨지만 작성완료를 하면 누르는 체크박스로 바뀌게 된다.

(어째서지...)


10. 수평선
마크다운 형식
3개 이상으로 적으면 수평선이 그어진다.

---
***
___
HTML 형식
<hr/>
11. 테이블
마크다운 형식
--- 기본 정렬
:--- 왼쪽 정렬
---: 오른쪽 정렬
:---: 가운데 정렬

| 제목 | 제목 | 제목 |
| :--- | :---: | ---: |
| 내용 | 내용 | 내용 |
| 내용 | 내용 | 내용 |
제목	제목	제목
내용	내용	내용
내용	내용	내용
HTML 형식
<table>
  <tr>
    <th>제목</th>
    <th>제목</th>
    <th>제목</th>
  </tr>
  <tr>
    <td>내용</td>
    <td>내용</td>
    <td>내용</td>
  </tr>
  <tr>
    <td>내용</td>
    <td>내용</td>
    <td>내용</td>
  </tr>
</table>
제목	제목	제목
내용	내용	내용
내용	내용	내용
11.1 셀 병합
HTML 형식
colspan=" " 열(column) 병합

<table>
  <tr>
    <td>내용</td>
    <td>내용</td>
  </tr>
  <tr>
    <td colspan="2">내용</td>
  </tr>
</table>
내용	내용
내용
미리보기 화면에서는 셀이 병합되지만 작성완료하면 병합이 안된다.


rowspan=" " 행(row) 병합

<table>
  <tr>
    <td rowspan="3">내용</td>
    <td>내용</td>
  </tr>
  <tr>
    <td>내용</td>
  </tr>
  <tr>
    <td>내용</td>
  </tr>
</table>
내용	내용
내용
미리보기 화면에서는 셀이 병합되지만 작성완료하면 병합이 안된다.


12. 😌 이모지
💻 MacOS control + command + space bar

🖥 Windows window key + .
