<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<title></title>
		<link rel="stylesheet" href="css/1.css">
		<script language="javascript">
        function openWindow(){
            document.getElementById('light').style.display='block';
        }
        function closeWindow(){
            document.getElementById('light').style.display='none';
        }
    </script>
	<script type="text/javascript" src="js/延迟消失出现.js"></script>
	</head>
	<body>
			<div class="header">
				
				<div class="logo">
				<img src="img/1.jpg" width="80px"  height="70px"/>
				</div>
				
				<div class="search-box">
		              	<input class="search-txt" type="text" name="" placeholder="Try to search" />
		              	<a class="search-btn" href="#"><img width="40px" height="40px"src="img/搜索.jpg"</a>
	          	</div>
	          	
				<div>
					<ul class="nav">
                        <li><a href="#">关于我们</a></li>
                        <li><a href="#">产品展示</a></li>
                        <li><a href="#">联系我们</a></li>
                        <li><a class="on" href="#">首　　页</a></li>
                        
                    </ul>
				</div>
				
				<div class="login" style="font-size: 8px;">
					
					<img id="loginimg" src="img/登录.jpg" onclick="openWindow()">
			    	<div id="loginimgbottom" class="imgbottom"></div>
			    	<div id="light" class="white">
			    		<a href="#" onclick="closeWindow()">Close</a>
			    		<form action="" method="" class="">
		                	<h1>Login</h1>
		                	<div class="forminput"><input class="username" type="text" name="" id="" placeholder="Username" /></div>
		                  	<div class="forminput"><input class="pwd" type="password" name="" id="" placeholder="Password" /></div>
		                  	<div class="forminpu">
		                  		<input type="submit" name="" id="" value="Login" onclick="f()"/>
		                  		<input type="submit" name="" id="" value="sign" onclick="f()"/>
		                  	</div>
		                </form>
			    	</div>
				</div>
				
			</div>
			<div class="container">		
				<div class="cright">
					<ul class="ul">
						<li id="1" class="shu"><a class="class" style="border-top-left-radius: 10px;border-top-right-radius: 10px;" href="">岐山臊子面</a></li>						
						<li class="shu"><a href="">淮南牛肉汤</a></li>	
						<li class="shu"><a href="">热干面</a></li>	
						<li class="shu"><a href="">兰州拉面</a></li>			
						<li class="shu"><a href="">扬州炒饭</a></li>						
						<li class="shu"><a href="">狗不理</a></li>						
						<li class="shu"><a href="">版面</a></li>
						<li class="shu"><a style="border-bottom-left-radius: 10px; border-bottom-right-radius: 10px;" border-bottom-radius=10px; href="">窝窝头</a></li>
					</ul>	
         				<div class="fr"></div>
					
				</div>

					
					<div class="box">
						<div id="" class="box-img"><img id="lb" src="img/1.jpg" width="600px" height="500px" /></div>
						<div id="lb" class="box-img"><img src="img/2.jpg" width="600px" height="500px" /></div> 
						<div id="lb" class="box-img"><img src="img/3.jpg" width="600px" height="500px" /></div> 
						<div id="lb" class="box-img"><img src="img/4.jpg" width="600px" height="500px" /></div> 
						<div class="box-left" id="box-left">&lt;</div>
						<div class="box-right" id="box-right">&gt;</div>
						<div class="box-zhiding">
							<ul>
								<li class="dot"></li>
								<li class="dot"></li>
								<li class="dot"></li>	
								<li class="dot"></li>	
							</ul>
						</div>
					</div>
				<div class="cleftleft">
					<ul class="navright">
							<li class="selected">ONE</li>
							<li>TWO</li>
							<li>THREE</li>
							<li>FOUR</li>
						</ul>
						<div class="contentright">
							<div class="list ">
								<p>ONE</p>
								<p>&nbsp;&nbsp;&nbsp;黎明</p>
							</div>
							<div  class="list">
								<p>TWO</p>
								<p>&nbsp;&nbsp;&nbsp;22</p>
							</div>
							<div  class="list">
								<p>THREE</p>
								<p>&nbsp;&nbsp;&nbsp;男</p>
							</div>
							<div  class="list">
								<p>FOUR</p>
								<p>&nbsp;&nbsp;&nbsp;商务班级</p>
							</div>
						</div>
				</div>
				
				<div class="cleft">
					<ul>
                        <li><a href="#"><img src="img/面.jpg"></a></li>
                        <li><a href="#"><img src="img/饭.jpg"></a></li>
                        <li><a href="#"><img src="img/汤圆.jpg"></a></li>
					</ul>
				</div>

			</div>
			<div class="footer">
				<div class="footleft"></div>
				<div class="footcenter"></div>
				<div class="footright"></div>				
			</div>
		<script>
			window.onload=function(){
				var username=document.getElementsByClassName("username")[0];
				var pwd=document.getElementsByClassName("pwd")[0];
				var ureg=/[a-zA-Z0-9_]{6,18}/;
				var creg=/[a-zA-Z0-9]{6,}/
				var treg=/^1[34578]\d{9}$/;
				var ereg=/^\w+([-+.]\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$/;
						
				username.onfocus=function(){
				    username.style.border="1px solid red";
				    username.value="";
				}
				username.onblur=function(){
				    if(username.value==""){
				        username.value="用户名输入错误"
//				        username.value="用户名支持数字、字母和下划线，6到18个字符";
				        username.style.border="1px solid red";
				    }
				    else if((username.value!="")&&(username.value.length<6)){
				        username.value="用户名输入错误"
//				        username.value="用户名支持数字、字母和下划线，6到18个字符";
				        username.style.border="1px solid red";
				    }
					else if(username.value.length>18){
				        username.value="用户名输入错误"
//			            username.value="用户名支持数字、字母和下划线，6到18个字符";
						username.style.border="1px solid red";
					}
				    else if(!ureg.test(username.value)){
				        username.style.border="1px solid red";
				        username.value="用户名输入错误"
				    }else{
				        username.style.border="1px solid #ccc";
				    }
				}
							
				pwd.onfocus=function(){
				    pwd.lastIndex=0;
				    pwd.style.border="1px solid blue";
				    pwd.value="";
				}
				pwd.onblur=function(){
				    if(pwd.value==""){
				        pwd.style.border="1px solid red";
				        pwd.value="密码输入错误"

				    }
				    else if((pwd.value!="")&&(pwd.value.length<6)){
				        pwd.style.border="1px solid red";
				        pwd.value="密码输入错误"

				    }
				    else if(!creg.test(pwd.value)){
				        pwd.style.border="1px solid red";
				        pwd.value="密码输入错误"
				        
				    }else{
				        pwd.style.border="1px solid #ccc";
				    }
				}
				
				
				autoMove();
			}
			
			function autoMove(){
				var imgs=document.getElementsByClassName("box-img");
				var dots=document.getElementsByClassName("dot");
				function intmove(index){
					for(var i=0;i<imgs.length;i++){
						imgs[i].style.opacity='0';
						dots[i].style.background="#ccc";
					}
					imgs[index].style.opacity="1";
					dots[index].style.background="red";
				}
				intmove(0);
				
				var count=1;
				function fMove(){
					if(count==imgs.length){
						count=0
					}
					intmove(count);
					count++;
				}
				var scollMove=setInterval(fMove,2000);
				
				var right=document.getElementById("box-right");
				var left=document.getElementById("box-left");
				left.onclick=function(){
					clearInterval(scollMove);
					if(count==0){
						count=imgs.length;
					}
					count--;
					intmove(count);
				    scollMove=setInterval(fMove,2000);
				};
				right.onclick=function(){
					clearInterval(scrollMove);
					fMove();
					scollMove=setInterval(fMove,2000);
                }
				
				for(var j=0;j<dots.length;j++)
				{
					dots[j].num=j;
					dots[j].onclick=function(){
						clearInterval(scollMove);
						index=this.num;
						intmove(index);
					}
				}			
}
		</script>

	</body>
</html>
