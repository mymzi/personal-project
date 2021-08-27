
<h3>test1</h3>

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
                    <th>
                        <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;인원 : <strong id="count">0</strong>
                        </p> 
                    </th>
                    <th>
                        <button onclick="countUp();">+</button>  
                        <button onclick="countDown3();">-</button> 
                        <button onclick="countRset();">0</button> 
                        
                        <script> 
                        var count=0; 
                        
                        var countUp=function(){ 
                            count=count+1; 
                            document.querySelector("#count").innerText=count; 
                            }; 
                            
                            var countDown3=function(){ 
                                if(count!==0){ 
                                    count=count-1; 
                                    document.querySelector("#count").innerText=count;
                    
                                 }
                                  }; 
                                   
                        var countRset=function(){ 
                            count=0; 
                            document.querySelector("#count").innerText=count;
                             }; 
                             
                        </script> 
                    </th>
            </tr>
            <th>숙박기간</th>
              <th>    
                        <form name="reservationday" action="값을 보낼 주소" method="post">
                            <input type='date' name='reservationday'/>
                        </form>
                        </th>
                   
           
        </table>

 
    <form action='login_page.php'>
        <div style='width:80px;float: right;'>
            <input type="button"
                      id="button1"
                      name="clicked_id"
                      value="예약"
                      onclick='button1_click()'>

                      
                
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
            var ui3 = document.getElementById('count').value;
            localStorage.setItem("count", ui3)
            var ui4 = document.getElementById('reservationday'.value);
            localStorage.setItem("reservationday", ui4)

            alert("에약하시겠습니까?");
            console.log(localStorage.getItem("title"));
        }
    </script>


</html>
```
test1에서의 문제점은 예약자성함과 연락처는 로컬스토리지에서 저장이 되는데 숙박인원과 숙박기간이 null값으로 나옴.
아직 css구현은 안됨.
php로 작성한것은 지우고 다른 html과 javascript로 새로 작성해서 예약버튼만들어야함.
