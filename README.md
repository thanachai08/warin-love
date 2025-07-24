<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <title>ถึงวาริน 💖</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="https://fonts.googleapis.com/css2?family=Kanit&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(to bottom, #ffe6f0, #ffd6ec);
      font-family: 'Kanit', sans-serif;
      text-align: center;
      color: #d63384;
    }

    .cover {
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      background: #fff0f5;
      display: flex;
      align-items: center;
      justify-content: center;
      z-index: 10;
      font-size: 2em;
      font-weight: bold;
      cursor: pointer;
      animation: fadein 2s ease-in-out;
    }

    @keyframes fadein {
      from { opacity: 0; } to { opacity: 1; }
    }

    .container {
      padding: 40px 20px;
      display: none;
    }

    .message {
      font-size: 1.4em;
      line-height: 1.8em;
      margin-bottom: 30px;
    }

    .btn {
      background-color: #ff99cc;
      color: white;
      font-size: 1.3em;
      padding: 15px 30px;
      margin: 10px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      transition: 0.3s;
    }

    .btn:hover {
      background-color: #ff66b2;
    }

    img {
      max-width: 200px;
      margin-top: 30px;
    }
  </style>
</head>
<body>

  <div class="cover" onclick="openPage()">แตะเพื่อเปิด 💖</div>

  <div class="container" id="mainContent">
    <div class="message">
      ตั้งแต่เราคุยกัน หนูทำให้พี่ยิ้มมากขึ้นทุกวันเลย<br><br>
      พี่มีความสุขมากๆ เลยนะ ตั้งแต่มาเจอหนู<br><br>
      หนูทำให้พี่อยากกลับมามีความรักอีกครั้ง<br><br>
      สุดท้ายนี้... อยากจะบอกว่า<br><br>
      <strong style="font-size:1.6em; color:#ff3399;">เป็นแฟนกันนะ 💖</strong>
    </div>

    <button class="btn" onclick="confirmLove()">ตกลง</button>
    <button class="btn" onclick="confirmLove()">ตกลง</button>

    <img src="https://i.pinimg.com/originals/ff/97/c8/ff97c87eebffcf916c41b19e63e53e56.png" alt="Cinnamoroll">
  </div>

  <!-- เพลง -->
  <audio id="bgMusic" autoplay loop>
    <source src="https://dl.dropboxusercontent.com/scl/fi/8o8wy1of2us1lw5ae4v1b/คู่ชีวิต-เพลง.mp3?rlkey=ti93v9scqp42yqwj6wh1f0nho&dl=0" type="audio/mpeg">
    เพลงนี้เล่นไม่ได้ในอุปกรณ์ของคุณ
  </audio>

  <script>
    function openPage() {
      document.querySelector('.cover').style.display = 'none';
      document.getElementById('mainContent').style.display = 'block';
      document.getElementById("bgMusic").play();
    }

    function confirmLove() {
      alert("เย้ พี่ดีใจที่สุดเลย 💖 พี่รักหนูนะ จะดูแลให้ดีที่สุดเลย 😊");
    }
  </script>

</body>
</html>
