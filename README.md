# User-registration

## AIM
Develop user registration form using html, css and javascript 

# ALGORITHM
### STEP 1
create a simple html page using heading tag
### STEP 2
Create a function to validate details in form using Javascript
### STEP 3
Use css to add styles to registration form
### STEP 4
Execute the program

# CODE
~~~
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>USER REGISTRATION FORM</title>
	<script>
		function Validate() {
			var name = 
				document.forms["RegForm"]["Name"];
			var email = 
				document.forms["RegForm"]["EMail"];
			var phone = 
				document.forms["RegForm"]["Telephone"];
			var what = 
				document.forms["RegForm"]["Subject"];
			var password = 
				document.forms["RegForm"]["Password"];
			var address = 
				document.forms["RegForm"]["Address"];

			if (name.value == "") {
				window.alert("Please enter your name.");
				name.focus();
				return false;
			}

			if (address.value == "") {
				window.alert("Please enter your address.");
				address.focus();
				return false;
			}

			if (email.value == "") {
				window.alert(
				  "Please enter a valid e-mail address.");
				email.focus();
				return false;
			}

			if (phone.value == "") {
				window.alert(
				  "Please enter your telephone number.");
				phone.focus();
				return false;
			}

			if (password.value == "") {
				window.alert("Please enter your password");
				password.focus();
				return false;
			}

			if (what.selectedIndex < 1) {
				alert("Please enter your course.");
				what.focus();
				return false;
			}

			return true;
		}
	</script>
	<style>
		div {
			box-sizing: border-box;
			width: 100%;
			border: 100px solid black;
			float: left;
			align-content: center;
			align-items: center;
		}

		form{
			margin: 0 auto;
			width: 600px;
			border: solid;
		}

	</style>

</head>
<body>
	<h1 style="text-align: center;">REGISTRATION FORM</h1>
        <form name="RegForm" action="/submit.php" 
              onsubmit="return Validate()" method="post">
            <p>Name: <input type="text" 
                            size="65" name="Name" /></p>
            <br />
            <p>Address: <input type="text" 
                               size="65" name="Address" />
          </p>
            <br />
            <p>E-mail Address: <input type="text" 
                            size="65" name="EMail" /></p>
            <br />
            <p>Password: <input type="text" 
                         size="65" name="Password" /></p>
            <br />
            <p>Telephone: <input type="text" 
                        size="65" name="Telephone" /></p>
            <br />
  
            <p>
                SELECT YOUR COURSE
                <select type="text" value="" name="Subject">
                    <option>BTECH</option>
                    <option>BBA</option>
                    <option>BCA</option>
                    <option>B.COM</option>
                </select>
            </p>
            <br />
            <br />
            <p>Comments: <textarea cols="55" 
                              name="Comment"> </textarea></p>
            <p>
                <input type="submit" 
                       value="send" name="Submit" />
                <input type="reset" 
                       value="Reset" name="Reset" />
            </p>
        </form>
	
</body>
</html>
~~~
# OUPUT
![SEC](t1.png)

# RESULT
user registration form using html, css and javascript was successfully executed.
