# green045.github.io
<html>
<head>
<script type="text/javascript">
function show_page1()
{
var xmlhttp;

if (window.XMLHttpRequest)
  {// code for IE7+, Firefox, Chrome, Opera, Safari
  xmlhttp=new XMLHttpRequest();
  }
else
  {// code for IE6, IE5
  xmlhttp=new ActiveXObject("Microsoft.XMLHTTP");
  }
xmlhttp.onreadystatechange=function()
  {
  if (xmlhttp.readyState==4 && xmlhttp.status==200)
    {
    document.getElementById("content").innerHTML=xmlhttp.responseText;
    }
  }
xmlhttp.open("GET","rule_page1.asp",true);
xmlhttp.send();
}
function show_page2()
{
var xmlhttp;

if (window.XMLHttpRequest)
  {// code for IE7+, Firefox, Chrome, Opera, Safari
  xmlhttp=new XMLHttpRequest();
  }
else
  {// code for IE6, IE5
  xmlhttp=new ActiveXObject("Microsoft.XMLHTTP");
  }
xmlhttp.onreadystatechange=function()
  {
  if (xmlhttp.readyState==4 && xmlhttp.status==200)
    {
		/*var hint ="<h1>遊戲規則</h1>"+
			"<p>出牌：當輪到玩家回合，說故事可打出任意張故事卡，但一句話只能打出一張卡</p>"+
			"<p>棄權：當玩家無法接續下去，可喊棄權並抽一張卡，左方玩家接續</p>")
		document.getElementById("content").innerHTML=hint;
		*/
		document.getElementById("content").innerHTML=xmlhttp.responseText;
    }
  }
xmlhttp.open("GET","rule_page2.asp?t=" + Math.random(),true);
xmlhttp.send();
}
function show_page3()
{
var xmlhttp;

if (window.XMLHttpRequest)
  {// code for IE7+, Firefox, Chrome, Opera, Safari
  xmlhttp=new XMLHttpRequest();
  }
else
  {// code for IE6, IE5
  xmlhttp=new ActiveXObject("Microsoft.XMLHTTP");
  }
xmlhttp.onreadystatechange=function()
  {
  if (xmlhttp.readyState==4 && xmlhttp.status==200)
    {
    document.getElementById("content").innerHTML=xmlhttp.responseText;
    }
  }
xmlhttp.open("GET","rule_page3.asp",true);
xmlhttp.send();
}
function show_page4()
{
var xmlhttp;

if (window.XMLHttpRequest)
  {// code for IE7+, Firefox, Chrome, Opera, Safari
  xmlhttp=new XMLHttpRequest();
  }
else
  {// code for IE6, IE5
  xmlhttp=new ActiveXObject("Microsoft.XMLHTTP");
  }
xmlhttp.onreadystatechange=function()
  {
  if (xmlhttp.readyState==4 && xmlhttp.status==200)
    {
    document.getElementById("content").innerHTML=xmlhttp.responseText;
    }
  }
xmlhttp.open("GET","rule_page4.asp",true);
xmlhttp.send();
}
</script>
</head>
<body>

<div id ="content"><h1>遊戲規則</h1></div>

<form action=""> 
<button id ="page1" onclick="show_page1()">1</button>
<button id ="page2" onclick="show_page2()">2</button>
<button id ="page3" onclick="show_page3()">3</button>
<button id ="page4" onclick="show_page4()">4</button>
</form>

</body>
</html>
