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
 
 
 <!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>테이블 테그</title>

		<style>
			/*선택자(selector)(=>태그를 지칭하는 방법) */
			.xxx , .xxx th , .xxx td{
				/*.xxx th <--th와 xxx사이의 공백은 후손이라는뜻 th갖고있는애 있니.*/
				/*.xxx는 
				class="xxx"라는 이름이 있는 곳에 이 style을 입히겠다는 뜻.*/
				border-collapse: collapse;
				/*경계선에 입체감 주지마*/

				border: 1px solid #A2A2A2;
				/*경계선의 두께는 1로 하고

				경계선의 선 모양은 직선
				경계선의 색상은 회색으로 했으면좋겠어*/
				padding:5;

				font-size: 9pt;
				/*rm*/
				font-family: tahoma,굴림,돋움,verdana;
			}
				.yyy , .yyy th , .yyy td{
				/*.xxx th <--th와 xxx사이의 공백은 후손이라는뜻 th갖고있는애 있니.*/
				border-collapse: collapse;
				/*경계선에 입체감 주지마*/

				border: 1px solid #000000;
				/*경계선의 두께는 1로 하고

				경계선의 선 모양은 직선
				경계선의 색상은 회색으로 했으면좋겠어*/
				padding:5;

				font-size: 9pt;
				/*rm*/
				font-family: tahoma,굴림,돋움,verdana;
			}
				#zzz , .#zzz th , #zzz td{
				/*#zzz 는 id=zzz를 가진놈이다.*/
				border-collapse: collapse;
				/*경계선에 입체감 주지마*/

				border: 1px solid red;
				/*경계선의 두께는 1로 하고

				경계선의 선 모양은 직선
				경계선의 색상은 회색으로 했으면좋겠어*/
				padding:5;

				font-size: 9pt;
				/*rm*/
				font-family: tahoma,굴림,돋움,verdana;
			}



		</style>


	</head>
		<body><!-- <center> -->
			

			<table class = "xxx" align="center">
				<caption align="top">성적표</caption>

				<!-- 행을 지배하는 태그 <tr></tr> -->
				<tr bgcolor="#CBCBCB">
					<!-- 열을 지배하는 태그 <td></td> 
						두꺼워지지 않고 각셀의 왼쪽 정렬-->
					<!-- 열을 지배하는 태그 <th></th> 
						두꺼워지고,각셀의 중앙으로 정렬-->

					<th width="100">이름</th>
					<th width="80">국어</th>
					<th width="80">영어</th>
				</tr>
				<tr align="center">
					<th>사오정</th>
					<th>70</th>
					<th>70</th>
				</tr>
				<tr align="center">

					<th>저팔계</th>
					<th>98</th>
					<th>100</th>
				</tr>
				<tr align="center">

					<th>손오공</th>
					<th>95</th>
					<th>100</th>
				</tr>



			</table>

			<hr>

			<table class = "yyy">
				<caption align="top">성적표</caption>

				<!-- 행을 지배하는 태그 <tr></tr> -->
				<tr bgcolor="#CBCBCB">
					<!-- 열을 지배하는 태그 <td></td> 
						두꺼워지지 않고 각셀의 왼쪽 정렬-->
					<!-- 열을 지배하는 태그 <th></th> 
						두꺼워지고,각셀의 중앙으로 정렬-->

					<th width="100">이름</th>
					<th width="80">국어</th>
					<th width="80">영어</th>
				</tr>
				<tr align="center">
					<th>사오정</th>
					<th colspan=2>70</th>
					<!-- colspan=2 : 양옆을 합친다. -->
					<!-- <th>70</th> -->
				</tr>
				<tr align="center">

					<th>저팔계</th>
					<th>98</th>
					<th>100</th>
				</tr>
				<tr align="center">

					<th>손오공</th>
					<th>95</th>
					<th>100</th>
				</tr>



			</table>
			<hr>

			<table id="zzz">
				<caption align="top">성적표</caption>

				<!-- 행을 지배하는 태그 <tr></tr> -->
				<tr bgcolor="#CBCBCB">
					<!-- 열을 지배하는 태그 <td></td> 
						두꺼워지지 않고 각셀의 왼쪽 정렬-->
					<!-- 열을 지배하는 태그 <th></th> 
						두꺼워지고,각셀의 중앙으로 정렬-->

					<th width="100">이름</th>
					<th width="80">국어</th>
					<th width="80">영어</th>
				</tr>
				<tr align="center">
					<th>사오정</th>
					<th>70</th>
					<th>70</th>
				</tr>
				<tr align="center">

					<th>저팔계</th>
					<th>98</th>
					<th rowspan="2">100</th>
					<!-- 위아래 셀을 합친다 -->
					<!-- 먼저 코딩 되는걸 rowspan -->
					<!-- 뒤에 코딩 되는걸 주석처리 -->
				</tr>
				<tr align="center">

					<th>손오공</th>
					<th>95</th>
					<!-- <th>100</th> -->
				</tr>

			</table>
			<hr>

			<table>
				<caption align="top">성적표</caption>

				<!-- 행을 지배하는 태그 <tr></tr> -->
				<tr bgcolor="#CBCBCB">
					<!-- 열을 지배하는 태그 <td></td> 
						두꺼워지지 않고 각셀의 왼쪽 정렬-->
					<!-- 열을 지배하는 태그 <th></th> 
						두꺼워지고,각셀의 중앙으로 정렬-->

					<th width="100">이름</th><!--1행1열-->
					<th width="80">국어</th><!--1행2열-->
					<th width="80">영어</th><!--1행3열-->
				</tr>
				<tr align="center">
					<th>사오정</th> 						<!--2행1열-->
					<th colspan="2" rowspan="3">70</th> <!--2행2열-->
					<!-- <th>70</th> --> 				<!--2행3열-->
				</tr>
				<tr align="center">

					<th>저팔계</th>						<!--3행1열-->
					<!-- <th>98</th>-->        			<!--3행2열-->
					<!--<th>100</th> -->				<!--3행3열-->
				</tr>
				<tr align="center">

					<th>손오공</th>						<!--4행1열-->
					<!--<th>95</th>-->					<!--4행2열-->
					<!--<th>100</th> -->				<!--4행3열-->
				</tr>



			</table>



		</body>
