<!DOCTYPE html>
<html lang="ms">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Detektif Bacaan Pintar</title>
<style>
body {
  font-family: Arial, sans-serif;
  text-align: center;
  background: #eaf6ff;
  padding: 25px;
}
.kotak {
  background: white;
  padding: 25px;
  border-radius: 15px;
  max-width: 650px;
  margin: auto;
}
button {
  padding: 15px;
  background: #1683d8;
  color: white;
  border: none;
  border-radius: 10px;
  font-size: 18px;
}
</style>
</head>
<body>

<div class="kotak">
<h1>📖 Detektif Bacaan Pintar</h1>
<h2>Misi 1: Membaca dengan Lancar</h2>

<p id="petikan">
Ali membantu seorang warga emas melintas jalan
dengan selamat.
</p>

<button onclick="mulaBaca()">🎤 MULA MEMBACA</button>

<h3>Hasil Bacaan:</h3>
<p id="hasil">Belum ada bacaan.</p>

<h3 id="skor"></h3>
</div>

<script>
const teks = document.getElementById("petikan").innerText;

function mulaBaca() {
  const SpeechRecognition =
    window.SpeechRecognition ||
    window.webkitSpeechRecognition;

  if (!SpeechRecognition) {
    alert("Pelayar ini tidak menyokong pengecaman suara.");
    return;
  }

  const recognition = new SpeechRecognition();
  recognition.lang = "ms-MY";
  recognition.continuous = false;
  recognition.interimResults = false;

  document.getElementById("hasil").innerText =
    "Sedang mendengar bacaan...";

  recognition.onresult = function(event) {
    const bacaan = event.results[0][0].transcript;

    document.getElementById("hasil").innerText = bacaan;

    const bersih = s => s.toLowerCase()
      .replace(/[^\p{L}\p{N}\s]/gu, "")
      .trim().split(/\s+/);

    const asal = bersih(teks);
    const murid = bersih(bacaan);

    // Kira padanan mengikut turutan perkataan.
    const dp = Array.from(
      {length: asal.length + 1},
      () => Array(murid.length + 1).fill(0)
    );

    for (let i = 1; i <= asal.length; i++) {
      for (let j = 1; j <= murid.length; j++) {
        dp[i][j] = asal[i-1] === murid[j-1]
          ? dp[i-1][j-1] + 1
          : Math.max(dp[i-1][j], dp[i][j-1]);
      }
    }

    const markah = Math.round(
      (dp[asal.length][murid.length] /
       asal.length) * 100
    );

    document.getElementById("skor").innerText =
      "Skor Padanan Bacaan: " + markah + "%";
  };

  recognition.onerror = function() {
    document.getElementById("hasil").innerText =
      "Suara tidak dapat dikesan. Sila cuba lagi.";
  };

  recognition.start();
}
</script>

</body>
</html>
