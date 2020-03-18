[toc]

# 비즈니스 스타일 꾸미기(콘텐츠편)

## 1. 콘텐츠 페이지 작성해보기

### 1) 박스 준비

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="http://netdna.bootstrapcdn.com/font-awesome/4.2.0/css/font-awesome.css">
    <script src="http://code.jquery.com/jquery-1.11.1.min.js"></script>
</head>
<body>
    <header class="header">
        <div class="header-inner">
            <div class="box1">
                <div class="header-site">
                    <h1><a href="#"><img src="img/06/logo-large.png" alt="Business"></a></h1>
                </div>
            </div>
            <div class="box2">
                <button type="button" id="header-menubtn">
                    <i class="fa fa-bars"></i><span>MENU</span>
                </button>
                <nav class="header-nav" id="menu">
                    <ul>
                        <li><a href="#">메인</a></li>
                        <li><a href="#">연혁</a></li>
                        <li><a href="#">사업 소개</a></li>
                        <li><a href="#">채용 정보</a></li>
                        <li><a href="#">문의</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
    
    <footer class="footer">
        <div class="box5-inner">
            <div class="copyright">
                Copyright &copy; Business CSS
            </div>
        </div>
    </footer>
    <script>
        $(function(){
            $("#header-menubtn").click(function(){
                $("#menu").slideToggle();
            });
                        
        });
    </script>
</body>
</html>
```

```css
@charset "UTF-8";

body{
    font-family: '맑은 고딕','Apple SD Gothic Neo',sans-serif;
    margin: 0;
}

/* 사이트 이름 */
.header-site h1{
    margin: 0;
    font-size: 30px;
}
.header-site h1 a{
    color: #000000;
    text-decoration: none;
}
.header-site img{
    border: none;
    width: 250px;
    height: 33px;
}


/* 헤더 그림 */
.topimg{
    max-width: 100%;
    height: auto;
    vertical-align: bottom;
}
/* 캐치 카피 */
.catch{
    margin: 0;
    font-size: 28px;
    position: absolute;
    bottom: 7%;
    left: 3%;
    padding: 15px;
    background-color: rgba(255, 255, 255, 0.7);
}
.top{
    position: relative;
}
/* 개요 */
.summery h1{
    margin-top: 0;
    margin-bottom: 0;
    font-size: 20px;
    font-weight: normal;
    padding: 5px 0;
}
.summery p{
    margin-top: 0;
    margin-bottom: 0;
    padding: 15px 5px;
    background-color: #524e3c;
}
.summery a{
    display: block;
    background-color: #222222;
    color: #ffffff;
    text-decoration: none;
    text-align: center;
}
.summery a:hover{
    opacity: 0.8;
}
.summery i{
    font-size: 38px;
    display: block;
    padding: 40px 0;
}
.summery .fa-database{
    background-color: #bfbd13;
}
.summery .fa-bar-chart-o{
    background-color: #f65d4a;
}
.summery .fa-envelope{
    background-color: #859f46;
}

/* 공지사항 */
.news{
    padding: 20px;
    border: solid 5px #dddddd;
}
.news h1{
    margin-top: 0;
    margin-bottom: 5px;
    font-size: 18px;
    color: #666666;
}
.news ul{
    margin: 0;
    padding: 0;
    list-style: none;
}

.news li a{
    text-decoration: none;
    display: block;
    padding: 5px;
    color: #000000;
    font-size: 14px;
    border-bottom: dotted 2px #dddddd;
}

.news li a:hover{
    background-color: #eeeeee;
}

.news time{
    color: #999999;
    font-weight: bold;
}

.news a:after{
    content: '';
    display: block;
    clear: both;
}
.news time{
    float: left;
    width: 60px;
}
.news .text{
    float: none;
    width: auto;
    margin-left: 60px;
}

/* 저작권 */
.copyright p{
    margin: 0;
    color: #666666;
    font-size: 14px;
}

/* footer를 바 형태로 디자인 */
.footer{
    background-color: #dddddd;
    padding-top: 15px;
    padding-bottom: 15px;
}

/* 박스의 왼쪽, 오른쪽 */
.header, .box4, .footer, .box6{
    padding-left: 15px;
    padding-right: 15px;
}

