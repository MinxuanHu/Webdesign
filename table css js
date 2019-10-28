# Webdesign
<!DOCTYPE html>

<!-- Also read chapter 9 from slides - Regular Expressions -->

<html>
<head>
	<title>Table CheckList</title>
	<link rel="stylesheet" type="text/css" href="table.css">
	<link rel="stylesheet" type="text/css" href="style.css">
	<script src="script.js"></script>

</head>
<style>
  #myTable input {
	margin-left: 5px;
}

#myTable {
	border:2px solid green;
	border-collapse: collapse;
	margin: 30px 30px 20px 40px;
}
#myTable td, th {
	border:1px solid green;
	padding: 5px;
}
#myTable th {
	color: #fff;
	background-color: #a7c942;
}
#button {
	color:#fff;
	background-color: gray;
	border-radius: 3px;
	/*border:2px solid orange;*/
	margin-left: 180px;
}
</style>

<body>
<script>

	function TestBlack(TagName){

		var obj = document.getElementById(TagName);
		if(obj.style.display==""){
			obj.style.display = "none";
		}else {
			obj.style.display = "";
		}
		}
    
    function Title(t1) 
{ this.mytitle = t1;
}

Title.prototype.getName = function () 
{ 
return (this.mytitle);
}

var socialMedia = {
  facebook : 'http://facebook.com',
  twitter: 'http://twitter.com',
  flickr: 'http://flickr.com',
  youtube: 'http://youtube.com'
};

// toggle detail view function
function toggleDetail(e) {
  var x = e.target.closest("tr").nextElementSibling;
  if (x.style.display === "none" || x.style.display === "") {
    x.style.display = "table-row";
  } else {
    x.style.display = "none";
  }
}

function clickCheck(e) {
  var button = document.getElementById("button");

  var x = e.target.closest("tr");
  var headRow = document.getElementById("myTable").firstChild.nextSibling.firstChild;
  // change color
  x.style.backgroundColor = e.target.checked ? "orange" : "white";
  // change delete btn
  if(e.target.checked) {
    if(headRow.childElementCount == 8) {
      var th = document.createElement('th');
      th.innerHTML = '<th>DELETE</th>';
      headRow.appendChild(th);
    }
    var temp = document.createElement('td');
    temp.innerHTML = '<button onclick="deleteRow(event)">Delete</button>'
    x.appendChild(temp);
  }else {
    x.removeChild(x.lastChild);
    //headRow.removeChild(headRow.lastChild);
  }
}

// delete current row and detail row
function deleteRow(e) {
  var x = e.target.closest("tr");
  var detailRow = e.target.closest("tr").nextElementSibling;
  x.remove();
  detailRow.remove();
}

function TestBlack(TagName){

  var obj = document.getElementById(TagName);
  if(obj.style.display==""){
    obj.style.display = "none";
  }else {
    obj.style.display = "";
  }
}

function TestBlack(TagName){

  var obj = document.getElementById(TagName);
  if(obj.style.display==""){
    obj.style.display = "none";
  }else {
    obj.style.display = "";
  }
}


function addRow() {
  var temp = document.createElement("tr");
  temp.innerHTML = ' \
<td><input type="checkbox"  name="cb[]"  onclick="changeColor(this)"onchange="clickCheck(event)"/><br /><br /><img src="down.png"  width="25px" onclick="TestBlack(\'div4\')"/></td> \
<td>Student New</td> \
<td>Teacher New</td> \
<td>Approved</td> \
<td>Fall</td> \
<td>TA</td> \
<td>00000</td> \
<td>100%</td>'
  document.getElementById("myTable").firstElementChild.appendChild(temp);
  var temp1 = document.createElement("tr");
  temp1.id = "div4";
  temp1.style.display = "none";
  temp1.innerHTML = '\
    <td colspan="8"> \
      Advisor:<br /><br /> \
      Award Details<br /> \
      Summer 1-2014(TA)<br /> \
      Budget Number: <br /> \
      Tuition Number: <br /> \
      Comments:<br /><br /><br /> \
      Award Status:<br /><br /><br /> \
    </td>'
  temp1.className += "dropDownTextArea";
  document.getElementById("myTable").firstElementChild.appendChild(temp1);

}



 function  submit()
{
  // document.getElementById("button").style.backgroundColor="gray"

    document.getElementById("button").disabled=true;

}



