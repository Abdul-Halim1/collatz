# collatz
<html>
	<head>
		<title>Titel</title>
		<meta http-equiv="Content-Type" content="text/html; charset=utf-8">

		<script>

			"use strict";
function Problem() {
var vN;
var vAusgabe;
var vP="->";
var vBerechnung=0;

vN = parseFloat(document.getElementById("idN").value);

vAusgabe="";


while(vN!=1){

vBerechnung++;

    if (vN%2==0) {
vAusgabe = vAusgabe+ vN/2 +vP ;

} else {

    vAusgabe = vAusgabe+vN*3+1 +vP ;

}
vBerechnung;



}
document.getElementById("idAusgabe").innerHTML = vAusgabe;


}
	 




		 </script>

</head>

	<body>
		<h1>Collatz 3n+1 Problem</h1>
      
		Collatz-Zahl:  <input id="idN" type="text" value="10"> <button onClick="Problem();">Collatz</button>




<div id="idAusgabe"></div>
	</body>
</html>
