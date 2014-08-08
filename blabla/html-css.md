---
layout: post
title: html과 css
categories: [html-css]
tags: [html, css]
fullview: false
---

1. [meta](#meta)  
1. [text](#text)  
1. [list](#list)  
1. [shadow](#shadow)  
1. [border](#border)  
1. [box-sizing](#box-sizing)  
1. [flexbox](#flexbox)  
1. [tablebox](#tablebox)  
1. [table](#table)  
1. [form](#form)  
1. [form - textarea](#textarea)  
1. [form - placeholder](#placeholder)  
1. [a11y_form](#a11y_form)  
1. [video](#video)  
1. [audio](#audio)  
1. [track](#track)  
1. [page-break](#page-break)  
1. [roll](#roll)  
1. [webkit](#webkit)  
1. [mobile_meta_link](#mobile_meta_link)  
1. [css_optimization](#css_optimization)  
1. [selector](#selector)  
1. [selector-before-after-data](#selector-before-after-data)  
1. [selector-child](#selector-child)  
1. [selector-string](#selector-string)  
1. [css_unit](#css_unit)  
1. [background](#background)  
1. [CSS_link](#CSS_link)  
1. [opacity](#opacity)  
1. [web_font](#web_font)  
1. [scrollbar](#scrollbar)  
1. [firefox_button](#firefox_button)  
1. [media_query](#media_query)  
1. [transition](#transition)  
1. [transform](#transform)  
1. [animation](#animation)  

---  
**example**  
1. <a href="http://smilesol85.github.io/blabla/view/html/line-clamp.html">line-clamp</a>  

## <a href="#" name="meta">meta</a>  
meta 태그 사용으로 해당 문서의 제목, 설명, 제작자 정보 등을 명시할 수 있다.  
	
	<!-- META 태그 LIST -->
	<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
	
	<!-- 페이지 자동 이동
	<meta http-equiv="refresh" content="2; url=http://www.naver.com/" />
	-->
	
	<!-- 전화번호 자동연결 차단 -->
	<!-- <a href="tel:010-1234-1234">전화걸기</a> -->
	<meta name="format-detection" content="telephone=no">
	
	<!-- document 정보 제목 -->
	<meta name="subject" content="문서 정보 제목" />
	
	<!-- document 제목 -->
	<meta name="title" content="문서 제목" />
	
	<!-- document 설명 -->
	<meta name="description" content="문서 설명, 검색 결과에 일부 설명으로 사용될 수 있다." />
	
	<!-- document 정보 -->
	<meta name="keywords" content="문서 정보" />
	
	<!-- document 제작자 정보 -->
	<meta name="author" content="문서 제작자 정보" />
	
	<!-- google 번역 링크 -->
	<meta name="google" content="notranslate" />
	
	<!-- 검색로봇 :  로봇 검색을 허가한다. -->
	<meta name="robots" content="all" />
	
	<!-- 검색로봇 : 로봇 검색을 허가하지 않는다. -->
	<meta name="robots" content="none" />
	
	<!-- 검색로봇 : 이 문서도 긁어가고 링크된 문서도 긁어간다. -->
	<meta name="robots" content="index,follow" />
	
	<!-- 검색로봇 : 이 문서는 긁어가지 말고 링크된 문서만 긁어간다. -->
	<meta name="robots" content="noindex,follow" />
	
	<!-- 검색로봇 : 이 문서는 긁어가되, 링크는 무시한다. -->
	<meta name="robots" content="index,nofollow" />
	
	<!-- 검색로봇 : 이 문서도 긁지 않고, 링크도 무시한다. -->
	<meta name="robots" content="noindex,nofollow" />
	
	<!-- document 대표 비디오 -->
	<link rel="video_src" href="비디오 url">
	
	<!-- 114x114 : 페이스북 썸네일로 사용 가능하다. 문서의 대표 이미지가 될 수 있겠다. -->
	<link rel="image_src" href="http://s-static.cubbying.com/static/images/common/thumbnail.png">
	
	<!-- 16x16 : www.favicon.com 에 접속해 아이콘 생성 -->
	<link rel="shortcut icon" type="image/x-icon" href="http://s-static.cubbying.com/static/favicon.ico">
	
	<!-- 114x114 애플 아이콘 -->
	<link rel="apple-touch-icon" href="http://s-static.cubbying.com/static/apple-touch-icon.png">
	
	<!-- opengraphics 태그 사용(facebook 이나 twitter 에 더욱 자세하게 표현하고 싶을 때)
	공식 홈페이지 (http://opengraphprotocol.org/, http://ogp.me/) -->
	<meta property="og:title" content="제목" />
	<meta property="og:description" content="페이지에 대한 요약" />
	<meta property="og:image" content="썸네일 이미지 주소" />
	<meta property="og:type" content="video" />
	<meta property="og:video" content="비디오 전송주소" />
	<!-- // META 태그 LIST -->

## <a href="#" name="text">text</a>  
	
	<!-- blockquote : 블록 요소 인용구 -->
	<blockquote>
		<blockquote>는 블록 요소의 인용문에서 사용된다.
	</blockquote>
	
	<!-- q : 인라인 요소 인용구 -->
	홍길동은 <q cite="http://www.naver.com/" title="title">blah blah~</q>알고 했습니다.
	<q> 인용구는 따옴표(" ")가 함께 표시된다.
	
	<!-- abbr : 인라인 요소 축약어 -->
	<abbr title="Apartmention">Apt.</abbr> : 스펠링 하나씩 발음하는 경우나 줄여서 단어를 단순하게 사용하는 경우
	
	<!-- acronym : inline element 축약어 -->
	<acronym title="Rich Internet Application">RIA</acronym> : 여러단어 조합
	
	<!-- font 
	<b> 굵은 글자 태그 </b>
	<i> 기울어진 글자 태그 </i>
	<small> 작은 글자 태그 </small>
	<sub> 아래에 붙는 글자 </sub>
	<sup> 위에 붙는 글자 </sup>
	<ins>  밑줄 글자 태그 </ins>
	<del> 가운데 줄이 그어진 글자 태그 </del>
	-->

## <a href="#" name="list">list</a>  
리스트 표현을 위해 ul, ol, dl 3가지 태그가 있다.  
- ul (Unordered List)  
- ol (Ordered List)  
- dl (Definition List)  

	
	<ul>
	<li>ul > li</li>
	<li>ul > li</li>
	</ul>

	<ol>
	<li>ol > li</li>
	<li>ol > li</li>
	</ol>

	<dl>
	<dt>dl > dt</dt>
	<dd>dl > dd</dd>
	</dl>

	<style>
	/* list style
		list-style:disc;
		list-style:circle;
		list-style:square;
		list-style:decimal;
		list-style:lower-roman;
		list-style:upper-roman;
		list-style:lower-alpha;
		list-style:upper-alpha;
	*/
	ul {list-style:square url("test.jpg");}
	</style>

## <a href="#" name="shadow">shadow</a>  
<a href="http://smilesol85.github.io/blabla/view/html/shadow.html">shadow</a>  
텍스트, 박스 영역에 그림자 효과를 적용할 수 있다.  
	
	.shadow1{box-shadow:5px 5px 10px red;text-shadow:5px 5px 10px blue}
	.shadow2{box-shadow:0 0 10px red;text-shadow:0 0 10px blue}
	.shadow3{box-shadow:0 0 0 1px red}
	.shadow4{box-shadow:0 10px 10px -5px red}
	.shadow5{box-shadow:inset 0 -10px 10px -8px red}
	.shadow6{box-shadow:inset 0 0 5px red}
	.shadow7{box-shadow:inset 0 -4px 10px red,inset -8px 0 10px red,inset 0 1px 10px red,inset 20px 0 10px red}
	.shadow8{box-shadow:0 0 1px 2px purple,0 0 1px 4px blue,0 0 1px 6px green,0 0 1px 8px yellow,0 0 1px 10px orange,0 0 1px 12px red}

## <a href="#" name="border">border</a>  
<a href="http://smilesol85.github.io/blabla/view/html/border.html">border</a>  
	
	/* border-radius */
	*{border-radius:10px}
	div{border-top-right-radius:10px}
	
	/* border-width */
	*{border-width:10px}
	div{border-top-width:10px}
	
	/* border-style */
	*{border-style:solid}
	div{border-right-style:solid}
	
	/* border-color */
	*{border-color:red}
	div{border-bottom-color:red}

##<a href="#" name="box-sizing">box-sizing</a>  
<a href="http://smilesol85.github.io/blabla/view/html/box-sizing.html">box-sizing</a>  
	
	/* border를 포함 */
	.box2{box-sizing:border-box}
	
	/* border를 포함하지 않음 */
	.box3{box-sizing:content-box}

##<a href="#" name="flexbox">flexbox</a>  
<a href="http://smilesol85.github.io/blabla/view/html/flexbox.html">flexbox</a>  
flexbox 사용은 box안의 요소들은 `블록 요소`라는 조건이 있다.  

	
	/* 부모 요소에 box 선언 */
	.box{display:box;display:-webkit-box}
	
	/* 상단 정렬 */
	.oBox2{-webkit-box-orient:vertical;-webkit-flex-direction:column;height:100px}
	
	/* 좌측 정렬 */
	.oBox3{-webkit-box-pack:start}
	
	/* 우측 정렬 */
	.oBox4{-webkit-box-pack:end}
	
	/* 일정 간격으로 정렬 */
	.oBox5{-webkit-box-pack:justify}
	
	/* 가운데 정렬 */
	.oBox6{-webkit-box-pack:center}
	
	/* 좌측 상단 정렬 */
	.oBox7{-webkit-box-align:start}
	
	/* 좌측 하단 정렬 */
	.oBox8{-webkit-box-align:end}
	
	/* 좌측 가운데 정렬 */
	.oBox9{-webkit-box-align:center}
	
	/* 왼쪽 상단 정렬 */
	.oBox10{-webkit-box-align:baseline}
	
	/* 왼쪽 정렬 */
	.oBox11{-webkit-box-align:stretch}
	
	/* 각 box 영역 정렬 */
	.box .oBoxE1{-webkit-box-flex:1}
	.box .oBoxE2{-webkit-box-flex:20}
	.box .oBoxE3{-webkit-box-flex:1}
	
	/* 각 box 순서 강제 정렬 */
	.box .oBoxE1{-webkit-box-ordinal-group:2}
	.box .oBoxE2{-webkit-box-ordinal-group:1}
	.box .oBoxE3{-webkit-box-ordinal-group:3}

##<a href="#" name="tablebox">tablebox</a>  
<a href="http://smilesol85.github.io/blabla/view/html/tablebox.html">tablebox</a>  

display:table-header-group, display:table-footer-group 은  
인라인으로 height값이 적용되지 않으며, line-height로 사용한다.  
	
	<style>        
	.boxes{display:table}
	.box4{background:gray}
	
	/* footer */
	.box1{background:red;display:table-footer-group;line-height:40px}
	
	/* caption */
	.box2{background:green;display:table-caption}
	
	/* header */
	.box3{background:white;display:table-header-group;line-height:40px}
	</style>
	
	<div class="boxes">
		<div class="box1">one => display:table-footer-group<p>table-footer-group은 i인라인으로 height값이 적용되지 않으며, line-height로 사용</p></div>
		<div class="box2">two => display:table-caption</div>
		<div class="box3">three => display:table-header-group<p>table-header-group은 인라인으로 height값이 적용되지 않으며, line-height로 사용</p></div>
		<div class="box4">four</div>
	</div>

## <a href="#" name="table">table</a>  
	
	<table border="1" summary="2학년 9반 개인별 성적입니다.">
	    <caption>2학년 9반 개인별 성적 목록</caption>
	    <colgroup>
	        <col width="100">
	      <col width="100">
	    	<col width="100">
	    </colgroup>
	    <thead>
	        <tr>
	            <th scope="col">홍길동</th>
	            <th scope="col">박한솔</th>
	            <th scope="col">이진권</th>
	        </tr>
	    </thead>
	    <tbody>
	        <tr>
	            <td>수학 0점</td>
	            <td>수학 0점</td>
	            <td>수학 0점</td>
	        </tr>
	        <tr>
	            <td>영어 0점</td>
	            <td>영어 0점</td>
	            <td>영어 0점</td>
	        </tr>
	    </tbody>
	    <tfoot>
	        <tr>
	            <td>평균 0점</td>
	            <td>평균 0점</td>
	            <td>평균 0점</td>
	        </tr>
	    </tfoot>
	</table>

- summary: table 내용 요약  
- caption: table 제목 및 설명문  
- th: table 제목 cell  
- td: table 데이터 cell  
- colgroup: 열 전체를 그룹 지정  
- col: 열 각각의 속성 지정  

## <a href="#" name="form">form</a>  
<a href="http://smilesol85.github.io/blabla/view/html/form.html">form</a>  
	
	<!-- form method : get || post -->
	<form action="#" method="get">
		<fieldset>
			<legend>HTML input type</legend>
			<label for="fhidden">hidden</label><input type="hidden" id="fhidden"><br>
            <label for="fbutton">button</label><input type="button" id="fbutton"><br>
            <label for="fimage">image</label><input type="image" id="fimage"><br>
            <label for="fcheckbox">checkbox</label><input type="checkbox" id="fcheckbox"><br>
            <label for="fradio">radio</label><input type="radio" id="fradio"><br>
            <label for="ffile">file</label><input type="file" id="ffile"><br>
            <label for="ftext">text</label><input type="text" id="ftext" placeholder="text"><br>
            <label for="fpassword">password</label><input type="password" id="fpassword"><br>
            <label for="fsubmit">submit</label><input type="submit" id="fsubmit"><br>
            <label for="freset">reset</label><input type="reset" id="freset"><br>
            <label for="age">연령</label>
            <select id="age">
                <option>10대</option>
                <option>20대</option>
                <option>30대</option>
                <option>40대</option>
            </select>
            <input type="submit" />
            <br>
            <label for="num">숫자</label>
            <select id="num" size="5" multiple="multiple">
                <option value="a">1</option>
                <option value="b">2</option>
                <option value="c">3</option>
                <option value="d">4</option>
            </select>
            <input type="submit" />
            <br>
            <label for="se">성별</label>
            <select id="se">
                <optgroup label="남자">
                    <option>남1</option>
                    <option>남2</option>
                    <option>남3</option>
                </optgroup>
                <optgroup label="여자">
                    <option>여1</option>
                    <option>여2</option>
                    <option>여3</option>
                </optgroup>
            </select>
            <input type="submit" />
		</fieldset>
		<fieldset>
            <legend>HTML5 add input type (Opera browser is all support, other browser is partial support October 2012)</legend>
            <label for="fcolor">color</label><input type="color" id="fcolor"><br>
            <label for="fdate">date</label><input type="date" id="fdate"><br>
            <label for="fdatetime">datetime</label><input type="datetime" id="fdatetime"><br>
            <label for="fdatetime-local">datetime-local</label><input type="datetime-local" id="fdatetime-local"><br>
            <label for="fmonth">month</label><input type="month" id="fmonth"><br>
            <label for="fweek">week</label><input type="week" id="fweek"><br>
            <label for="ftime">time</label><input type="time" id="ftime"><br>
            <label for="femail">email</label><input type="email" id="femail"><br>
            <label for="fnumber">number</label><input type="number" id="fnumber"><br>
            <label for="frange">range</label><input type="range" id="frange"><br>
            <label for="fsearch">search</label><input type="search" id="fsearch"><br>
            <label for="ftel">tel</label><input type="tel" id="ftel"><br>
            <label for="furl">url</label><input type="url" id="furl">
        </fieldset>
	</form>
    
## <a href="#" name="textarea">textarea</a>  
- name : 요소 이름 지정  
- cols : 가로로 쓰여지는 텍스트 수  
- rows : 세로로 쓰여지는 텍스트 수  
- readonly : 클릭은 되나 택스트를 입력할 수 없습니다.  
- disabled : 클릭조차 되지 않으며 사용하지 않는 경우입니다.  

**readonly="readonly" disabled="disabled"**
    
	<textarea name="textarea_name" cols="30" rows="5" readonly="readonly" disabled="disabled" onclick="this.value=''">
	텍스트를 입력하세요.
	</textarea>

**readonly="readonly"**
    
	<textarea name="textarea_name" cols="30" rows="5" readonly="readonly" onclick="this.value=''">
	텍스트를 입력하세요.
	</textarea>

**useable**
    
	<textarea name="textarea_name" cols="30" rows="5" onclick="this.value=''">
	텍스트를 입력하세요.
	</textarea>

## <a href="#" name="placeholder">placeholder</a>  
<a href="http://smilesol85.github.io/blabla/view/html/placeholder.html">placeholder</a>  

placeholder는 HTML5 DTD 에서 표준으로 추가되어 사용 가능하다.  
이렇게 되면 자바스크립트에서 입력폼에 포커스가 되면  
value를 초기화 하는 일은 불필요하게 된다.  

> placeholder는 android 하위 버전에서 텍스트 정렬이 되지 않는 버그가 있다.
> font-size 및 color는 사용 가능하다.
    
	<style>
	input::-webkit-input-placeholder{font-size:18px;color:red}
	</style>
	
	<input type="text" placeholder="텍스트를 입력">

## <a href="#" name="a11y_form">a11y_form</a>  
	
	<form>
		<fieldset>
			<legend>title</legend>
			<p><label for="userid">아이디</label><input type="text" id="userid"></input></p>
			<p><label for="userpw">비밀번호</label><input type="text" id="userpw"></input></p>
		</fieldset> 
	</form>

> label은 form을 구조화하고 접근성을 높일 수 있다.  
	웹 표준을 지원하는 브라우저의 경우 label만 선택해도 form control을 선택할 수 있으며,
	음성 브라우저의 경우 form control이 label과 인접하지 않는 경우에도 인식할 수 있도록 지원한다.  

**웹 접근성을 고려한 select**

전송 버튼없이 자바스크립트의 onchange 이벤트를 사용한 select는 접근성을 고려하지 않은 방법이다.  
전송 버튼이 없는 경우 키보드 사용자나 자바스크립트를 사용할 수 없는 사용자를 고려하여 noscript 태그를 사용하면 되겠지.. 하겠지만, 그러한 방법은 반쪽짜리 접근성이다.  
전송 버튼을 생성하여 접근성을 지키는 방법을 습관화 하자.  
	
	<select>
		<option>웹 접근성을 고려한 select tag</option>
		<option>웹 접근성을 고려한 select tag</option>
		<option>웹 접근성을 고려한 select tag</option>
		<option>웹 접근성을 고려한 select tag</option>
	</select>
	<input type="submit">

##<a href="#" name="video">video</a>  
<a href="http://smilesol85.github.io/blabla/view/html/video.html">video</a>  
	
	<video preload controls autoplay loop poster="" width="300" height="150">
		<source src="#" type="video/mp4" />
		<source src="#" type="video/ogv" />
	</video>

속성 : preload, controls, autoplay, loop, poster, width, height  

> source 태그는 브라우저마다 지원하는 확장자 형식이 다르기 때문에 사용한다.  

모든 브라우저를 지원하지 않기 때문에 source 태그로 `mp4`, `ogv` 확장자 또는 `mp4`, `WebM` 확장 파일을 사용한다.  
모든 브라우저에서 사용 가능한 video.js 플러그인이 있다.  

<a href="http://videojs.com/">video.js 플러그인</a>

head 태그에 아래 2줄을 추가해야 한다.
	
	<!-- video 태그의 class 에는 class="video-js vjs-default-skin" data-setup="{}" 을 추가해 주면 된다. -->
	<link href="http://vjs.zencdn.net/c/video-js.css" rel="stylesheet">
	<script src="http://vjs.zencdn.net/c/video.js"></script>

##<a href="#" name="audio">audio</a>  
<a href="http://smilesol85.github.io/blabla/view/html/audio.html">audio</a>  
	
	<audio preload controls="controls" autoplay="autoplay" loop>
		<source src="#" type="audio/mp3" />
		<source src="#" type="audio/ogg" />
	</audio>

audio 태그의 속성중 controls 및 autoplay 등의 속성은 줄여서 `controls autoplay`와 같이 사용 가능하다.  
source 태그는 브라우저마다 지원하는 확장자 형식이 다르기 때문에 사용한다.  
보통 `mp3`와 `ogg` 확장자이면 거의 모든 브라우저는 지원 가능하다.  
	
	<source src="" type="audio/mp3" />
	<source src="" type="audio/ogg" />

타입은 생략 가능 하지만, 브라우저가 음악 파일을 내려받은 뒤 재생 가능한 파일인지 확인이 필요하므로 트래픽이 낭비된다.  
따라서 타입 속성을 사용하는 것이 좋다.  

> MP3 라이센스 때문에 5000번 이상 재생한 MP3 파일은 2500달러를 내야 한다고 한다.  

##<a href="#" name="track">track</a>  
<a href="http://smilesol85.github.io/blabla/view/html/track.html">track</a>  

> track 태그는 video 태그에 자막을 표시할 때 사용한다.

확장자는 .srt 로 저장 형식을 모든 파일로 선택 후 강제 지정해야 한다.  
	
	<video width="400" height="100" controls="controls"> 
		<source src="test.mp4" type="video/mp4" /> 
		<source src="test.webm" type="video/webm" /> 

		<track kind="subtitles" src="track.srt" srclang="ko" label="Korean" /> 
		<track kind="subtitles" src="track.srt" srclang="en" label="English" /> 
		<track kind="subtitles" src="track.srt" srclang="jp" label="Japanese" /> 
		<track kind="subtitles" src="track.srt" srclang="ch" label="Chinese" /> 
	</video>

**track.srt**
	
	1
	00:00:00,000 --> 00:00:03,000
	<h1>동영상 입니다.</h1>
	<p>자막 자막 자</p>

	2
	00:00:03,000 --> 00:00:10,000
	<p>자막 자막 자</p>

> 반드시 빈줄 다음에 다음 자막 파일을 만들어야 한다.  

현재 사용 가능한 브라우저는 없으며 <a href="http://videojs.com/">video.js plug-in</a>를 이용하면 된다.  

## <a href="#" name="page-break">page-break</a>  
인쇄시 강제로 다음 페이지로 넘길 수 있다.  
영역이 끝나면 페이지를 나눈다.  
`블록 요소에만 적용` 되며, 인라인 요소에는 적용되지 안된다.  
	
	<div style="page-break-after:always"></div> 
	<!--
	page-break-after:always;  // 항상 페이지 넘김
	page-break-after:auto;  // 기본값
	page-break-after:avoid;  // 페이지를 강제로 넘기지 못하게 한다.
	-->

## <a href="#" name="roll">roll</a>
- 표지판 역할을 한다고 볼 수 있겠다. (application, banner, main, navigation, search 등)  
- 문서에서 구조를 형성하는 요소에 부여한다. (section, navigation, note, heading 등)  
- 문서에서 어플리케이션 구조를 형성하는 요소에 부여한다. (alert, alertdialog, progressbar, status)  
- 사용자 인터페이스 역할을 한다. (treegrid, toolbar, menuitem 등)  
- 사용자 입력수신 역할을 한다. (checkbox, slider, option 등)  

**nav 태그 예로 들어보면 아래와 같다.**
	
	<nav role="navigation"></nav>

> nav 요소는 반드시 navigation 으로 작동 하지만, 스크린리더 중 일부는 인식하지 못하는 리더기가 있다.  

## <a href="#" name="webkit">webkit</a>  
<a href="https://developer.mozilla.org/en-US/docs/Web/CSS/-moz-appearance">-webkit 속성</a>
	
	/* webkit 기반의 브라우저에서 텍스트 사이즈가 들쑥날쑥 하지 않게 조절한다. */
	* {-webkit-text-size-adjust:none;}
	
	/* font size 조절 */
	-webkit-text-size-adjust:8px;
	
	/* 그림자 등이 깨끗이 사라진다. */
	-webkit-appearance:none;

## <a href="#" name="mobile_meta_link">mobile_meta_link</a>  
- 해상도를 고려한 레이아웃

	> 가로 길이를 가변폭(%)의 레이아웃으로 기획하고 개발 및 디자인 해야 한다. 모바일의 해상도가 다양하기 때문이다.

- 사용자를 편하게! 터치 오류를 줄여라

- 화면 확대비율 고정
			
		<meta name="viewport" content="width=디바이스-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0" />

	위와 같은 meta 태그는 화면 확대 비율을 기기 사이즈에 맞게 조정하는 부분이다.

	> initail-scale : 기본적인 확대 배율 결정. 0.5로 설정하면 원래 사이즈의 0.5배 크기로 보인다.  
	> maximum-scale : 최대 확대 배율을 결정한다.  
	> minimum-scale : 최소 확대 배율을 결정한다.  
	> user-scalable : 화면의 확대/축소 가능 여부를 결정한다. 0이면 불가능, 1이면 가능하다.  

	단, initial-scale값과 maximum-scale 값이 같다면, 최대 확대 배율이 100% 이므로 1로 설정해도 확대되지 않는다.  
	예를 들어 initial-scale=1.0, maximum-scale=2.0 으로 설정했다면 최대 2배까지 확대할 수 있다.

- 사이트 아이콘 제공
    iPhone에서는 웹 사이트 바로가기 아이콘을 홈화면에 넣울 수 있다.

	+ iPhone3g, iPhone3gs
			
			<link rel="apple-touch-icon-precomposed" media="screen and (resolution:163dpi)" href="이미지 경로" />
			<link rel="apple-touch-icon-precomposed" media="screen and (resolution:132dpi)" href="이미지 경로" />

	+ iPad
			
			<link rel="apple-touch-icon-precomposed" media="screen and (resolution:163dpi)" href="이미지 경로" />

	+ iPhone4
			
			<link rel="apple-touch-icon-precomposed" media="screen and (resolution:326dpi)" href="이미지 경로" />

- 자바스크립트 최소화  
jQuery는 훌륭한 자바스크립트 프레임워크이지만 모바일에서는 부담스러울 수 있다.  

- hover 이벤트는 모바일에서 소용이 없다.  
터치로 작동하는 디바이스에서는 hover 이벤트 사용은 무의미하다.  

- 레티나 디스플레이(Retina Display)  
레티나 디스플레이(Retina Display)를 위해서 30px x 30px image라면 2배 크기인 60px x 60px 로 작업을 해야한다.  

		
		.myImage {
		   width: 100px;
		   height: 40px;
		   -webkit-background-size: 100px 40px;
		   background: url("images/myImage.jpg");
		}

		@media screen and (-webkit-디바이스-pixel-ratio: 2) {
		   .myImage {
		     background: url("images/myImage@2x.jpg");
		   }
		}


- meta 태그, link 태그

			
		< link rel="apple-touch-icon" href="/apple-touch-icon.png"/ >
		< link rel="apple-touch-startup-image" href="/startup.png" >
		< meta name="apple-mobile-web-app-capable" content="yes" / >
		< meta name="apple-mobile-web-app-status-bar-style" content="black" / >


	+ link rel="apple-touch-icon" href="/apple-touch-icon.png"

		> 등록되는 문서의 아이콘을 지정할 수 있다.

		일반적으로 iPhone에서 문서 아이콘을 추가 하게되면 문서 화면을 캡쳐한 내용을 아이콘으로 사용하는데  
		apple-touch-icon이라는 link를 추가하여 내가 지정한 아이콘으로 사용할 수 있다.  
		favicon의 iPhone 버전이라고 생각하면 됩니다.

		+ iPhone : 57×57 png 이미지 사용
		+ iPad : 72×72 png 이미지 사용
		+ iPhone4 : 114×114 png 이미지 사용

		가능하면 114×114 이미지로 제작하여 사용하면 iPhone에서 자동으로 리사이즈 한다.

		기본적으로 iPhone이 제공하는 UI 처리된다.  
		(모서리를 둥글게 하고 반원형의 밝은 부분을 추가해 주는 것)  
		원하지 않을 때는 rel 속성의 값을 apple-touch-icon-precomposed 라는 이름으로 지정하여 사용하면 된다.
				
			<link rel="apple-touch-icon-precomposed" href="/apple-touch-icon-precomposed.png"/>

		> 이렇게 지정한 precomposed 아이콘 이미지는 android의 Add to Home Screen 기능에서도 지원된다.  
		> 사이즈는 48×48 입니다.


	+ link rel="apple-touch-startup-image" href="/startup.png"
		화면이 로딩될 때 startup 이미지를 지정할 수 있다.  
		웹 앱이지만 앱 처음 로딩시 로고화면 같이 노출할 수 있다.  
		iPhone 기본 앱에 들어있는 Default.png 와 비슷한 역할이다.  

		단, 이미지의 크기가 정확히 맞아야 한다.

		+ iPhone : 320×460
		+ iPhone4 : 640×920
		+ iPad : 768×1004


	+ meta name="apple-mobile-web-app-capable" content="yes"  
		웹 앱으로 선언하여 브라우저의 URL 바를 보이지 않게 할 수 있다.

		즉, 웹 앱이 마치 일반 네이티브 앱처럼 화면 전체(최상단 상태바 20px 제)를 활용할 수 있도록 한다.

	+ meta name="apple-mobile-web-app-status-bar-style" content="black"  
		상태바의 색상을 지정할수 있다.  
		바탕화면이 검정색인 앱의 경우 상태바만 회색인 이질감을 줄이기 위해 사용합니다.

		3가지 style : default (회색) , black , black-translucent ( 반투명 )

## <a href="#" name="css_optimization">CSS optimization</a>  
CSS란 `Cascading Style Sheets`의 약자이다.  
HTML 4.0 이후부터 style을 사용하므로써 HTML 문서와 디자인을 분리시키는 것이 가능해졌습니다.  
style이란 HTML 요소들이 어떻게 디스플레이 될 것인가에 대한 정의를 말합니다.  

style은 크게 4가지 방법으로 사용 가능합니다.  
우선 순위는 숫자가 높을 수록 높습니다.  

1. broser default  
1. External Style Sheet (head 태그안에 link 태그로 외부에서 link됩니다.)  
1. Internal Style Sheet(style이라는 태그를 써서 문서안에서 정의됩니다.)  
1. Inline Style (각 태그에 style=""이라는 속성을 이용해 정의됩니다.)  

CSS 최적화 방법(optimization manual)  

- inline, internal 보다 external stylesheet를 권장한다.  
	+ 유지보수가 좋을 뿐만 아니라, 브라우저에 캐시되어 추가적인 HTTP 요청이 발생하지 않는다.  

- 속도 향상을 위해서 `@import`는 지양한다.  
	+ 페이지 내에서 link 태그와 `@import`를 병행해서 사용하거나 여러 `@import`만을 사용할 경우  
	순차적으로 로딩하기 때문에 page speed에 영향을 미친다.  
	+ link 태그를 여러번 사용할 경우 병행 즉 동시 다운로드가 보장되어 속서면에서 좋다.  

- 모니터, 프린트, 소형기기를 위한 css를 분류한다.  
			
		<link type="text/css" rel="stylesheet" href="print.css" media="print">
		/* print.css */
		#header, #footer, .navWrap {display:none}

		
- !important 사용은 피하자! 렌더링 이슈가 발생할 수 있다.

- 이미지 표현을 위해 스프라이트 기법 사용을 사용하자.
	+ 정사각형의 스프라이트 이미지 사용시 속도면에서 더 빠르다는 것을 알 수 있다.
	+ 이미지 태그에서 src 경로는 display:none 이지만 request를 발생한다.  
	CSS background-image로 지정되고 display:none을 지정하면 request를 발생하지 않는다.  
	단, inline style로 적용될 경우 FF를 제외한 browser에서 request를 발생한다.

- 숫자 0 이외의 숫자에는 단위 붙이자.

- 색 지정에는 RGB 값 사용 권장한다.

- 전체 사이즈 및 폰트 사이즈에서는 em 사용, 절대 사이즈에는 px 사용, 상대 사이즈에는 % 사용하자.

- css 속성은 가능하면 축약형 사용하자.
			
		padding:5px 0 2px 0;
	
- 최소한의 id 와 class를 사용하자.

## <a href="#" name="selector">selector</a>  
<a href="http://smilesol85.github.io/blabla/view/html/selector.html">selector</a>  
	
	* : 전체 선택자  
	tag : tag 선택자  
	#id : 아이디 선택자  
	.class : 클래스 선택자  
	ul li : 후손 선택자  
	ul > li : 자손 선택자  
	span + span : 동위 선택자  
	span ~ em : 동위 선택자  
	:active : 반응 선택자  
	:hover : 반응 선택자  
	:checked : 상태 선택자  
	:focus : focus 선택자  
	[type=text]:enabled : enabled 선택자  
	[type=text]:disabled : disabled 선택자  
	:not(.not) : 부정 선택자  

## <a href="#" name="selector-before-after-data">selector-before-after-data</a>
<a href="http://smilesol85.github.io/blabla/view/html/selector-before-after-data.html">selector-before-after-data</a>  

**counter가 가능하다.**  
	
	<style>
	p{counter-increment:nSmilesol;}
	p::before{content:counter(nSmilesol)'. ';}
	p::after{content:' -' attr(data-page) "page";}

	span::before{content:'Before section';color:red;}
	span::after{content:'After section';color:blue;}
	p{counter-increment:nSmilesol;}
	p::before{content:counter(nSmilesol)'. ';}
	p::after{content:' -' attr(data-page) "page";}
	</style>

	<span>view style</span>
	<p data-page="100">texttexttexttexttexttexttexttexttexttexttexttexttext</p>
	<p data-page="200">countercountercountercounter</p>

웹 표준에 준수하기 위해서는 태그에 지정된 속성 이외에는 사용할 수 없다. 하지만 `data-를 사용하면 사용자 지정 속성`으로 인정해 준다.  

## <a href="#" name="selector-child">selector-child</a>  
<a href="http://smilesol85.github.io/blabla/view/html/selector-child.html">selector-child page</a>  
	
	.first-child li:first-child{color:red;} /* 첫 번째 자식 요소 선택 */
	li:first-of-type{color:red;} /* li 요소 중 첫번째 li 선택 */
	.first-child li:last-child{color:blue;} /* 마지막 자식 요소 선택 */
	li:last-of-type{color:blue;} /* li 요소 중 마지막 li 선택 */

	/* n번째 선택 */
	.first-child li:nth-child(3),.first-child li:nth-last-child(3){color:orange;}
	li:nth-of-type(3),li:nth-last-of-type(3){color:orange;}

## <a href="#" name="selector-string">selector-string</a>
<a href="http://smilesol85.github.io/blabla/view/html/selector-string.html">selector-string page</a>  
	
	/* 첫 번째 문자 선택 */
	.sFl::first-letter{color:red;}

	/* 첫 번째 라인 선택 */
	.sFln::first-line{color:red;}

	/* selection 선택자 */
	.dh::selection{color:red;}

	/* 선택자[속성~=값] - 속성 안의 값이 특정 값을 단어로 포함하고 있는 것 선택 */
	.strSlt-a[data-role~=ab]{color:red;}

	/* 선택자[속성|=값] - 속성 안의 값이 특정 값을 단어로 포함하고 있는 것 선택 */
	.strSlt-b[data-role|=ko]{color:red;}

	/* 선택자[속성*=값] - 속성 안의 값이 특정 값을 포함하고 있는 것 선택 */
	.strSlt-b2[data-role*=x]{color:red;}

	/* 선택자[속성^=값] - 속성 안의 값이 특정 값으로 시작하는 태그를 선택 */
	.strSlt-c[data-role^=a]{color:red;}

	/* 선택자[속성$=값] - 속성 안의 값이 특정 값으로 끝나는 태그를 선택 */
	.strSlt-d[data-role$=f]{color:red;}
    
## <a href="#" name="css_unit">CSS unit</a>  
많은 사람들이 em단위를 쓰면 해상도에 따라서 크기가 달라진다고 오해하는 경우가 많다.  

em을 쓰는 이유는 IE6과 같이 zoom 기능이 없는 browser에서  
브라우저의 폰트 사이즈 옵션을 조절했을 때 동작하게 하기 위함이다.  

최근의 브라우저들이 모두 zoom 기능을 지원하고 있어 em대신 px을 사용해도 상관 없다.    
하지만 반응형 웹 디자인을 추구하는 작업을 하시거나,  
화면 크기에 따라서 동적으로 body의 font-size를 조절하는 특수한 작업을 하실 경우에는  
em을 활용하여 scaleable한 UI를 구성할 수도 있습니다.  
또한 해외 웹사이트의 대부분이 em 을 사용하며, 유동성 부분 때문에 em이 표준으로 자리잡아가고 있습니다.  

**편리한 작업을 위한 CSS 단위별 폰트크기(px, em, %, pt)**  

| Pixels      | EMs         | Percent | Points |
|:-----------:|:-----------:|:-------:|:------:|
| 6px         | 0.375em     | 37.5%   | 5pt    |
| 7px         | 0.438em     | 43.8%   | 5pt    |
| 8px         | 0.5em       | 50%     | 6pt    |
| 9px         | 0.563em     | 56.3%   | 7pt    |
| 10px        | 0.625em     | 62.5%   | 8pt    |
| 11px        | 0.688em     | 68.8%   | 8pt    |
| 12px        | 0.75em      | 75%     | 9pt    |
| 13px        | 0.813em     | 81.3%   | 10pt   |
| 14px        | 0.875em     | 87.5%   | 11pt   |
| 15px        | 0.938em     | 93.8%   | 11pt   |
| 16px        | 1em         | 100%    | 12pt   |
| 17px        | 1.063em     | 106.3%  | 13pt   |
| 18px        | 1.125em     | 112.5%  | 14pt   |
| 19px        | 1.188em     | 118.8%  | 14pt   |
| 20px        | 1.25em      | 125%    | 15pt   |
| 21px        | 1.313em     | 131.3%  | 16pt   |
| 22px        | 1.375em     | 137.5%  | 17pt   |
| 23px        | 1.438em     | 143.8%  | 17pt   |
| 24px        | 1.5em       | 150%    | 18pt   |

**단위별 폰트의 특징**  

- pt : 포인트(points) - 1포인트는 0.72인치  
- px : 픽셀(pixels) - 화면 해상도에 대한 상대크기  
- %, em : 지정되거나 상속받은 (또는 상위 엘리먼트)에 대한 백분율 상대 크기  

**em 사용 예**

em은 부모의 요소에 영향을 받아 매번 계산해 보고 눈으로 확인해 봐야 하는 단점이 있다.  
	
	body { font-size:62.5%; }
	h1 { font-size: 2.4em; } /* =24px */
	p  { font-size: 1.4em; } /* =14px */
	li { font-size: 1.4em; } /* =14px */

**rem 사용 예**  

em의 단점인 부모 요소의 영향을 받는 단점을 보안하기 위해서  
CSS3에서 갠찮은 단위를 소개 했는데 그 중 rem(root em) 단위는 꽤 유용하게 쓰일 것 같다.  
rem 단위는 대부분의 브라우저를 지원하나 아직 전부 지원하지는 않는다.  
rem 지원 여부 : http://caniuse.com/#search=rem  
모드 브라우저 대응을 위해 아래와 같이 활용할 수 있겠다.

아래 코드는 부모인 p 태그에 1.4rem이 선언되어 있고,  
자식 요소인 span 태그에 부모에 종속되지 않은 1.2rem을 선언할 수 있다.
	
	p { font-size: 1.4rem; } p span { font-size: 1.2rem; }

## <a href="#" name="background">background</a>  
	
	/* 배경색 지정 */
	div{background-color:#ffffff}
	
	/* 배경에 image 삽입 */
	div{background-image:url('이미지경로')}
	
	/* 배경 반복 설정 no-repeat , repeat-x , repeat-y */
	div{background-repeat:no-repeat}
	
	/* scroll : 스크롤하도록 지정 , fixed : 고정되도록 지정 , inherit : 부모 요소의 값 상속하도록 지정 */
	div{background-attachment:scroll}
	
	/* left , right , center , top , bottom , 100px */
	div{background-position:10px 10px}
	
	/* 하나로 사용할 때 */
	div{background:#fff url('../images/test.jpg') no-repeat 0 150px}
	
	/* background 여러개 사용 */
	div{background:url(), linear-gradient(), url()}
	div{background-repeat:no-repeat, no-repeat, repeat}
	div{background-position:bottom right, left, right}

## <a href="#" name="CSS_link">CSS_link</a>  
link style 선언 순서 (LoVe HAte)
	
	a:link{color:blue}
	a:visited{color:red}
	a:hover{color:green}
	a:active{color:yellow}

## <a href="#" name="opacity">opacity</a>  

**background:#000; opacity:없음**
	
	<!-- background:#000; opacity:없음 -->
	<div style="background:#000; color:#fff;">
	background:#000; opacity:없음
	</div>

**(for all browsers) background:#000; opacity:0.5;**
	
	<!-- (for all browsers) background:#000; opacity:0.5; -->
	<div style="background:#000; color:#fff; opacity:0.5;">
	(for all other browsers) background:#000; opacity:0.5;
	</div>

**(for IE5~7) background:#000; filter:alpha(opacity:50);**
	
	<!-- (for IE5~7) background:#000; filter:alpha(opacity:50); -->
	<div style="background:#000; color:#fff; filter:alpha(opacity:50);">
	(for IE5~7) background:#000;  filter:alpha(opacity:50);
	</div>

**(for IE8) background:#000; -ms-filter:alpha(opacity:50);**
	
	<!-- (for IE8) background:#000; -ms-filter:alpha(opacity:50); -->
	<div style="background:#000; color:#fff; -ms-filter:alpha(opacity:50);">
	(for IE8) background:#000;  -ms-filter:alpha(opacity:50);
	</div>

**(for all IE version) background:#000; -ms-filter:alpha(opacity:50); filter:alpha(opacity:50);**
	
	<!-- (for all IE version) background:#000; -ms-filter:alpha(opacity:50); filter:alpha(opacity:50); -->
	<div style="background:#000; color:#fff; -ms-filter:alpha(opacity:50); filter:alpha(opacity:50);">
	(for all IE version) background:#000;  -ms-filter:alpha(opacity:50); filter:alpha(opacity:50);
	</div>

**background:#000; opacity:0.5; -ms-opacity:0.5; -ms-filter:alpha(opacity:50); filter:alpha(opacity:50);**
	
	<!-- background:#000; opacity:0.5; -ms-opacity:0.5; -ms-filter:alpha(opacity:50); filter:alpha(opacity:50); -->
	<div style="background:#000; color:#fff; opacity:0.5; -ms-opacity:0.5; -ms-filter:alpha(opacity:50); filter:alpha(opacity:50);">
	background:#000;  opacity:0.5; -ms-opacity:0.5; -ms-filter:alpha(opacity:50); filter:alpha(opacity:50);
	</div>

## <a href="#" name="web_font">web_font</a>  
웹 브라우저는 사용자의 컴퓨터에 설치된 폰트만 사용할 수 있다.  
개발할 당시의 컴퓨터에는 폰트가 설치되어 있지만,  
사용자의 컴퓨터에 설치되어 있지 않은 폰트를 사용하고 싶은 경우 웹 폰트를 사용한다.  

웹 폰트는 사용자가 웹 페이지에 접속하는 순간 폰트를 자동으로 내려 받는다.  

<a href="http://www.google.com/webfonts">google web font - free</a>  

> IE9 버전에서는 서버에서 실행할 경우 웹 폰트가 적용되며,  
> 로컬에서 실행할 경우 보안 문제 때문에 웹 폰트가 적용되지 않는다.
	
	@font-face {
	font-family:NanumGothic;  /* font name 마음대로 지정 */
	src:local('NanumGothic'),  /* 사용자 컴퓨터에 있는 폰트 사용 */
	     url('NanumGothic.eof'),  /* web font down */
	     url('NanumGothic.ttf'),
	     url('NanumGothic.woff');
	} 
	/* 위에서 생성한 font 사용 */
	*{font-family:’<strong>NanumGothic</strong>’;}

**각 포멧별 사용 가능한 브라우저**

- .eof : ie만 지원
- .ttf / .otf : ie 를 제외한 브라우저 지원
- .svg : opera만 지원
- .woff : ie, chorme, firefox만 지원

> 따라서 .eof 와 .ttf 포맷을 사용하면 모든 브라우저를 지원한다.  

## <a href="#" name="scrollbar">scrollbar</a>
	
	<!-- ie 적용 -->
	html {
	scrollbar-face :움직이는 바 전체색
	scrollbar-shadow :바의 오른쪽과 밑쪽 그림자색
	scrollbar-highlight :바의 왼쪽과 위쪽의 얇은 선색
	scrollbar-3dlight :바의 왼쪽위쪽에 진하게 드러가는 선:
	scrollbar-darkshadow :바의 오른쪽과 밑쪽에 들어가는 얇은 색
	scrollbar-track :바가 없는 아래부분의 색
	scrollbar-arrow :위 아래 화살표 색
	}

	<!-- webkit 적용 -->
	*{overflow-y:scroll;-webkit-overflow-scrolling:touch}
	*::-webkit-scrollbar {width:8px;height:8px;border:3px solid #fff}
	*::-webkit-scrollbar-button:start:decrement, ::-webkit-scrollbar-button:end:increment {display:block;height:10px;background:url('./images/bg.png') #efefef}
	*::-webkit-scrollbar-track {background:#efefef;-webkit-border-radius:10px;border-radius:10px;-webkit-box-shadow:inset 0 0 4px rgba(0,0,0,.2)}
	*::-webkit-scrollbar-thumb {height:50px;width:50px;background:rgba(0,0,0,.2);-webkit-border-radius:8px;border-radius:8px;-webkit-box-shadow:inset 0 0 4px rgba(0,0,0,.1)}

## <a href="#" name="firefox_button">firefox_button</a>  
button 태그에 디자인 요소를 추가하기 위해서  
padding, background, border 등을 재정의 하는 경우가 있다.  
그러나 firefox에서는 padding 값과 border 값이 적용되지 않고 여백이 발생한다.  
firefox가 버튼 내부에 focus가 갔을때 사용하기 위한 내부 여백이라고 한다.  

firefox에서도 padding, border가 style 적용한 값으로 노출하고자 할때는  
`::-moz-focus-inner` 라는 선택자를 사용한다.  

    
    {% highlight css %}
	button{padding:0;border:0;background:none}
	button::-moz-focus-inner{padding:0;border:0}
    {% endhighlight %}


## <a href="#" name="media_query">media_query</a>  
@media는하나의 CSS에서 분기처리하여 다양한 장치에서 문서가 출력될 수 있도록 정의할 수 있다.  

**방법1. link 태그 사용**
	
	<link rel="stylesheet" href="screen.css" media="screen">
	<link rel="stylesheet" href="print.css" media="print">

각각 지정한 미디어 장치에 따라 style이 적용된다.  

**방법2. CSS내에서 사용**
	
	<style>
	@media screen{}
	</style>

> @media only all and (조건문) {실행문}  
- @media : 미디어쿼리 시작 선언  
- only : 생략 가능하며, 생략시 기본값은 only 이다.  
- all : all, aural, braille, embossed, handheld, print, projection, screen, speech, tty, tv 의 미디어 타입을 선택할 수 있다.  
- and : 앞과 뒤의 조건을 만족해야 한다. / or : 앞과 뒤중 하나만 만족하면 된다.  
	
	/* 0 ~ 500px */
	@media screen and (max-width:500px){
	h1{color:red}
	}
	
	/* 500px ~ 800px */
	@media screen and (min-width:500px) and (max-width:800px){
	h1{color:yellow}
	}
	
	/* 800px ~ */
	@media screen and (min-width:800px){
	color:green
	}
	
	/* 세로모드 */
	@media screen and (orientation:portrait){
	color:pink
	}
	
	/* 가로모드 */
	@media screen and (orientation:landscape){
	color:orange
	}
	
	/* 레티나 디스플레이 */
	@media screen and (-webkit-min-디바이스-pixel-ratio:2){
	color:blue
	}
    
## <a href="#" name="transition">transition</a>
<a href="http://smilesol85.github.io/blabla/view/html/transition.html">transition</a>  

현재(2013.02.27) transition 속성은 벤더프리픽스를 사용한다.

- transition-duration : 재생할 시간 지정  
- transition-delay : 지정 시간 후 재생  
- transition-property : 변경할 속성 지정  
- transition-timing-function : 수치 변형 함수 지정  
- (수치 변형 함수 : ease, ease-in, ease-out, ease-in-out 기타 등등)  

## <a href="#" name="transform">transform</a>  
<a href="http://smilesol85.github.io/blabla/view/html/transform.html">transform</a>  

HTML5에서 3차원을 구현하는 방법에는 크게 2가지가 있다.
- 자바스크립트를 사용한 WebGL  
- CSS3를 사용한 3차원 변환  

대표적인 CSS3 변환을 사용하는 자바스크립트 플러그인중 HTML을 활용하여 ppt를 만들 수 있는 <a href="http://bartaz.github.io/impress.js/">Impress.js</a>가 있다.  
현재(2013/02/29) transform속성도 transition속성과 animation속성과 같이 벤더프리픽스를 사용해야 한다.  

transform 속성은 아래와 같다.  
- translate(X,Y) : 특정 크기 이동  
- translateX(X) : X축으로 특정 크기 이동  
- translateY(Y) : Y축으로 특정 크기 이동  
- scale(X,Y) : 특정 크기 확대 및 축소  
- scaleX(X) : X축으로 특정 크기 확대 및 축소  
- scaleX(Y) : Y축으로 특정 크기 확대 및 축소  
- skew(X,Y) : 특정 각도로 기울임  
- skewX(X) : X축으로 특정 각도 기울임  
- skewY(Y) : Y축으로 특정 각도 기울임  
- rotate(Z) : 특정 각도 회전  

3차원 변환 함수에서는 Z값만 추가해 주면 된다.  
- translate3d(X,Y,Z);  
- scale3d(X,Y,Z);  
- rotate3d(X,Y,Z);  

변환 함수 선언 순서에 따라 결과가 달라질 수 있으니 주의해야 한다.  
결과는 선언한 순서에 따라 적용된다.  

transform-origin속성은 rotate함수 적용시 회전의 중심점을 설정할 수 있다.  
    
> transform-origin:100% 100%;  
> transform-origin:right bottom;  

transform-style 속성은 3차원 속성 회전할 때 후손의 3차원 속성을 무시할지,유지할지 선택할 수 있다.  
    
> transform-style:flat : 후손의 3차원 속성을 무시한다.  
> transform-style:preserve-3d : 후손의 3차원 속성을 유지한다.  

backface-visibility 속성은 3차원에서 후면을 보이게 하거나, 보이지 않게 설정 가능하다.  
    
> backface-visibility:hidden : 후면을 보이지 않게  
> backface-visibility:visible : 후면을 보이게  

## <a href="#" name="animation">animation</a>  
<a href="http://smilesol85.github.io/blabla/view/html/animation.html">animation page</a>  

<a href="http://animateyourhtml5.appspot.com/pres/index.html?lang=en#1">HTML5 animation</a>  

animation속성은 transition속성과 비슷하다.  
차이점은 keyframe을 활용할 수 있다는 점이다.  

animation 속성은 아래와 같다.  
- animation-delay : 지정 시간 후 재생  
- animation-direction : 애니메이션 진행 방향 설정 (alternate, normal)  
- animation-duration : 지정 시간동안 재생  
- animation-iteration-count : 반복 횟수 지정 (infinite, 1, 2, 3)  
- animation-name : 애니메이션 이름 지정, `@keyframes`활용  
- animation-play-state : 애니메이션 재생 상태 지정 (paused, running)  
- animation-timing-function : 수치 변형 함수 지정  
    
		    
			
		/* create keyframe */
		@-webkit-keyframes ani{
		from{left:0;-webkit-transform:rotate(0deg);}
		50%{left:500px;}
		to{left:500px;-webkit-transform:rotate(360deg);}
		}
		
		@keyframes ani{
			from{left:0;transform:rotate(0deg);}
			50%{left:500px;}
			to{left:500px;transform:rotate(360deg);}
		}
		
		div{
			-webkit-animation-name:ani;
			-webkit-animation-duration:2s;
			-webkit-animation-timing-function:linear;
			animation-name:ani;
			animation-duration:2s;
			animation-timing-function:linear;
			
			/* 한 방향 */
			-webkit-animation-iteration-count:infinite;
			animation-iteration-count:infinite;
		}
		
		div{
			-webkit-animation-name:ani;
			-webkit-animation-duration:2s;
			-webkit-animation-timing-function:linear;
			animation-name:ani;
			animation-duration:2s;
			animation-timing-function:linear;
			
			/* 처음으로 되돌아 감 */
			-webkit-animation-iteration-count:infinite;
			-webkit-animation-direction:alternate; /* normal 은 from 에서 to */
			animation-iteration-count:infinite;
			animation-direction:alternate; /* normal from 에서 to */
		}
		
		div:hover{
			-webkit-animation-name:ani;
			-webkit-animation-duration:2s;
			-webkit-animation-timing-function:linear;
			animation-name:ani;
			animation-duration:2s;
			animation-timing-function:linear;
			
			-webkit-animation-play-state:paused; /* running */
			animation-play-state:paused; /* running */
		}
    

**animation 속성 한 줄로 입력하기**  
> animation:|animation-name|animation-duration|animation-timing-function|animation-delay|animation-iteration-count|animation-play-state  