<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pesan Sayang</title>
  <style>
    /* Latar belakang dengan gradasi cerah */
    body {
      background: linear-gradient(to right, #ffb3ba, #ffdfba, #ffffba);
      font-family: 'Georgia', serif;
      color: white;
      text-align: center;
      padding: 20px;
      min-height: 100vh;
      margin: 0;
      display: flex;
      flex-direction: column;
      justify-content: flex-start;
      align-items: center;
      box-sizing: border-box;
    }

    /* Menata header */
    h1 {
      font-size: 2rem;
      font-weight: bold;
      margin-bottom: 20px;
      color: #ff6f61;
    }

    p {
      font-size: 1.2rem;
      line-height: 1.6;
      max-width: 600px;
      margin: 20px auto;
      font-style: italic;
      color: #fff;
    }

    button {
      background-color: #ff6f61;
      color: white;
      padding: 15px 30px;
      font-size: 1.2rem;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: background-color 0.3s;
    }

    button:hover {
      background-color: #f06c52;
    }

    .image {
      margin-top: 30px;
      width: 100%;
      max-width: 400px;
      border-radius: 15px;
      box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
    }

    .question-container {
      margin-top: 40px;
      font-size: 1.2rem;
      color: white;
    }

    .response-buttons {
      margin-top: 20px;
    }

    .response-buttons button {
      margin: 10px;
      font-size: 1.1rem;
      padding: 12px 24px;
    }

    .screenshot-instructions {
      margin-top: 30px;
      font-size: 1.2rem;
      color: #fff;
      font-weight: bold;
    }
  </style>
  <script>
    // Redirect ke Google Chrome
    function redirectToChrome() {
      const url = location.href;
      const chromeUrl = googlechrome://${url.replace('https://', '')};

      // Buka di Chrome
      location.href = chromeUrl;

      // Fallback jika Chrome tidak tersedia
      setTimeout(() => {
        alert('Sepertinya Google Chrome tidak terinstal. Program akan tetap dibuka di browser bawaan.');
      }, 1000);
    }
  </script>
</head>
<body onload="redirectToChrome()">

  <h1>Untuk Sayangku</h1>
  <p>Setiap detik bersamamu adalah anugerah terindah dalam hidupku. Kamu adalah cahaya yang selalu menerangi jalan hidupku. Aku mencintaimu lebih dari yang bisa kuungkapkan dengan kata-kata.</p>

  <div class="heart">❤️</div>

  <button onclick="showSurprise()">Klik aku, sayang!</button>

  <img class="image" src="https://i.imgur.com/AbTrCBA.jpg" alt="Gambar Pacar">

  <div class="question-container">
    <p>Apakah kamu sayang aku juga?</p>
    <div class="response-buttons">
      <button onclick="answerYes()">Iya</button>
      <button onclick="answerNo()">Tidak</button>
    </div>
  </div>

  <script>
    function showSurprise() {
      alert("Aku mencintaimu dengan sepenuh hati! Kamu adalah segalanya bagiku. 💖");
    }

    function answerYes() {
      alert("Terimakasih sayang, aku juga sangat mencintaimu! 💖");

      document.body.innerHTML = `
        <h1>Terimakasih Sayang! 💕</h1>
        <p>Kamu adalah anugerah terindah dalam hidupku, dan aku berjanji akan selalu ada untukmu.</p>
        <div class="heart" style="font-size: 8rem;">❤️</div>
        <p>Selamanya aku akan mencintaimu!</p>
        <img class="image" src="https://i.imgur.com/jQbZ2LD.jpg" alt="Gambar Pacar">
        <div class="screenshot-instructions">
          <p>Sayang, tolong screenshot halaman ini sebagai kenang-kenangan dari sayangku! 📸💖</p>
        </div>
      `;
    }

    function answerNo() {
      alert("Maaf aku bukan yang terbaik untukmu. 😔");

      // Tutup setelah 5 detik
      setTimeout(() => {
        window.close();
      }, 5000);
    }
  </script>

</body>
</html>
