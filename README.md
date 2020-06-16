# Simple-Calculator
A simple web based Calculator will perform arithmetic mathematical operations. It is based on CSS, HTML and JAVASCRIPT file.

<html>
<head>
<style>
body
{
background-color:yellow;
}
.box
{
height:450px;
width:320px;
margin-left:100px;
background-color:green;
border-radius:20px;
}
.displaydesign
{
background color:#64d5c6;
font-size:38px;
height:110px;
width:320px;
border-top-left-radius:14px;
border-top-right-radius:14px;
font-weight700;
color:#5e5858;
}
.buttondesign
{
width:60px;
height:60px;
background:#ecedef;
font-size:30px;
font-weight:700'
color:#5E5858;;
border:none;
border-radius:50%;
cursor:pointer;
margin:20px 5px 0px 10px;
outline:none;
}
</style>

<script>
function display(val)
{
document.getElementById('final_output').value+=val;
}

function solve()
{
var expr=document.getElementById('final_output').value;
var soln=eval(expr);
document.getElementById('final_output').value=soln;
}

</script>

</head>

<body>
<h1>Simple Calculator</h1>
<div class="box">
<input type="text"class="displaydesign" id="final_output"><br/>
<button type="button"class="buttondesign" onclick="display('7')">7</button>
<button type="button"class="buttondesign" onclick="display('8')">8</button>
<button type="button"class="buttondesign" onclick="display('9')">9</button>
<button type="button"class="buttondesign" onclick="display('+')">+</button><br/>
<button type="button"class="buttondesign" onclick="display('4')">4</button>
<button type="button"class="buttondesign" onclick="display('5')">5</button>
<button type="button"class="buttondesign" onclick="display('6')">6</button>
<button type="button"class="buttondesign" onclick="display('-')">-</button><br/>
<button type="button"class="buttondesign" onclick="display('1')">1</button>
<button type="button"class="buttondesign" onclick="display('2')">2</button>
<button type="button"class="buttondesign" onclick="display('3')">3</button>
<button type="button"class="buttondesign" onclick="display('*')">*</button><br/>
<button type="button"class="buttondesign" onclick="display('0')">0</button>
<button type="button"class="buttondesign" onclick="display('.')">.</button>
<button type="button"class="buttondesign" onclick="display('/')">/</button>
<button type="button"class="buttondesign" onclick="solve()">=</button>
</div>
</body>

</html>

