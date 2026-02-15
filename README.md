# ryzzx2.0 <!DOCTYPE html>
<html>
<head>
  <title>Question</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
      background-color: #ffe6f0;
      margin-top: 100px;
    }

    h1 {
      font-size: 40px;
    }

    .btn {
      font-size: 20px;
      padding: 10px 20px;
      margin: 20px;
      cursor: pointer;
      border: none;
      border-radius: 10px;
    }

    #yes {
      background-color: #ff66b2;
      color: white;
    }

    #no {
      background-color: #999;
      color: white;
      position: absolute;
    }
  </style>
</head>
<body>

<h1>Do you like me?</h1>

<button class="btn" id="yes" onclick="yesClick()">Yes</button>
<button class="btn" id="no" onmouseover="moveNo()">No</button>

<script>
  function yesClick() {
    document.body.innerHTML = "<h1>Yayyy ❤️ I like you too!</h1>";
  }

  function moveNo() {
    let x = Math.random() * window.innerWidth - 100;
    let y = Math.random() * window.innerHeight - 100;

    document.getElementById("no").style.left = x + "px";
    document.getElementById("no").style.top = y + "px";
  }
</script>

</body>
</html>.
