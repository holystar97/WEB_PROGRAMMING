# 2020/09/03/Thr, 1731017 김민경

<div>
<img width="451" alt="스크린샷 2020-09-03 오후 6 30 20" src="https://user-images.githubusercontent.com/35961898/92108614-a2738580-ee22-11ea-94b9-ef813317bc59.png">
<img width="366" alt="스크린샷 2020-09-03 오후 8 07 26" src="https://user-images.githubusercontent.com/35961898/92108622-a4d5df80-ee22-11ea-92fc-76c7f867a707.png">
<img width="504" alt="스크린샷 2020-09-03 오후 6 28 16" src="https://user-images.githubusercontent.com/35961898/92108626-a56e7600-ee22-11ea-9398-b301141492aa.png">
<img width="249" alt="스크린샷 2020-09-03 오후 8 01 55" src="https://user-images.githubusercontent.com/35961898/92108627-a56e7600-ee22-11ea-83dc-2f6254d5e878.png">
<img width="626" alt="스크린샷 2020-09-03 오후 6 38 15" src="https://user-images.githubusercontent.com/35961898/92108631-a6070c80-ee22-11ea-8de1-92534126643c.png">
<img width="565" alt="스크린샷 2020-09-03 오후 6 37 29" src="https://user-images.githubusercontent.com/35961898/92108644-aa332a00-ee22-11ea-928a-041dad482ccc.png">
</div>
#### 1. 오늘 강의의 주요 주제들은?



###### 1.1 HTML5 기본 문서 만들기 

```html
<!DOCTYPE html>
<html>
  <head>
    문서제목, 자바스크립트 코드, CSS 스타일 정의, 메타 데이터 정의
  </head>
  <body>
    문서의 본문 텍스트, 이미지, 테이블, 자바스크립트 코드, 동영상 등 
    <!--이것은 주석문입니다. -->
  </body>
</html>
```



> html 구성요소



* html의 구성원소는 tag 의 집합니다. 

태그는 태그이름과 여러 속성 (attribute)들로 구성이된다.

여기서 속성(attribute)는 속성이름과 값으로 구성된다. 



```html
<img src="apeach.jpg" width="100" height="50" alt="반가워 어피치">
```



여기서 `img` 는 tag의 이름

`src="apeach.jpg" , width="100" ,height="50",alt="반가워 어피치"` 는 attribute 

`src`  는 attribute 의 name

`apeach.jpg`	는 attribute의 value 가 된다. 



* 대부분의 경우 시작 tag와 종료 tag가 있다 
* 태그와 속성은 대소문자 구분이 없다





> Html 기본 문서 만들기







`title` 은 페이지의 제목 tag

`h1~h6` 까지는 문단 제목 tag

`title` 은  설명문(툴팁) 의 attribute

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>첫 타이틀</title>
</head>
<body>
<p>
    <h1 title="h1태그">페이지에 &nbsp;&nbsp; 타이틀을 다는 예제입니다.</h1>
</p>
<p>
    <h2>타이틀은 브라우저의 타이블 바에 보여집니다.</h2>
</p>
</body>
</html>
```

![스크린샷 2020-09-03 오후 6.28.16](/Users/mkrice/Desktop/스크린샷 2020-09-03 오후 6.28.16.png)



`p` 는 단락 나누기 tag  (br 대신에 단락을 구분할 때 쉽게 쓰임)

`hr` 은 수평선 긋기 tag (문단 내 내용의 전환이 필요한 곳에 주로 사용)

`br` 은 새로운 줄로 넘어갈 때 사용하는 tag

`pre` 는 개발자가 작성한 format를 그대로 출력하고 싶을때 사용하는 tag

`div` 는 division tag, 여러 html 태그들을 블록으로 묶는 컨테이너로 이용된다. 

`span` 은 확장의 의미를 가진 tag, 텍스트 일부분에 특별한 모양을 주거나 자바스크립트 코드로 텍스트 일부분을 제어하고자 할 때 사용한다.

`&nbsp` 은 빈칸 문자(기호) 를 코드로 표현한 것이다



다음은 메타 데이터 (데이터를 설명하는 데이터) 에 관한 tag 이다.

예를 들어 사진의 경우 찍은 장소와 시간 데이터가 메타 데이터,

오디오 파일의 경우 재생시간, 채널 수 가 메타 데이터,

이미지 파일의 경우 이미지 폭, 높이, 컬러 해상도 정보가 메타 데이터이다. 

html은 이와 같은 메타 정보를 표현하기 위해 여러 tag 를 가진다. 

` <base> ,<link>,<script>,<style>,<title>,<meta>`  등이 있다. 

```html
<meta charset="UTF-8">
<meta name="author" content="minkyung"
```



> Html 고급 문서 만들기



`img`  이미지 삽입 tag 

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>이미지 삽입</title>
</head>
<body>
<h3>이미지 삽입</h3>
<hr>
<p>어피치의 사진입니다.</p>
<img src="images/a.jpg" width="150" height="200" alt="apeach">
<img src="b.jpg" width="80" height="100" alt="apeach 사진 없음">
<img src="https://www.google.co.kr/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png" alt="사진 주소 변경됨"
     width="100" height="100">
</body>
</html>
```



