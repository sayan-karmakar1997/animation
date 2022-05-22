<!DOCTYPE html>
<html>
<head>
<title>animation</title>
<style> 
	.box{
		margin-top: 50px;
		width: 200px;
		height: 25px;
		background-color: red;
		animation-name: example;
		animation-duration: 5s;
		animation-delay: 2s;
		position: relative;
		animation-iteration-count: infinite;
		border-radius: 100px;
		animation-direction: alternate-reverse;
		
	}
	@keyframes example {
	  0%   {background-color: red; left:0px;top:0px; transform: rotate(0deg);}
	  25%  {background-color: yellow; left:500px;top:0px; transform: rotate(360deg);}
	  50%  {background-color: blue; left:500px;top:200px; transform: rotate(720deg);}
	  75% {background-color: green; left:0px;top:200px; transform: rotate(1080deg);}
	  100% {background-color: #bceff5; left:0px;top:10px; transform: rotate(1440deg);}
	}
	 
	
	#one {animation-timing-function: linear;}
	#two {animation-timing-function: ease;}
	#three {animation-timing-function: ease-in;}
	#four {animation-timing-function: ease-out;}
	#five {animation-timing-function: ease-in-out;}

	
</style>
</head>
<body>

	<div class="box" id="one"></div>
	<div class="box" id="two"></div>
	<div class="box" id="three"></div>
	<div class="box" id="four"></div>
	<div class="box" id="five"></div>
	
	
</body>
</html>
