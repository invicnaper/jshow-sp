jshow-sp
========

Jshow is a function that allows sending forms and showing results with out loading pages. It uses XHR to send request . just creat a form and enjoy the result :)
How to use 
========
to use JSHOW , starting with adding :

	<script src="jquery-1.10.2.js"></script>
	<script src="jshow-sp-0.1.js"></script>
	
then you should add a form to your page .

    <form name="form_test">
	  <p>Email : <input type="text" name="email"></input></p>
    <p>Last Name : <input type="text" name="last_name"></input></p>
	  <p>First Name: <input type="text" name="first_email"></input></p>
	  <input type="submit" name="submit" id="send" value="send" onclick="javascript:load_jshow('insert.php', 'form_test', 'result', 'send')"></input> 
    </form> 
    
we will call the function using : 

    onclick="javascript:load_jshow('insert.php', 'form_test', 'result', 'send')"
    
the first argument means the page that we will load ex: insert.php .
the second is the form name : form_test
the third is the id of div result
the last is the id of div error

Jshow willdetect all elements of your form . and the you should edit your php file . and use

    $_POST[element_name];
    
    
    
