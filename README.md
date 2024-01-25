# importantLinks

You can open a GitHub repository in VS Code for the Web directly from a URL, following the schema: https://vscode.dev/github/<organization>/<repo> . Using the VS Code repository as an example, this would look like: https://vscode.dev/github/microsoft/vscode .
Ex: https://vscode.dev/github.com/Vee-ra/importantLinks/edit/main/README.md

https://stackoverflow.com/questions/46407230/load-spring-boot-app-properties-from-database
Introduction to Java Software Course | DevelopIntelligence - copy paste to URL

SQL USER CREATION:
sqlplus / as sysdba;
CREATE USER SIT_SERVICING IDENTIFIED BY SIT_SERVICING;
Grant IMP_FULL_Database to SIT_SERVICING;
GRANT ALL PRIVILEGES TO SIT_SERVICING;
https://grow.google/intl/en_in/certificates/ - Google certificates
https://getcssscan.com/css-box-shadow-examples - Too many Box shadow models
Validation:
if ((localStorage.getItem("userName") !== null) && (localStorage.getItem("password") !== null))
{
    // you have values for both userName and password
}
for your case you can test if textbox values match the values in local storage

if ((localStorage.getItem("userName") === null) && (localStorage.getItem("password") === null))
{
    localStorage.setItem("user", "Subho"); // writes name and password to local storage if not exists
    localStorage.setItem("pass", "Subho"); 
}

if ( (localStorage.getItem("user") == document.getElementById('userName').value)
{
    if ( (localStorage.getItem("pass") == document.getElementById('password').value)
    {
        // login is successful
    }           
}

----
<input type="text" id=user ><br>
                <label for="key" id=passlbl>password:</label><br>
                <input type="password" id="pd">
here is the javascript

let username = document.getElementById("user");
let pwd = document.getElementById("pd");

createCookie(username.value,pwd.value)

function createCookie(name,pwds){
    today = new Date();
    var expire = new Date();
    expire.setTime(today.getTime() + 3600000*24*15);
    document.cookie = name.value+"="+encodeURI(pwds.value)+";path=/" + ";expires="+expire.toUTCString();} 
    ---
    You can store the data as an array.

if(!localStorage.getItem("credentials")) localStorage.setItem("credentials", JSON.stringify([]));

var arr = JSON.parse(localStorage.getItem("credentials"));
console.log(arr)

let user_name = document.getElementById("username");
let user_paswrd = document.getElementById("password");

let store_data = () => {
  credentials.push({username: user_name, password: user_paswrd});
  localStorage.setItem("credentials", JSON.stringify(arr))

};
<input id="username" type='text' placeholder="username"><br>
<input id="password" type='password' placeholder="password"><br>
<button onclick="store_data">Submit</button>
-----
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>logSign</title>
</head>

<body>
  <form id="signup-form">
    <input id="name1" type="text" placeholder="Username" value="" required>
    <input id="pass1" type="password" placeholder="Password" value="" required>
    <input id="signup_btn" type="submit" value="Signup">
  </form>

  <form id="login-form">
    <input id="name2" type="text" placeholder="Username" value="" required>
    <input id="pass2" type="password" placeholder="Password" value="" required>
    <input id="login_btn" type="submit" value="Login">
  </form>
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script>
    $(document).ready(function () {
      $("#signup-form").submit(function () {
        var nm1 = $("#name1").val();
        var ps1 = $("#pass1").val();
        localStorage.setItem("n1", nm1);
        localStorage.setItem("p1", ps1);

      });

      $("#login-form").submit(function () {
        var enteredName = $("#name2").val();
        var enteredPass = $("#pass2").val();

        var storedName = localStorage.getItem("n1");
        var storedPass = localStorage.getItem("p1");

        if (enteredName == storedName && enteredPass == storedPass) {
          alert("You are logged in!");
        }
        else {
          alert("Username and Password do not match!");
        }

      });

    });
  </script>
</body>

</html>
---

