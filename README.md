<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login to Shinwari webpage</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <a href="index.html">Home</a>
    <a href="http://127.0.0.1:5500/Deshbourd.html"class= "click here-button">click here</a>
    <div class="container">
        <div class="form-container">
            <form id="login-form">
                <h2>Login</h2>
                <div class="form-group">
                    <label for="login-username">Username:</label>
                    <input type="text" id="login-username" name="login-username" required>
                </div>
                <div class="form-group">
                    <label for="login-password">Password:</label>
                    <input type="password" id="login-password" name="login-password" required>
                </div>
                <a href="http://127.0.0.1:5500/Deshbourd.html"></a>
                <button type="submit">Login</button>
            </form>
            <div class="register-link">
                <p>Don't have an account? <a href="#" id="register-link">Register here</a></p>
            </div>
        </div>
        <div class="form-container hidden" id="register-form-container">
            <form id="register-form">
                <h2>Register</h2>
                <div class="form-group">
                    <label for="register-username">Username:</label>
                    <input type="text" id="register-username" name="register-username" required>
                </div>
                <div class="form-group">
                    <label for="register-password">Password:</label>
                    <input type="password" id="register-password" name="register-password" required>
                    <a href="index.html">Home</a>
    <a href="http://127.0.0.1:5500/Deshbourd.html">Shinwari webpage</a>
    <button>Done</button>
                </div>
                <a href="index.html">Home</a>
    <a href="http://127.0.0.1:5500/Deshbourd.html">Shinwari webpage</a>
                <button>Done</button>
            </form>
            <div class="login-link">
                <p>Already have an account? <a href="#" id="login-link">Login here</a></p>
            </div>
        </div>
    </div>

    <script src="script.js"></script>
</body>
<style class="css">
    body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f2f2f2;
}

.container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.form-container {
    background-color: #fff;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.form-group {
    margin-bottom: 15px;
}

label {
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
}

input {
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

button {
    padding: 10px 20px;
    background-color: #007bff;
    border: none;
    color: #fff;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
}

.hidden {
    display: none;
}

.register-link,
.login-link {
    text-align: center;
}

.register-link a,
.login-link a {
    color: #007bff;
}
</style>
<javascript class="js">
    document.addEventListener("DOMContentLoaded", function() {
        document.getElementById("register-link").addEventListener("click", function(event) {
            event.preventDefault();
            document.getElementById("login-form").classList.add("hidden");
            document.getElementById("register-form-container").classList.remove("hidden");
        });
    
        document.getElementById("login-link").addEventListener("click", function(event) {
            event.preventDefault();
            document.getElementById("register-form-container").classList.add("hidden");
            document.getElementById("login-form").classList.remove("hidden");
        });
    
        document.getElementById("login-form").addEventListener("submit", function(event) {
            event.preventDefault();
            var username = document.getElementById("login-username").value;
            var password = document.getElementById("login-password").value;
            // You can add your login logic here, like sending a request to a server
            console.log("Login with username: " + username + " and password: " + password);
        });
    
        document.getElementById("register-form").addEventListener("submit", function(event) {
            event.preventDefault();
            var username = document.getElementById("register-username").value;
            var password = document.getElementById("register-password").value;
            // You can add your registration logic here, like sending a request to a server
            console.log("Register with username: " + username + " and password: " + password);
        });
    });
    
</javascript>
</html>