/* 박스의 위아래 */
.header {
    padding-top: 20px;
    padding-bottom: 10px;
}
.box4{
    padding : 20px 0;
}
.box4-1{
    padding-bottom: 20px;
}
.box6{
    padding-top: 20px;
}
.box6-1, .box6-2, .box6-3{
    padding-bottom: 10px;
}

/* SNS 매뉴 */
.follow ul{
    margin: 0;
    padding: 0;
    list-style: none;
}
.follow li a{
    display: block;
    margin-bottom: 10px;
    padding: 10px;
    border-radius: 4px;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
}
.follow li a:hover{
    opacity: 0.8;
}
.follow-tw{
    background-color: #63bafb;
}
.follow-fb{
    background-color: #5288f7;
}
.follow-gp{
    background-color: #f65d4a;
}
.follow i{
    margin-right: 10px;
    font-size: 24px;
    vertical-align: middle;
}
.follow p{
    margin-top: 0;
    margin-bottom: 20px;
    padding: 10px;
    background-color: #c1dd22f1;
    font-size: 14px;
    text-align: center;
}
.follow-info {
	position: relative;
	background: #f3ffaf;
}
.follow-info:after {
	top: 100%;
	left: 50%;
	border: solid transparent;
	content: " ";
	height: 0;
	width: 0;
	position: absolute;
	pointer-events: none;
	border-color: rgba(221, 221, 221, 0);
	border-top-color: #f3ffaf;
	border-width: 15px;
	margin-left: -15px;
}
/* ####### 599px 이하 ####### */
@media (max-width:599px){
    .header-site h1{
        margin: 0;
        font-size: 20px;
    }
    .header-nav li a{
        padding: 10px 7px;
        font-size: 11px;
    }
    
    /* 캐치 카피 */
    .catch{
        display: none;
    }
}

/* ####### 767px 이하 ####### */
@media (max-width:767px){

    /* 토글 버튼 */
    #header-menubtn{
        padding: 6px 12px;
        border: solid 1px #aaaaaa;
        border-radius: 5px;
        background-color: #ffffff;
        position: absolute;
        top: 20px;
        right: 15px;
        cursor: pointer;
    }
    #header-menubtn:hover{
        background-color: #dddddd;
    }
    #header-menubtn:focus{
        outline: none;
    }
    #header-menubtn i{
        color: #888888;
        font-size: 18px;
    }
    #header-menubtn span{
        display: inline-block;
        text-indent: -9999px;
    }
    #header-nav {
        display: none;
    }
    .header-nav ul{
        margin:0;
        padding:0;
        list-style:none;
    }
    .header-nav li a{
        display: block;
        padding:5px;
        color: #000000;
        font-size: 14px;
        text-decoration: none;
    }
    .header-nav li a:hover{
        background-color: #eeeeee;
    }
}

/* ####### 768px 이상 ####### */
@media (min-width:768px){

    /* 토글 버튼 */
    #header-menubtn{
        display: none;
    }

    /* 네비게이션 */
    #menu{
        display: block !important;
    }

    /* 네비게이션 */
    .header-nav ul{
        margin: 0;
        padding:0;
        list-style: none;
    }
    .header-nav li a{
        display: block;
        padding: 10px 15px;
        color: #000000;
        text-decoration: none;
        font-size: 14px;
        
    }
    .header-nav li a:hover{
        background-color: #eeeeee;
    }
    .header-nav ul:after{
        content:'';
        display: block;
        clear: both;
    }
    .header-nav li{
        float: left;
        width: auto;
    }

    /* BOX1과 BOX2를 가로 정렬하는 설정 */
    .header::after{
        content: '';
        display: block;
        clear: both;
    }
    .box1{
        float: left;
        width: auto;
    }
    .box2{
        float: right;
        width: auto;
    }

    /* BOX4-1과 BOX4-2를 가로 정렬하는 설정 */
    .box4::after{
        content: '';
        display: block;
        clear: both;
    }
    .box4-1{
        float: left;
        width: 70%;
        padding-right: 35px;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box;
        box-sizing: border-box;
    }
    .box4-2{
        float: left;
        width: 30%;
    }
    .box6:after{
        content: '';
        display: block;
        clear: both;
    }
    
    .box6-1{
        float: left;
        width: 32%;
        margin-right: 2%;
    }
    .box6-2{
        float: left;
        width: 32%;
        margin-right: 2%;
    }
    .box6-3{
        float: left;
        width: 32%;
    }
}