</html>
 
 <!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>테이블 테그</title>

		<style>
			/*선택자(selector)(=>태그를 지칭하는 방법) */
			.xxx , .xxx th , .xxx td{
				/*.xxx th <--th와 xxx사이의 공백은 후손이라는뜻 th갖고있는애 있니.*/
				/*.xxx는 
				class="xxx"라는 이름이 있는 곳에 이 style을 입히겠다는 뜻.*/
				border-collapse: collapse;
				/*경계선에 입체감 주지마*/

				border: 1px solid #A2A2A2;
				/*경계선의 두께는 1로 하고

				경계선의 선 모양은 직선
				경계선의 색상은 회색으로 했으면좋겠어*/
				padding:5;

				font-size: 9pt;
				/*rm*/
				font-family: tahoma,굴림,돋움,verdana;
			}
				.yyy , .yyy th , .yyy td{
				/*.xxx th <--th와 xxx사이의 공백은 후손이라는뜻 th갖고있는애 있니.*/
				border-collapse: collapse;
				/*경계선에 입체감 주지마*/

				border: 1px solid #000000;
				/*경계선의 두께는 1로 하고

				경계선의 선 모양은 직선
				경계선의 색상은 회색으로 했으면좋겠어*/
				padding:5;

				font-size: 9pt;
				/*rm*/
				font-family: tahoma,굴림,돋움,verdana;
			}
				#zzz , .#zzz th , #zzz td{
				/*#zzz 는 id=zzz를 가진놈이다.*/
				border-collapse: collapse;
				/*경계선에 입체감 주지마*/

				border: 1px solid red;
				/*경계선의 두께는 1로 하고

				경계선의 선 모양은 직선
				경계선의 색상은 회색으로 했으면좋겠어*/
				padding:5;

				font-size: 9pt;
				/*rm*/
				font-family: tahoma,굴림,돋움,verdana;
			}



		</style>


	</head>
		<body><!-- <center> -->
			

			<table class = "xxx" align="center">
				<caption align="top">성적표</caption>

				<!-- 행을 지배하는 태그 <tr></tr> -->
				<tr bgcolor="#CBCBCB">
					<!-- 열을 지배하는 태그 <td></td> 
						두꺼워지지 않고 각셀의 왼쪽 정렬-->
					<!-- 열을 지배하는 태그 <th></th> 
						두꺼워지고,각셀의 중앙으로 정렬-->

					<th width="100">이름</th>
					<th width="80">국어</th>
					<th width="80">영어</th>
				</tr>
				<tr align="center">
					<th>사오정</th>
					<th>70</th>
					<th>70</th>
				</tr>
				<tr align="center">

					<th>저팔계</th>
					<th>98</th>
					<th>100</th>
				</tr>
				<tr align="center">

					<th>손오공</th>
					<th>95</th>
					<th>100</th>
				</tr>



			</table>

			<hr>

			<table class = "yyy">
				<caption align="top">성적표</caption>

				<!-- 행을 지배하는 태그 <tr></tr> -->
				<tr bgcolor="#CBCBCB">
					<!-- 열을 지배하는 태그 <td></td> 
						두꺼워지지 않고 각셀의 왼쪽 정렬-->
					<!-- 열을 지배하는 태그 <th></th> 
						두꺼워지고,각셀의 중앙으로 정렬-->

					<th width="100">이름</th>
					<th width="80">국어</th>
					<th width="80">영어</th>
				</tr>
				<tr align="center">
					<th>사오정</th>
					<th colspan=2>70</th>
					<!-- colspan=2 : 양옆을 합친다. -->
					<!-- <th>70</th> -->
				</tr>
				<tr align="center">

					<th>저팔계</th>
					<th>98</th>
					<th>100</th>
				</tr>
				<tr align="center">

					<th>손오공</th>
					<th>95</th>
					<th>100</th>
				</tr>



			</table>
			<hr>

			<table id="zzz">
				<caption align="top">성적표</caption>

				<!-- 행을 지배하는 태그 <tr></tr> -->
				<tr bgcolor="#CBCBCB">
					<!-- 열을 지배하는 태그 <td></td> 
						두꺼워지지 않고 각셀의 왼쪽 정렬-->
					<!-- 열을 지배하는 태그 <th></th> 
						두꺼워지고,각셀의 중앙으로 정렬-->

					<th width="100">이름</th>
					<th width="80">국어</th>
					<th width="80">영어</th>
				</tr>
				<tr align="center">
					<th>사오정</th>
					<th>70</th>
					<th>70</th>
				</tr>
				<tr align="center">

					<th>저팔계</th>
					<th>98</th>
					<th rowspan="2">100</th>
					<!-- 위아래 셀을 합친다 -->
					<!-- 먼저 코딩 되는걸 rowspan -->
					<!-- 뒤에 코딩 되는걸 주석처리 -->
				</tr>
				<tr align="center">

					<th>손오공</th>
					<th>95</th>
					<!-- <th>100</th> -->
				</tr>

			</table>
			<hr>

			<table>
				<caption align="top">성적표</caption>

				<!-- 행을 지배하는 태그 <tr></tr> -->
				<tr bgcolor="#CBCBCB">
					<!-- 열을 지배하는 태그 <td></td> 
						두꺼워지지 않고 각셀의 왼쪽 정렬-->
					<!-- 열을 지배하는 태그 <th></th> 
						두꺼워지고,각셀의 중앙으로 정렬-->

					<th width="100">이름</th><!--1행1열-->
					<th width="80">국어</th><!--1행2열-->
					<th width="80">영어</th><!--1행3열-->
				</tr>
				<tr align="center">
					<th>사오정</th> 						<!--2행1열-->
					<th colspan="2" rowspan="3">70</th> <!--2행2열-->
					<!-- <th>70</th> --> 				<!--2행3열-->
				</tr>
				<tr align="center">

					<th>저팔계</th>						<!--3행1열-->
					<!-- <th>98</th>-->        			<!--3행2열-->
					<!--<th>100</th> -->				<!--3행3열-->
				</tr>
				<tr align="center">

					<th>손오공</th>						<!--4행1열-->
					<!--<th>95</th>-->					<!--4행2열-->
					<!--<th>100</th> -->				<!--4행3열-->
				</tr>



			</table>


		</body>
