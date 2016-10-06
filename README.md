# tablesorter
Flexible client-side table sorting
<script type="text/javascript" src="/path/to/jquery-latest.js"></script> 
<script type="text/javascript" src="/path/to/jquery.tablesorter.js"></script> 

<table id="myTable" class="tablesorter"> 
<thead> 
<tr> 
    <th>Last Name</th> 
    <th>First Name</th> 
    <th>Email</th> 
    <th>Due</th> 
    <th>Web Site</th> 
</tr> 
</thead> 
<tbody> 
<tr> 
    <td>Sandy</td> 
    <td>Sandhya</td> 
    <td>sandy@gmail.com</td> 
    <td>$50.00</td> 
    <td>http://www.sandy.com</td> 
</tr> 
<tr> 
    <td>Rata</td> 
    <td>prado</td> 
    <td>prador@yahoo.com</td> 
    <td>$50.00</td> 
    <td>http://www.prado.com</td> 
</tr> 
<tr> 
    <td>R</td> 
    <td>aryan</td> 
    <td>aryan@hotmail.com</td> 
    <td>$100.00</td> 
    <td>http://www.aryan.com</td> 
</tr> 
<tr> 
    <td>Sweety</td> 
    <td>swit</td> 
    <td>sweaty@earthlink.net</td> 
    <td>$50.00</td> 
    <td>http://www.sweety.com</td> 
</tr> 
</tbody> 
</table> 

Start by telling tablesorter to sort your table when the document is loaded:

$(document).ready(function() 
    { 
        $("#myTable").tablesorter(); 
    } 
); 

Click on the headers and you'll see that your table is now sortable! You can also pass in configuration options when you initialize the table. This tells tablesorter to sort on the first and second column in ascending order.

$(document).ready(function() 
    { 
        $("#myTable").tablesorter( {sortList: [[0,0], [1,0]]} ); 
    } 
); 
