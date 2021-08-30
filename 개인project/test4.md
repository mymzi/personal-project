```
<!DOCTYPE html>
<html>

  
    <head>
        <style>
          .container {
            width: 100%;
            height: 100%;
            background: rgb(231, 183, 128);
            
          }
          
       
        </style>
        <link rel="stylesheet" type="text/css" href="css/color1.css" />
        <link rel="stylesheet" type="text/css" href="css/style.css" />
      </head>
      <body style="text-align:center;">
        <div class="container">Lodging reservations  ♥ Thank you for your visit ♥</div>
      </body>
    <head>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <title>장동펜션 예약</title>
    </head>
    <body>
        
        <div style="width: 300px;margin: 0 auto;">
            <a href="notice.html"><h1 style="font-family: 'Dongle-Regular'; font-size:55px;">펜션 예약</h1></a>
          
        </div>

        
            <tr>
            <table style="width: 300px;margin: 0 auto;";>

            <tr>
               
                <th style="font-family: 'Dongle-Regular'; font-size:30px;">예약자 성함</th>   
                <td>
                    <input type="text" id="title" name="title">
                </td>
            </div>
            </tr>
            <tr>
                <th style="font-family: 'Dongle-Regular'; font-size:30px;">연락처</th>
                <td>
                    <input type="number" id="phonenumber" name="phonenumber">
                </td>
            </tr><br>
            <tr>
                <th style="font-family: 'Dongle-Regular'; font-size:30px;">숙박인원</th>
                <td>
                  <input type="number" id="persons" name="persons">
                </td>
    
            </tr>
            <th style="font-family: 'Dongle-Regular'; font-size:30px;">숙박기간</th>
              <th>    
                        <form name="reservationday" action="값을 보낼 주소" method="post">
                            <input type='date' id='reservationday' name='reservationday'/>
                        </form>
                        </th>
                   
             >
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
        <p>공지사항은 상단의 펜션 예약을 클릭해주세요!</p>
		<address>
			대표자명 : 김미지<br>
      E-Mail : alwl7615@naver.com<br>
			Address : 전라남도 장흥군 장동면 하산마을회관 맞은편<br>
			TEL : 010-4807-7615/010-8640-4064
		</address>
	</body>
</html>
```
css추가하고 펞션예약 클릭 시에 다른 페이지로 넘어가는 걸 구현하였음

```
<!DOCTYPE html>
<html>
    <head>
    </style>
    <link rel="stylesheet" type="text/css" href="css/color1.css" />
    <link rel="stylesheet" type="text/css" href="css/style.css" />
    </head>
    <body>
        <div style="width: 900px;margin: 0 auto;">
            <a href="project.html"> <h1 style="font-family: 'Dongle-Regular'; font-size:55px;">공지사항</h1></a>
            <h2 style="font-family: 'Dongle-Regular'; font-size:40px;">펜션 예약 후 예약 확정은 문자메시지나 입력하신 예약자 전화번호로 연락드리겠습니다.</h2>
            <p style="font-family: 'Dongle-Regular'; font-size:30px;">입실시간과 퇴실시간은 예약현황에 따라 달라질 수도 있습니다.<br><br>
                예약 확정 후 보내드린 계좌번호로 입금해주시면 감사하겠습니다^^.<br><br> 대표자명 : 김미지<br>
                 E-Mail : alwl7615@naver.com<br>
			    Address : 전라남도 장흥군 장동면 하산마을회관 맞은편<br>
			    TEL : 010-4807-7615/010-8640-4064<br>
                계좌번호 : 312-0094-7440-01 (농협 김미지)
                </p>

    </body>

</html>
```