var t = new Title("CONNECT WITH ME!");
</script>


	<table id="myTable" >
		<tr>
			<th></th>
			<th>STUDENT</th>
			<th>ADVISOR</th>
			<th>AWARD<br/>STATUS</th>
			<th>SEMESTER</th>
			<th>TYPE</th>
			<th>BUDGET<br />#</th>
			<th>PERCENTAGE</th>
			<th>DELETE</th>
		</tr>
		<tr class = "selectedRows">
			<td><input type="checkbox"  name="cb[]"  onclick="changeColor(this)" onchange="clickCheck(event)"/><br /><br /><img src="down.png"  onclick="TestBlack('div1')"  width="25px" /></td>
			<td>Student 1</td>
			<td>Teacher 1</td>
			<td>Approved</td>
			<td>Fall</td>
			<td>TA</td>
			<td>12345</td>
			<td>100%</td>
<!--			<td style="display: none"><button id="delete1" onclick="deleteRow(this)" name="del">Delete</button></td>-->
		</tr>
		<tr class="dropDownTextArea" id ="div1" style="display:none"><td colspan="8" >
			Advisor:<br /><br />
			Award Details<br />
			Summer 1-2014(TA)<br />
			Budget Number: <br />
			Tuition Number: <br />
			Comments:<br /><br /><br />
			Award Status:<br /><br /><br />
		</td></tr>
		<tr class = "selectedRows">
			<td><input type="checkbox"  name="cb[]" onclick="changeColor(this)" onchange="clickCheck(event)"/><br /><br /><img src="down.png" onclick="TestBlack('div2')" width="25px" /></td>
			<td>Student 2</td>
			<td>Teacher 2</td>
			<td>Approved</td>
			<td>Fall</td>
			<td>TA</td>
			<td>23456</td>
			<td>100%</td>
<!--			<td><button id="delete2" onclick="deleteRow(this)">Delete</button></td>-->
		</tr>
		<tr class="dropDownTextArea" id="div2" style="display:none"><td colspan="8">
			Advisor:<br /><br />
			Award Details<br />
			Summer 1-2014(TA)<br />
			Budget Number: <br />
			Tuition Number: <br />
			Comments:<br /><br /><br />
			Award Status:<br /><br /><br />
		</td></tr>
		<tr class = "selectedRows">
			<td><input type="checkbox"  name="cb[]" onclick="changeColor(this)" onchange="clickCheck(event)"/><br /><br /><img src="down.png" onclick="TestBlack('div3')" width="25px" /></td>
			<td>Student 3</td>
			<td>Teacher 3</td>
			<td>Approved</td>
			<td>Fall</td>
			<td>TA</td>
			<td>34567</td>
			<td>100%</td>
<!--			<td><button id="delete3" onclick="deleteRow(this)">Delete</button></td>-->
		</tr>
		<tr class="dropDownTextArea" id="div3" style="display:none"><td colspan="8">
			Advisor:<br /><br />
			Award Details<br />
			Summer 1-2014(TA)<br />
			Budget Number: <br />
			Tuition Number: <br />
			Comments:<br /><br /><br />
			Award Status:<br /><br /><br />
		</td></tr>
	</table>
<script>



	  // function deleteRow(bt){
	  // 	var f = obj.checked;
		// var tbody = document.getElementById('myTable').lastChild;
	  // 	var tr = bt.parentNode.parentNode;
		//   tbody.deleteRow(bt.parentNode.parentNode.rowIndex);
	  //
	  // }



	 function changeColor(e) {
	 	var f = e.checked;

		var chkColor = "orange"; //选中后颜色
	 	var noColor = "#fff";  //取消选中后的颜色

		 var inputs = document.getElementsByName("cb[]");
		 var checked_counts = 0;
		 for(var i=0;i<inputs.length;i++) {

			 if (inputs[i].checked) {

				 checked_counts++;
			 }
		 }
		 // alert(checked_counts）;
         if(f){
			 e.parentElement.parentElement.style.backgroundColor = chkColor;

		 }else{
			 e.parentElement.parentElement.style.backgroundColor = noColor;
         }

		if(checked_counts!= 0){

	 		document.getElementById("button").disabled=false;
	 		document.getElementById("button").style.backgroundColor="orange";}
		else{

	 		document.getElementById("button").disabled=true;
	 		document.getElementById("button").style.backgroundColor="gray";}
	  }

</script>



	<br /><br />
	<input type="submit" value="SUBMIT SELECTED AWARDS"  id="button" onclick="submit()">

	<input type="button" value="Add New Student" id="add" onclick="addRow('myTable')" >

	<nav class="socialmediaicons"></nav>
</body>
</html>
