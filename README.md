<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login - Hole in One</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #1a1a1a;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .login-container {
            background: #2e2b23;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(255, 215, 0, 0.5);
            text-align: center;
            width: 300px;
        }
        h2 {
            margin-bottom: 20px;
            color: #d4af37;
        }
        input {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .btn {
            background-color: #d4af37;
            color: black;
            border: none;
            padding: 10px;
            width: 100%;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
        }
        .btn:hover {
            background-color: #b8860b;
        }
        .links {
            margin-top: 10px;
        }
        .links a {
            color: #d4af37;
            text-decoration: none;
        }
        .links a:hover {
            text-decoration: underline;
        }

        /* Media Query for mobile devices */
        @media (max-width: 768px) {
            .login-container {
                width: 90%; /* Take up more space on smaller screens */
                padding: 20px;
            }
            h2 {
                font-size: 24px; /* Smaller header size */
            }
            input, .btn {
                font-size: 14px; /* Adjust input and button size */
            }
        }
    </style>
</head>
<body>
    <div class="login-container">
        <h2>Login to Hole in One</h2>
        <form id="loginForm">
            <input type="email" id="email" placeholder="Email" required>
            <input type="password" id="password" placeholder="Password" required>
            <button type="submit" class="btn">Login</button>
        </form>
        <div class="links">
            <p><a href="PASS FORG.html">Forgot Password?</a></p>
            <p><a href="sign up page.html">Create an Account</a></p>
        </div>
    </div>

    <script>
        // Adding event listener for form submission
        document.getElementById("loginForm").addEventListener("submit", function(event) {
            event.preventDefault(); // Prevent form from submitting the traditional way

            // Get the values entered by the user
            const email = document.getElementById("email").value;
            const password = document.getElementById("password").value;

            // Example check (in a real-world scenario, you would compare against a database)
            if (email && password) {
                // Redirect to home page (or you can put the actual URL of your home page)
                window.location.href = "home page.html"; // Change this URL to match your home page
            } else {
                alert("Please enter a valid email and password.");
            }
        });
    </script>
</body>
</html>
