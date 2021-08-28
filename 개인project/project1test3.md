```
<!DOCTYPE html>
<html>
    <head>
        <style>
          .container {
            width: 100%;
            height: 100%;
            background: pink;
          }
        </style>
      </head>
      <body style="text-align:center;">
        <div class="container">Lodging reservations  ♥ Thank you for your visit ♥</div>
      </body>
    <head>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <title>장동펜션 예약</title>
    </head>
    <body>
        <h1>펜션 예약하기</h1>
        <table style="width: 500px; height: 400px; margin: 0px auto;">
            <tr>
                <th>성함</th>   
                <td>
                    <input type="text" id="title" name="title">
                </td>
            </tr>
            <tr>
                <th>연락처</th>
                <td>
                    <input type="number" id="phonenumber" name="phonenumber">
                </td>
            </tr><br>
            <tr>
                <th>인원</th>
                <td>
                  <input type="number" id="persons" name="persons">
                </td>
    
            </tr>
            <th>숙박기간</th>
              <th>    
                        <form name="reservationday" action="값을 보낼 주소" method="post">
                            <input type='date' id='reservationday' name='reservationday'/>
                        </form>
                        </th>
                   
           
        </table>

 
        <div style='width:80px;float: right;'>
            <input type="button"
                      id="button1"
                      name="clicked_id"
                      value="예약"
                      onclick='button1_click()'                 
            >         
                
        </div>
        <div style='width:50px;float: right;'>
            <input type='button'
                      class='btn'
                      name='btn'
                      value='취소'
                      onclick='alert("취소하시겠습니까?")'>
        </div>

                      

        
        
    </form>

    <script>
        function button1_click(){
            var ui1 = document.getElementById('title').value;
            localStorage.setItem("title", ui1)
            var ui2 = document.getElementById('phonenumber').value;
            localStorage.setItem("phonenumber", ui2)
            var ui3 = document.getElementById('persons').value;
            localStorage.setItem("persons", ui3)
            var ui4 = document.getElementById('reservationday').value;
            localStorage.setItem("reservationday", ui4)

            alert("에약하시겠습니까?");
            console.log(localStorage.getItem("title"));
        }
    </script>


</html>
<br>
<br>

<!doctype html>
<html lang="ko">
	<head>
	<meta charset="utf-8">
		<title>HTML</title>
	</head>
	<body>
		<p>장동펜션에 오신 걸 환영합니다.</p>
		<address>
			대표자명 : 김종만<br>
      E-Mail : alwl7615@naver.com<br>
			Address : 전라남도 장흥군 장동면 하산마을회관 맞은편<br>
			TEL : 010-4807-7615/010-8640-4064
		</address>
	</body>
</html>
```

카운트 증감버튼을 없애고 직접 숫자를 입력하는 방식으로 바꾸어 로컬스토리지에 뜨게 코딩하였다
숙박인원이 로컬스토리지에 나올 수 있도록 다시 확인을 해보았는데  value가 ()밖으로 꺼내져 나오게해서 해결하였다.

해결안된점--> css를 사용해서 홈페이지를 좀 더 꾸민 후 시간이 남으면 예약자확인페이지로 넘어갈 수 있도록 form을 만들어 볼 예정이다.