</html>
 
 
 
 <!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<title></title>


	<style>
		.xxx ,.xxx th, .xxx td {

		border-collapse: collapse;
				/*경계선에 입체감 주지마*/

		border: 1px solid #A2A2A2;
				/*경계선의 두께는 1로 하고

				경계선의 선 모양은 직선
				경계선의 색상은 회색으로 했으면좋겠어*/
		padding:5;

		font-size: 8pt;
				/*rm*/
		font-family: tahoma,굴림,돋움,verdana;


		}
		.yyy ,.yyy th, .yyy td {

		border-collapse: collapse;
				/*경계선에 입체감 주지마*/

		border: 1px solid #777777;
				/*경계선의 두께는 1로 하고

				경계선의 선 모양은 직선
				경계선의 색상은 회색으로 했으면좋겠어*/
		padding :5;

		font-size: 6pt;
				/*rm*/
		font-family: tahoma,굴림,돋움,verdana;


		}

	</style>
</head>
<body><


	<table class = "xxx" cellpadding
	="5">
		
		<!-- 1행 -->
		<tr>
			<th colspan="2" align="center" height="15" bgcolor="#736AFF" ><font color="white"><&lt;추천 도서&gt;</font></th>
			
		</tr>
		<!-- 2행 <img src="img/naver.jpg">-->
		<tr>
			<th rowspan="3" width="100"><img src="img/secret.jpeg" width="100" height="130"> </th>
			<td width="200" ><b> the secret 시크릿 : 수세기 동안 단 1%만이 알았던 부와 성공의 비밀</b></td>
		</tr>
		<!-- 3행 -->

		<tr>
			<td><font color="grey">저자 : 론다 번 저/김우열 역<br>
				출판사 : 살림biz<br>
				원제 : the secret<br>
				출판일 : 2007년 06월<br></font>
			</td>
		</tr>
		<!-- 4행 -->

		<tr>
			<td><font color="grey"> 인생을 성공으로 이끄는 '위대한 비밀'의 단편들은 오래 전부터 구전과 문학과 종교와 철학에서 발견되었다. 이제 최초로 ‘비밀’의 모든 조각이 하나로 묶여 세계에 소개되었다. 이 책에서 독자는 돈, 건강, 인간관계, 행복 등 삶의 모든 면에서 ‘비밀’을 활용하는 법을 배울 것이다. 내면에 잠재되어 숨겨진 힘을 이해하기 시작할 터이고, 그리하여 모든 측면에서 기쁨을 발견하게 되리라.</font>
			</td>
		</tr>
		<!-- 5행 -->

		<tr>
			<th rowspan="3"><img src="img/because.jpeg" width="100" height="130"></th>
			<td><b>사랑하기 때문에</b></td>
		</tr>
		<!-- 6행 -->

		<tr>
			<!-- <th> </th> -->
			<td><font color="grey">저자 : 기욤 뮈소 저/전미연 역<br>
				출판사 : 밝은세상/tea & book(기획사)<br>
				원제 : parce que je t'aime<br>
				출판일 : 2007년 12월<br> </font>
			</td>
		</tr>
		<!-- 7행 -->

		<tr>
			<!-- <th> </th> -->
			<td><font color="grey"> 『사랑하기 때문에』의 주인공들인 커너, 마크, 에비, 앨리슨은 저마다 깊은 상처와 고통이 있다. 사회적인 성공이나 부의 축적과는 무관하게 상처는 현재를 어둠 속으로 밀어 넣는 동시에 미래마저 암울한 빛깔을 띠게 한다. 이 소설은 상처를 딛고 일어서는 사람들의 이야기다. 가해자와 피해자, 상처를 입힌 자와 상처받은 자들은 서로 화해와 용서를 통해 삶을 어둠 속으로 이끄는 상처를 극복해간다.
			</font>
			</td>
		</tr>





	</table>