@media (min-width:1190px){

    /* 전체 너비를 고정 */
    .box3, .box4, .header-inner, .footer-inner, .box6{
        width: 1140px;
        margin: 0 auto;
    }

    /* BOX A 아래에 테두리 삽입 */
    .header {
        margin-bottom: 20px;
        border-bottom: solid 1px #dddddd;
    }
}
```

### 2) 콘텐츠 코딩

- 네브바 만들기
- 가로정렬하는 방법 학습

## 2. 요소 추가와 수정

### 1) 제목에 붉은색 바 추가하는 방법

```css
padding-left: 20px;
border-left: solid 20px #c50018;
```

### 2) 본문 너비의 최댓값을 지정하는 방법

```css
.story .lead {
    max-width: 100%;
    font-size: 20px;
    color: #666666;
}
```

### 3) 이미지 크기 맞추는 방법

```css
.storyimg{
    max-width: 100%;
    height: auto;
    margin-bottom: 20px;
}
```

### 4) 빵부스러기 링크 넣는 방법

- 302p

![image](https://user-images.githubusercontent.com/26649731/76914414-93912900-68fd-11ea-9e45-a930c1bf4f9d.png)

```html
<div class="bread">
    <ol>
        <li><a href="#">메인</a></li>
        <li><a href="#">사업 소개</a></li>
    </ol>
</div>
```

```css
/* 빵부스러기 리스트 */
.bread{
    margin-bottom: 20px;
}
.bread ol{
    margin: 0;
    padding: 0;
    list-style: none;
}
.bread li a{
    display: inline-block;
    color: #000000;
    text-decoration: none;
    font-size: 14px;
}
.bread li a:hover{
    background-color: #eeeeee;
}
.bread ol:after{
    content: '';
    display: block;
    clear: both;
}
.bread li{
    float: left;
    width: auto;
}
.bread li::after{
    content: '\003e';
    color: #888888;
    margin-left: 10px;
    margin-right: 10px;
}
```

### 5) 사이드바 디자인

![image](https://user-images.githubusercontent.com/26649731/76915878-1caa5f00-6902-11ea-9e1c-055cc2cb951f.png)

```html
<div class="box7-2">
            <aside class="sidemenu">
                <h1><i class="fa fa-caret-square-o-down"></i>사업 소개</h1>
                <ul>
                    <li><a href="#">데이터 축적</a></li>
                    <li><a href="#">데이터 분석/해석</a></li>
                    <li><a href="#">데이터 시각화</a></li>
                    <li><a href="#">애플리케이션 활용</a></li>
                    <li><a href="#">24시간 지원</a></li>
                    <li><a href="#">실적 소개</a></li>
                </ul>
            </aside>
        </div>
```

```css
/* 사이드 매뉴 */
.sidemenu{
    border: solid 6px #eeeeee;
}
.sidemenu h1{
    margin: 0;
    font-size: 16px;
    font-weight: normal;
    padding: 10px;
}
.sidemenu h1 i{
    margin-right: 5px;
    color: #8abc60;
    font-size: larger;
}
.sidemenu ul{
    margin: 0;
    padding: 0;
    list-style: none;
}
.sidemenu li a{
    display: block;
    padding: 10px;
    color: #000000;
    font-size:14px;
    text-decoration: none;
    border-top: 1px solid #dddddd;
}
.sidemenu li a:hover{
    background-color: #eeeeee;
}
```

### 6) 글 단락 2단 구성

![image](https://user-images.githubusercontent.com/26649731/76916368-91ca6400-6903-11ea-96c0-dfaa346d289d.png)

- 311p

```html
<div class="story-body">
    <p>
        힘...바람이다.
    </p>
    	광야에서 .....인도하겠다는 열매를 돋고, 없으면, 듣는다.
    <p>d
        무엇이 유소... 것이다.
    </p>
</div>
```

```css
.story-body{
    margin-top: 40px;
    column-count: 2;
    column-gap: 40px;
}
```

