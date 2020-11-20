# html2
html code practice
<div 태그 한행을 독차지>
 
target = "_blank" 새로운 화면이 새롭게 하나더 열린다. 팝업된다. 
target = "_self" 내 화면에서 새로운 페이지 열림 
 
 
1.한행을 다 독차지하는 태그 다 불러봐,
h1~h6
p태그
hr태그
 
 
1. 샘 과제 도서프로그램 코딩 태그
2. 교재 복습 
3. 코딩 다시 치기
 
valign
 
td 
th 차이
tr 차이
 
ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
Chap. 4   DIV 태그

 
1. div 태그

> 이미지, 문자열 등을 기준별로 그룹화 시켜 서로 [겹치게 포개 놓기], [펼쳐 놓기], [감춰놓기] 등을 할 수 있는 태그이다.
> <div>~</div> 영역은 block 형식(=한 행을 차지함= 아래로 쌓인다)
> <div> 태그의 속성은 CSS의 표현방식인 style 속성으로 표현한다.
     > < div style = " 속성1 : 속성값1 ; ~ ; " >
     
ex)
<div style="background-color : lightblue; width: 100;height: 50; padding: 5 ; 
                   position: absolute ; top : 50 ; left: 50 ; z-index: 5 ; visibility: visible; ">
[급보]<br>강정호 만루 홈런!<br>오늘만 5타점 기록!
</div>
 
> 한 행을 독차지하는 태그는 div 다음 컨텐츠는 아래로 내려간다.
   이걸 블럭(block)형식이라고 한다.(마치 블럭쌓는 것처럼)
> 인라인(inline) 형식은 왼쪽에서 오른쪽으로 쌓이는 형식이다.
 
 
2. div 태그 속성

 
(1) < div style = " position : 위치 ; " >

> div 태그의 위치를 지정한다.
> 위치의 종류 
         1) static 
               > div 태그의 현재 코딩 위치서만 존재함.
              > <주의> 이동성이 없기 때문에 top, left, z-index 속성은 사용해도 효과가 없다.
 
          2) relative
              > div 태그 현재 코딩 위치를 0,0으로 기준삼고
                  top, left 속성 사용에 따라 div 태그를 위치시킨다.
                  z-index 속성을 사용하면 기존 컨텐츠 위에 위치할 수 있다.
 
         3) absolute
              > 화면 왼쪽 상단 모서리를 0,0 으로 기준 삼고
                  top, left 속성에 따라 div 태그를 위치시킨다.
                  z-index 속성을 사용하려면 기존 컨텐츠 위에 위치할 수 있다.
 
 
(2) < div style = " left : 화면 왼쪽 여백 ; " >     

     > 웹브라우저 왼쪽 테두리에서 div 태그 영역(div 태그)까지의 가로 위치를 나타냄
 
(3) < div style = " top : 화면 상단 여백 ; " > 

     > 웹브라우저 상단 테두리에서 div 태그 영역(div 태그)까지의 세로 위치를 나타냄

(4) < div style = " padding : 상여백 우여백 하여백 좌여백 ; " >

     > div 태그 영역 내부의 상,우,하,좌 여백 지정
     > padding : 값; 일 경우 상,우,하,좌 여백 모두 동일 지정.
     > padding-top; padding-right; padding-bottom; padding-left;
 
(5) <div style = " width : div 태그 영역 넓이 ; " >

     > div 태그 영역 넓이를 지정
     > <주의> div 태그 내부에 출력물이 전혀 없을 경우 width 옵션이 안 먹힌다.
     > 즉 넓이가 없다. &nbsp; 라도 주어야 width 옵션이 먹힌다.
     > <div></div> 높이 넓이 없음. 
     > <div>&nbsp;</div>  높이 넓이 있음.
 
 