</body>
</html>
 
 
 <!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<title></title>


	<style>
		.xxx ,.xxx th, .xxx td {

		border-collapse: collapse;
				/*경계선에 입체감 주지마*/

		border: 1px solid #A2A2A2;
				/*경계선의 두께는 1로 하고

				경계선의 선 모양은 직선
				경계선의 색상은 회색으로 했으면좋겠어*/
		padding:5;

		font-size: 8pt;
				/*rm*/
		font-family: tahoma,굴림,돋움,verdana;


		}
		.yyy ,.yyy th, .yyy td {

		border-collapse: collapse;
				/*경계선에 입체감 주지마*/

		border: 1px solid #777777;
				/*경계선의 두께는 1로 하고

				경계선의 선 모양은 직선
				경계선의 색상은 회색으로 했으면좋겠어*/
		padding :5;

		font-size: 6pt;
				/*rm*/
		font-family: tahoma,굴림,돋움,verdana;


		}

	</style>
</head>
<body><


	<table class = "xxx" cellpadding
	="5">
		
		<!-- 1행 -->
		<tr>
			<th colspan="2" align="center" height="15" bgcolor="#736AFF" ><font color="white"><&lt;추천 도서&gt;</font></th>
			
		</tr>
		<!-- 2행 <img src="img/naver.jpg">-->
		<tr>
			<th rowspan="3" width="100"><img src="img/secret.jpeg" width="100" height="130"> </th>
			<td width="200" ><b> the secret 시크릿 : 수세기 동안 단 1%만이 알았던 부와 성공의 비밀</b></td>
		</tr>
		<!-- 3행 -->

		<tr>
			<td><font color="grey">저자 : 론다 번 저/김우열 역<br>
				출판사 : 살림biz<br>
				원제 : the secret<br>
				출판일 : 2007년 06월<br></font>
			</td>
		</tr>
		<!-- 4행 -->

		<tr>
			<td><font color="grey"> 인생을 성공으로 이끄는 '위대한 비밀'의 단편들은 오래 전부터 구전과 문학과 종교와 철학에서 발견되었다. 이제 최초로 ‘비밀’의 모든 조각이 하나로 묶여 세계에 소개되었다. 이 책에서 독자는 돈, 건강, 인간관계, 행복 등 삶의 모든 면에서 ‘비밀’을 활용하는 법을 배울 것이다. 내면에 잠재되어 숨겨진 힘을 이해하기 시작할 터이고, 그리하여 모든 측면에서 기쁨을 발견하게 되리라.</font>
			</td>
		</tr>
		<!-- 5행 -->

		<tr>
			<th rowspan="3"><img src="img/because.jpeg" width="100" height="130"></th>
			<td><b>사랑하기 때문에</b></td>
		</tr>
		<!-- 6행 -->

		<tr>
			<!-- <th> </th> -->
			<td><font color="grey">저자 : 기욤 뮈소 저/전미연 역<br>
				출판사 : 밝은세상/tea & book(기획사)<br>
				원제 : parce que je t'aime<br>
				출판일 : 2007년 12월<br> </font>
			</td>
		</tr>
		<!-- 7행 -->

		<tr>
			<!-- <th> </th> -->
			<td><font color="grey"> 『사랑하기 때문에』의 주인공들인 커너, 마크, 에비, 앨리슨은 저마다 깊은 상처와 고통이 있다. 사회적인 성공이나 부의 축적과는 무관하게 상처는 현재를 어둠 속으로 밀어 넣는 동시에 미래마저 암울한 빛깔을 띠게 한다. 이 소설은 상처를 딛고 일어서는 사람들의 이야기다. 가해자와 피해자, 상처를 입힌 자와 상처받은 자들은 서로 화해와 용서를 통해 삶을 어둠 속으로 이끄는 상처를 극복해간다.
			</font>
			</td>
		</tr>





	</table>












</body>
</html>
