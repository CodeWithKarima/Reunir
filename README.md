<!DOCTYPE html>
<html>
<head>
  <title>Connexion préliminaire</title>
  <style>
    .login-popup-overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.5);
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .login-popup {
      background-color: #ffffff;
      padding: 20px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      border-radius: 5px;
      width: 300px;
    }

    .login-popup label {
      display: block;
      margin-bottom: 10px;
    }

    .login-popup input[type="text"],
    .login-popup input[type="password"] {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 3px;
    }

    .login-popup input[type="submit"] {
      width: 100%;
      padding: 10px;
      background-color: #337ab7;
      color: #ffffff;
      border: none;
      border-radius: 3px;
      cursor: pointer;
    }

    .login-popup input[type="submit"]:hover {
      background-color: #286090;
    }
  </style>
</head>
<body>
  <div class="login-popup-overlay">
    <div class="login-popup">
      <form action="authentification.php" method="post">
        <label for="username">Nom d'utilisateur:</label>
        <input type="text" id="username" name="username" required>

        <label for="password">Mot de passe:</label>
        <input type="password" id="password" name="password" required>

        <input type="submit" value="Se connecter">
      </form>
    </div>
  </div>
</body>
</html>