(6) <div style = " height : div 태그 영역 높이 ; " >

     > div 태그 영역 높이를 지정
     > <주의> div 태그 내부에 출력물이 전혀 없을 경우 height 옵션은 안 먹힌다.
     > 즉 높이가 없다. &nbsp; 라도 주어야 width 옵션이 먹힌다.
     > <div></div> 높이 넓이 없음. 
     > <div>&nbsp;</div>  높이 넓이 있음.
 
(7) < div style = "border : 테두리선 두께 선모양 색상; " >

     > div 태그 영역의 테두리선두께, 선모양, 색상 설정.
     > 예) <div style = "border : 2px solid red;">
 
(8) < div style = " background-color : div 태그 영역 생상; " >

     > div 태그 영역 색상을 지정.
 
 
(9) < div style = " background-image : url('이미지파일명') ; " >

 
     > div 태그 영역 배경 이미지를 지정
 
(10) < div style = " z - index : 우선 순위 번호 ; " > 

 
     > div 태그 영역이 겹쳤을 때 우선순위를 지정. 번호가 클수록 상위.
 
(11) < div style = " visibility : 보임 여부 설정 ; " >

 
     > div 태그 영역 보임 여부를 설정.
     > 보임 여부 설정값은 visible(보임), hidden(안보임)
     > <주의>none 설정 시 안보이고 차지하는 공간은 남아있음.
 
(12) < div style = " display : 보임 여부 설정 ; " >

     > div 태그 영역 보임 여부를 설정.
     > 보임 여부 설정값은 block(보임), none(안보임)
     > <주의> none 설정 시 안보이고 차지하는 공간도 없음.
 
(13) < div style = " overflow : 스크롤바 설정; " >

     > [div 태그 영역 내용물 크기 > div 태그 영역 크기] 클 경우 스크롤 바의 보임 여부를 설정
     > auto : 내용이 지정 크기 보다 크면 자동 보임.
     > hidden : 내용 지정 크기 보다 크면 자동 보임.
     > scroll : 내용 크기 관계없이 스크롤바 보임.
     > visible : 정해진 크기 관계없이 스크롤바 보임.
 
(14) < div style = " filter : Alpha(Opacity = 투명 수치) " >

 
     > JQuary 에서 다룰 예정
 

Chap. 5

TABLE  태그

 
1. TABLE 태그

> 문자열 또는 이미지를 [행]과 [열]로 표시하는 태그이다.
> 웹화면의 구성 요소를 원하는 형태로 배치할 때, DB에서 데이터를 가져와 출력할 때 많이 사용한다.
 
2. TABLE 태그 형식
 
[태그 소스]ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
 
<table>
          <caption> 표제목 </caption>
          <thead>
                    <tr>
                              <th>헤더1</th>
                              <th>헤더2</th>
                              <th>헤더n</th>
                    </tr>
          </thead>
          <tbody>
                     <tr>
                            <td> 데이터11</td>
                            <td> 데이터12</td>
                            <td> 데이터1n</td>
                     </tr>
                     <tr>
                            <td> 데이터21</td>
                            <td> 데이터22</td>
                            <td> 데이터2n</td>
                     </tr>
                     <tr>
                            <td> 데이터m1</td>
                            <td> 데이터m2</td>
                            <td> 데이터mn</td>
                     </tr>
          </tbody>
</table>
ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
> <caption> 태그는 생략 가능하다. (cap 모자= 표제목)
> <tr>은 한 행을 지배한다. (table row)
> <th><td>는 한 셀을 지배한다. (table header) (tablebo dy)
> <tr>의 개수가 전체 행의 개수이다.
> <th> 태그 안의 문자는 자동으로 중앙으로 배치되고 글자가 두꺼워진다. (table header)
> <td> 태그 안의 문자는 자동으로 왼쪽으로 배치되고 글자는 얇다. (tablebo dy)
> <thead>,<tbody>는 생략이 가능하다. 그러나 jQuery에서 테이블을 컨트롤 할 때는 유용하게 사용된다.
> </td> </th> </tr> 은 생략 가능하나 영역을 나타내므로 되도록 쓴다. 
 
 
 
 
 
 
 
 
 
 
 
