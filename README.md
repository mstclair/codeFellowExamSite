<!DOCTYPE html>
<html lang ="en">
<head>
<title>Sign-In</title>
<meta charset = "UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" type="text/css"href="style.css"> 
<SCRIPT LANGUAGE="JavaScript">
function NameData (form) {
    var TestVar = form.inputbox.value;
	if(TestVar.length===0)
		{
    alert ("You must have not entered anything " + TestVar+ " please enter your name");
		}
	else if (TestVar.length>0)
	{	
		
		window.open("MFTExamII.html");
		
		localStorage.clear();
		localStorage.setItem("name", TestVar)
	}

}
</SCRIPT>

</head>
<body>

<div class="container">

<header>
   <h1>What you need to know to pass the Washington State MFT Licensure Exam</h1>
</header>
  
<article>


	<h1 style = "background-color: black; width: 100%; height:15%;" >Sign in and access resources, strategies, and other helpful information</h1>
 
 <img src = "WAstate.jpg">
 <FORM NAME="myform" ACTION="" METHOD="GET">Enter Name <BR>
<INPUT TYPE="text" NAME="inputbox" VALUE="" placeholder= "Name"><P>
<INPUT TYPE="button" NAME="button" Value="Submit" onClick="NameData(this.form)">
</FORM>


</article>

<footer>Matt St.Clair Web Productions</footer>

</div>

</body>

</html>

