# calculator
<html>
	<head>
	 
	<style>
	input[type="text"]
         {
         background-color:white;
         border: solid black 3px;
         width:100%;
        
         }

    input[type="button"]
         {
         background-color:white;
         color: blue;
         border: solid black 3px;
         width:100%

         }

    input[type="input"]
         {
         background-color:white;
         color: black;
         border: solid black 3px;
         width:100%;
        
         }

    input[type="inputType"]
         {
         background-color:red;
         color: white;
         border: solid black 3px;
         width:100%;

         }
         
    input[type="equalto"]
         {
         background-color:blue;
         color: white;
         border: solid black 3px;
         width:100%;
         height :100%

         }
    </style>
   
   </head>
	<body>
		<table border ="15%" height="10%" width ="10%">
		
		<tr>
			
			<td colspan="10"><input type="text" id="result"/></td><br><br>
		</tr>

		<tr>
			<td><input type="button" value="+" onclick="dis('+')"/> </td >
			<td><input type="button" value="-" onclick="dis('-')"/> </td>
			<td><input type="button" value="*" onclick="dis('*')"/> </td>
			<td><input type="button" value="/" onclick="dis('/')"/> </td>
		</tr><br><br>


		<tr>
			<td><input type="input" value="7" onclick="dis('7')"/> </td >
			<td><input type="input" value="8" onclick="dis('8')"/> </td>
			<td><input type="input" value="9" onclick="dis('9')"/> </td>
			<td rowspan="5"><input type="equalto" value="=" onclick="solve()" /> </td>
		</tr><br><br>

		<tr>
			<td><input type="input" value="4" onclick="dis('4')"/> </td >
			<td><input type="input" value="5" onclick="dis('5')"/> </td>
			<td><input type="input" value="6" onclick="dis('6')"/> </td>
			
		</tr><br><br>

		<tr>
			<td><input type="input" value="1" onclick="dis('1')"/> </td >
			<td><input type="input" value="2" onclick="dis('2')"/> </td>
			<td><input type="input" value="3" onclick="dis('3')"/> </td>
			
		</tr><br><br>

		<tr>
			<td><input type="input" value="0" onclick="dis('0')"/> </td >
			<td><input type="input" value="." onclick="dis('.')"/> </td>
			<td><input type="inputType" value="AC" onclick="clr('AC')" /> </td>
			
		</tr>
	</table>



		<script>
         function dis(val)
         {
             document.getElementById("result").value+=val
         }
           
         //function that evaluates the digit and return result
         function solve()
         {
             let x = document.getElementById("result").value
             let y = eval(x)
             document.getElementById("result").value = y
         }
           
         //function that clear the display
         function clr()
         {
             document.getElementById("result").value = ""
         }
      </script>
	


		
	</body>
</html>
© 2022 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
