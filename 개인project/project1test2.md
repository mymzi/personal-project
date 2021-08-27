   '''                    
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
'''

숙박인원을 나타내기 위해 count 버튼을 만들었는데 잘 되지않아서 우선 활용한 코드를 이 쪽으로 빼놓고 실현 가능한 구현을 해보았음

