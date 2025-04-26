<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Birthday Locked Site</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      padding-top: 100px;
      background-color: #000000;
      color: #ffffff;
      margin: 0;
      height: 100vh;
    }
    #content {
      display: none;
      opacity: 0;
      transition: opacity 2s ease;
    }
    input[type="password"] {
      padding: 10px;
      font-size: 16px;
      width: 250px;
      background-color: #222;
      border: none;
      color: white;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      margin-top: 10px;
      background-color: #444;
      color: white;
      border: none;
      cursor: pointer;
    }
    button:hover {
      background-color: #666;
    }
    .hint {
      margin-top: 5px;
      font-size: 14px;
      color: gray;
    }
    p.message {
      white-space: pre-line;
      font-size: 18px;
      margin-top: 20px;
    }
    #error {
      color: red;
      margin-top: 10px;
    }
  </style>
</head>
<body>

<div id="login">
  <h2>Enter my birthday</h2>
  <input type="password" id="password" placeholder="DDMMYYYY">
  <div class="hint">Format: DDMMYYYY</div>
  <br>
  <button onclick="checkPassword()">Submit</button>
  <p id="error"></p>
</div>

<div id="content">
  <h1>...</h1>
  <p class="message">
    I wish that I won't wake up tomorrow.
    Everything gonna be the same.
  </p>
</div>

<script>
  function checkPassword() {
    const correctPassword = "17062010"; // Your birthday (DDMMYYYY)
    const userInput = document.getElementById("password").value;
    if (userInput === correctPassword) {
      document.getElementById("login").style.display = "none";
      const content = document.getElementById("content");
      content.style.display = "block";
      setTimeout(() => {
        content.style.opacity = 1;
      }, 100); // small delay for smoother fade
    } else {
      document.getElementById("error").innerText = "Wrong password. Try again!";
    }
  }
</script>

</body>
</html>
