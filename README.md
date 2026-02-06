<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<title>For Hala ❤️</title>

<style>
body {
  background: linear-gradient(135deg, #ff758c, #ff7eb3);
  font-family: Arial, sans-serif;
  text-align: center;
  height: 100vh;
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

.container {
  background: white;
  padding: 40px 30px;
  border-radius: 25px;
  box-shadow: 0 15px 30px rgba(0,0,0,0.25);
  width: 90%;
  max-width: 430px;
  max-height: 90vh;
  overflow-y: auto;
  position: relative;
}

h1 { color: #ff4d6d; }

p {
  font-size: 16px;
  line-height: 1.9;
  color: #333;
}

.buttons {
  margin-top: 40px;
  position: relative;
  height: 160px;
}

button {
  padding: 14px 28px;
  font-size: 16px;
  border: none;
  border-radius: 30px;
  cursor: pointer;
  position: absolute;
  width: 110px;   /* حجم ثابت */
}

#yes {
  background: #ff4d6d;
  color: white;
  left: 40px;
  bottom: 20px;
}

#no {
  background: #ddd;
}

.hidden {
  display: none;
}

.love {
  text-align: right;
  margin-top: 20px;
}
</style>
</head>

<body>

<div class="container" id="card">
  <h1>حبيبتي حلا 🤍</h1>
  <p>I have a question</p>
  <h2>Would you be my Valentine?</h2>

  <div class="buttons">
    <button id="yes">Yes 💖</button>
    <button id="no">No 🙃</button>
  </div>
</div>

<div class="container hidden" id="result">
  <h1>Best decision ever 🤍🤍🤍🤍</h1>
  <p style="color:#888; font-size:14px;">14 / 2 / 2026</p>

  <div class="love">
    <p>
      حبيبتي حلا 🤍<br><br>
      أنا أكثر إنسان محظوظ بالدنيا لأنه عندي إياكي…<br><br>
      ما عندي بالدنيا أغلى منك، ولا رح يكون 🤍<br><br>
      بوسة على جبينك 😚<br>
      بحبك كثير يا روحي والله
    </p>
  </div>

  <iframe 
    width="100%" 
    height="215"
    src="https://www.youtube.com/embed/450p7goxZqg?autoplay=1&mute=0"
    allow="autoplay; encrypted-media"
    allowfullscreen>
  </iframe>
</div>

<script>
const noBtn = document.getElementById("no");
const yesBtn = document.getElementById("yes");
const card = document.getElementById("card");
const result = document.getElementById("result");

/* ثلاث أماكن ثابتة */
const positions = [
  { top: "20px", right: "20px" },
  { bottom: "20px", right: "20px" },
  { top: "70px", left: "150px" }
];

let index = 0;

function moveNo() {
  const pos = positions[index];
  noBtn.style.top = pos.top || "";
  noBtn.style.bottom = pos.bottom || "";
  noBtn.style.left = pos.left || "";
  noBtn.style.right = pos.right || "";
  index = (index + 1) % positions.length;
}

noBtn.addEventListener("mouseover", moveNo);
noBtn.addEventListener("click", function(e){
  e.preventDefault();
  moveNo();
});

yesBtn.addEventListener("click", () => {
  card.classList.add("hidden");
  result.classList.remove("hidden");
});
</script>

</body>
</html>
