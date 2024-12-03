<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modern Clothing Store</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <nav class="navbar navbar-dark bg-dark">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">Clothing Store</a>
        </div>
    </nav>

    <div class="container my-5">
        <h1 class="text-center mb-4">Welcome to Our Clothing Store</h1>
        <div class="row">
            <div class="col-md-4">
                <div class="card">
                    <img src="https://via.placeholder.com/150" class="card-img-top" alt="T-Shirt">
                    <div class="card-body">
                        <h5 class="card-title">T-Shirt</h5>
                        <p class="card-text">Price: $20</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card">
                    <img src="https://via.placeholder.com/150" class="card-img-top" alt="Jeans">
                    <div class="card-body">
                        <h5 class="card-title">Jeans</h5>
                        <p class="card-text">Price: $50</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card">
                    <img src="https://via.placeholder.com/150" class="card-img-top" alt="Jacket">
                    <div class="card-body">
                        <h5 class="card-title">Jacket</h5>
                        <p class="card-text">Price: $100</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="text-center mt-4">
            <button class="btn btn-success" onclick="redirectToLogin()">Login</button>
        </div>
    </div>

    <script>
        function redirectToLogin() {
            window.location.href = 'login.html';
        }
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <div class="container d-flex justify-content-center align-items-center" style="height: 100vh;">
        <div class="card p-4" style="width: 300px;">
            <h3 class="text-center mb-4">Login</h3>
            <form onsubmit="login(event)">
                <div class="mb-3">
                    <input type="text" class="form-control" placeholder="Username" required>
                </div>
                <div class="mb-3">
                    <input type="password" class="form-control" placeholder="Password" required>
                </div>
                <button type="submit" class="btn btn-primary w-100">Login</button>
            </form>
        </div>
    </div>

    <script>
        function login(event) {
            event.preventDefault();
            window.location.href = 'chat.html';
        }
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chat</title>
    <style>
        body {
            font-family: "Courier New", monospace;
            background-color: #000;
            color: #0f0;
            padding: 20px;
        }
        .chat-box {
            border: 1px solid #0f0;
            background-color: #111;
            padding: 20px;
            height: 300px;
            overflow-y: auto;
        }
        .message {
            margin-bottom: 10px;
        }
        .logout-btn {
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #ff0000;
            color: white;
            border: none;
            cursor: pointer;
        }
        .logout-btn:hover {
            background-color: #cc0000;
        }
    </style>
</head>
<body>
    <h1>Hack Chat</h1>
    <div class="chat-box">
        <div class="message"><strong>[User1]:</strong> The system is secure.</div>
        <div class="message"><strong>[User2]:</strong> Can you crack it?</div>
        <div class="message"><strong>[Admin]:</strong> Stay focused.</div>
    </div>
    <button class="logout-btn" onclick="logout()">Logout</button>

    <script>
        function logout() {
            window.location.href = 'index.html';
        }
    </script>
</body>
</html>