![스크린샷 2020-09-03 오후 6.30.20](/Users/mkrice/Desktop/스크린샷 2020-09-03 오후 6.30.20.png)

`<ol>, <ul>,<dl>`  리스트 만들기 tag

1. ol - ordered list 
2. ul - unordered list
3. dl - definition list 



`tabel` 표 만들기 tag

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>좋아하는 카카오 프렌즈</title>
</head>
<body>
    <table>
        <caption>좋아하는 캐릭터</caption>
        <tbody>
            <tr>
                <td><img src="images/apeach2.jpg"></td>
                <td><img src="images/lion2.jpg"></td>
                <td><img src="images/tube2.jpg"></td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```

![스크린샷 2020-09-03 오후 6.33.06](/Users/mkrice/Desktop/스크린샷 2020-09-03 오후 6.33.06.png)



`<a>`  하이퍼링크 만들기  tag



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>사이트 리스트</title>
</head>
<body>
    <h4>사이트 리스트</h4>
    <ul>
        <li><a href="http://www.w3c.org" target="right">W3C</a></li>
        <li><a href="http://www.etnews.com" target="_self">전자신문</a></li>
        <li><a href="http://www.mk.co.kr" target="_top">매일경제신문</a></li>
        <li><a href="http://www.w3c.org" target="_blank">새 창에 W3C</a></li>
    </ul>

</body>
</html>
```

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>target 속성 활용</title>
</head>
<body>
<h3>target 속성 활용</h3>
<hr>
    <iframe src="ex2-2-24-sitelist.html" name="left" width="200" height="300"></iframe>
    <iframe src="http://www.w3c.org" name="right" width="300" height="300">s</iframe>
</body>
</html>
```

![스크린샷 2020-09-03 오후 6.37.29](/Users/mkrice/Desktop/스크린샷 2020-09-03 오후 6.37.29.png)

`<iframe>` 인라인 프레임 만들기 tag

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>iframe 를 이용한 캐릭터 사이트</title>
</head>
<body>
    <h3>2개의 캐릭터 사이트입니다.</h3>
    <hr>
    <iframe src="https://store.kakaofriends.com/kr/index?tab=home" name="upper" width="300" height="300"> </iframe>
    <iframe src="https://www.linefriends.com/?lang=ko" name="lower" width="300" height="300"> </iframe>
</body>
</html>
```



![스크린샷 2020-09-03 오후 6.38.15](/Users/mkrice/Desktop/스크린샷 2020-09-03 오후 6.38.15.png)

target 속성은 `<a>, <base>, <area>, <form> ` tag에서 html 페이지를 출력할 윈도우를 지정하는 데 사용된다.

다음은 target attribute 의 value 이다.

`_blank`  새로운 브라우저 윈도우(탭 ) 생성

`_self`  현재 윈도우

`_parent` 부모 윈도우

` _top` 최상위 브라우저 윈도우



`<audio>, <video>`  미디어 삽입 tag

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>오디오 삽입</title>
</head>
<body>
    <h3>오디오 삽입</h3>
    <hr>
    페이지 로드 즉시 음악이 연주됩니다.
    <audio controls autoplay loop src="audio/music.mp3">
        브라우저가 audio 태그를 지원하지 않습니다.
    </audio>
</body>
</html>
```



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>비디오 삽입</title>
</head>
<body>
<h3>비디오 삽입</h3>
<hr>
    페이지 로드 즉시 영상이 재됩니다.
    <video controls autoplay loop src="video/leafs_and_drops_03.mov" width="200" height="200">
        브라우저가 audio 태그를 지원하지 않습니다.
    </video>
</body>
</html>
```



###### 1.2 html 문서 구조화와 웹폼

> 시멘틱 웹 

