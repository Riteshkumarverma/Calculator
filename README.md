//# Calculator
//A simple Calculator using Html, Css, JavaScript
<html> 
<head> 
	<script> 
		
		function dis(val) 
		{ 
			document.getElementById("result").value+=val 
		} 
		
		 
		function solve() 
		{ 
			let x = document.getElementById("result").value 
			let y = eval(x) 
			document.getElementById("result").value = y 
		} 
		
		 
		function clr() 
		{ 
			document.getElementById("result").value = "" 
		} 
	</script> 
	
	<style> 
		.title{ 
		margin-bottom: 2px; 
		text-align: center;
		background-color: pink;
		margin: 6px;
		width: 618px;
		height: 70px; 
		font-size: 50;
		color: blue;
		border: solid black 4px; 
		} 

		input[type="button"] 
		{ 
		background-color:blue;

		color: yellow;
		font-size: 24;

		margin: 9px;
		shape-margin: 4px;
		width:130px;
		height:60px;
		} 

		input[type="text"] 
		{ 
		background-color:yellow; 
		border: solid purple 4px; 
		width:450px;
		margin: 8px;
		height:70px;
		color: red;
		font-size: 18
		} 
	</style> 
</head> 

<body> 
	<div class = title >Calculator</div> 
	<table border="1"> 
		<tr> 
			<td colspan="3"><input type="text"  id="result"/></td> 
			
			<td><input type="button" value="c" onclick="clr()"/> </td> 
		</tr> 
		<tr> 
			
			<td><input type="button" value="1" onclick="dis('1')"/> </td> 
			<td><input type="button" value="2" onclick="dis('2')"/> </td> 
			<td><input type="button" value="3" onclick="dis('3')"/> </td> 
			<td><input type="button" value="/" onclick="dis('/')"/> </td> 
		</tr> 
		<tr> 
			<td><input type="button" value="4" onclick="dis('4')"/> </td> 
			<td><input type="button" value="5" onclick="dis('5')"/> </td> 
			<td><input type="button" value="6" onclick="dis('6')"/> </td> 
			<td><input type="button" value="-" onclick="dis('-')"/> </td> 
		</tr> 
		<tr> 
			<td><input type="button" value="7" onclick="dis('7')"/> </td> 
			<td><input type="button" value="8" onclick="dis('8')"/> </td> 
			<td><input type="button" value="9" onclick="dis('9')"/> </td> 
			<td><input type="button" value="+" onclick="dis('+')"/> </td> 
		</tr> 
		<tr> 
			<td><input type="button" value="." onclick="dis('.')"/> </td> 
			<td><input type="button" value="0" onclick="dis('0')"/> </td> 
			<!-- solve function call function solve to evaluate value -->
			<td><input type="button" value="=" onclick="solve()"/> </td> 
			<td><input type="button" value="*" onclick="dis('*')"/> </td> 
		</tr> 
	</table> 
</body> 
</html> 