웹 문서를 구조화하여 의미 있는 내용탐색이 용이하도록 하는 웹 을 구현하고자 한다. 

> 시멘틱 tag

`<header>, <section>,<article>,<main>,<summary>,<mark> `  등

`<figure>` 은 본문에 사빙ㅂ된 그림을 블록화하는 시멘틱 태그이다 

`<details> / <summary>` 상세정보를 담는 시멘틱 블록 태그 / details로 구성되는 블록의 제목의 표현

> 시멘틱 인라인 tag

`<mark>,<time>,<meter>,<progress>` 

중요한 텍스트임을 표시

시간 정보 표시

주어진 범위나 %의 데이터 양 표시

작업의 진행 정도 표시 



> 웹 폼
>
> 간단한 로그인 폼 만들기



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>로그인 폼</title>
</head>
<body>
    <h3>로그인 폼</h3>
    <hr>
    <form name="fo" method="get">
        사용자 id : <input type="text" size="15" value=""><br>
        비밀 번호: <input type="password" size="15" value="">
                <input type="submit" value="완료">
    </form>
</body>
</html>
```

![스크린샷 2020-09-03 오후 8.01.55](/Users/mkrice/Desktop/스크린샷 2020-09-03 오후 8.01.55.png)

`name` : 폼의 이름을 지정하는 속성 



`action` : 폼 데이터를 처리할 웹 서버 응용프로그램을 지정

submit 버튼이 클릭되면 브라우저는 action 속성에 지정된 웹 서버에 연결하고 웹 서버 응용프로그램을 실행할 것을 지시

이때 사용자가 입력한 폼 데이터를 함께 전송 



`method` : 폼 데이터를 웹 서버로 전송하는 형식 

Get/ post 방식이 있다.



> 폼 만들기



```html
<input type="text">
<input type="password">
<input type="button">
<input type="submit">
<input type="reset">
<input type="image">
<input type="checkbox|radio">
<select>
</select>
<button type="button|reset|submit">
</button>
<textarea></textarea>
```



> 데이터 목록을 가진 텍스트 입력 창 ,<datalist>



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>데이터 목록을 가진 텍스트 입력</title>
</head>
<body>
    <h3>가보고 싶은 곳 </h3>
    <hr>
    <form>
        나라: <input type="text" list="countries"><br>
            <datalist id="countries">
                <option value="가나"></option>
                <option value="스위스"></option>
                <option value="브라질"></option>
            </datalist>
        보고싶은 것: <input type="text" list="what"><br>
        <datalist id="what">
            <option value="산"></option>
            <option value="바다"></option>
            <option value="도시"></option>
        </datalist>
    </form>
</body>
</html>
```

![스크린샷 2020-09-03 오후 8.07.26](/Users/mkrice/Desktop/스크린샷 2020-09-03 오후 8.07.26.png)





> 라디오 버튼 



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>캡션을 가진 라디오버튼</title>
</head>
<body>
    <h3>갖고 싶은 것 하나만 선택? (&lt;label&gt;이용)</h3>
    <hr>
    <form>
        <label>
            <input type="radio" name="china" value="1">
            어피치 <img src="images/apeach2.jpg">
        </label><br>
        <label>
            <input type="radio" name="china" value="2">
            라이언 <img src="images/lion2.jpg">
        </label><br>
        <label>
            <input type="radio" name="china" value="3">
            튜브 <img src="images/tube2.jpg">
        </label><br>

    </form>


</body>
</html>
```



![스크린샷 2020-09-03 오후 8.08.41](/Users/mkrice/Desktop/스크린샷 2020-09-03 오후 8.08.41.png)



여기서 name 은 모두 같게 설정하는데, 이는 후에 자바스크립트에서 항목을 묶는데 사용된다.

그리고 value 로 각기 다른 값을 설정하여, 선택된 값을 구별한다.



> Label

캡션과 폼 요소를 묶는 방법이다. 



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>로그인 폼</title>
</head>
<body>
    <h3>로그인 폼</h3>
    <hr>
    <form name="fo" method="get">
        <label>사용자 id : <input type="text" size="15" value="" placeholder="apache name: "></label><br>
        비밀 번호: <input type="password" size="15" value="">
                <input type="submit" value="완료">
    </form>
</body>
</html>
```





이와 같이 지정할 경우, input text 부분 말고 한 label로 묶인 사용자 Id 를 선택해도 text 창이 눌러지는 효과가 있다. 



#### 2. 질문사항: 의문이 해소되지 않은 부분은?



###### - 없습니다. 감사합니다.

