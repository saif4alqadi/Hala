<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>For Hala ❤️</title>
<style>
body {
  background: linear-gradient(135deg, #ff758c, #ff7eb3);
  font-family: 'Arial', sans-serif;
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
}

h1 {
  color: #ff4d6d;
}

p {
  font-size: 16px;
  color: #333;
  line-height: 1.7;
}

.buttons {
  margin-top: 35px;
  position: relative;
  height: 140px;
}

button {
  padding: 14px 28px;
  font-size: 16px;
  border: none;
  border-radius: 30px;
  cursor: pointer;
}

#yes {
  background: #ff4d6d;
  color: white;
}

#no {
  background: #ddd;
  position: absolute;
}

.no-text {
  margin-top: 10px;
  font-size: 14px;
  color: #ff4d6d;
  height: 18px;
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
  <h1>حبيبي حلا🤍</h1>
  <p>I have a question</p>
  <h2>Would you be my Valentine?</h2>

  <div class="buttons">
    <button id="yes">Yes 💖</button>
    <button id="no">No 🙃</button>
  </div>

  <div class="no-text" id="noText"></div>
</div>

<div class="container hidden" id="result">
  <h1>Best decision ever 🤍🤍🤍🤍</h1>
<p style="color:#888; font-size:14px; margin-top:-10px;">
14 / 2 / 2026
</p>
  <div class="love">
    <p>
      حبيبتي حلا 🤍<br><br>

      أنا أكثر إنسان محظوظ بالدنيا لأنه عندي إياكي…  
      عنجد أنا ما بعرف شو عملت إشي منيح بحياتي عشان ربنا يخلي قلبك يحبني.<br><br>

      بتعرفي حلا، هيك لما الواحد يكون عنده إشي غالي كثير؟  
      زي واحد اشترى شغلة غالية، كيف بضل طول الوقت يفكر فيها ويتطلع عليها؟  
      أنا هيك بحس معك والله.<br><br>

      وعنجد يا روحي، ما بعرف إذا هاض الإشي healthy أو لا،  
      بس أنا أغلب الوقت بخاف عليكي وبعتبرك زي بنتي  
      أكثر ما إني أفكر فيكي كحبيبتي…  
      (مع إني أكيد بفكر فيكي كحبيبتي 🙂🙂🙂)  
      بس قصدي من كثر الحب 🤍<br><br>

      حبيبتي حلا،  
      ما عندي بالدنيا أغلى منك، ولا رح يكون.  
      ما في حدا بحنيتك، لأنك حنونة عليّ… حنونة عليي.<br><br>

      وبعرف إنه أي حدا بالعالم هسا نفسه يكون مكاني  
      وتكوني إنتِ الڤالنتاين تبعتهم،  
      بس يخسوا والله ما ينولوها 😌<br><br>

      بوسة على جبينك 😚<br>
      بحبك كثير يا روحي والله 🤍
    </p>
  </div>

  <iframe width="100%" height="215"
    src="https://www.youtube.com/embed/450p7goxZqg?autoplay=1"
    frameborder="0" allow="autoplay; encrypted-media" allowfullscreen>
  </iframe>
</div>

<script>
const noBtn = document.getElementById("no");
const yesBtn = document.getElementById("yes");
const card = document.getElementById("card");
const result = document.getElementById("result");
const noText = document.getElementById("noText");

const phrases = ["تخسي 😌", "فشرتي 😂", "لا تحاولي 😏", "بالله؟ 🙄"];

noBtn.style.top = "60px";
noBtn.style.left = "140px";

noBtn.addEventListener("mouseover", () => {
  const x = Math.random() * 260;
  const y = Math.random() * 90;
  noBtn.style.left = x + "px";
  noBtn.style.top = y + "px";

  const randomPhrase = phrases[Math.floor(Math.random() * phrases.length)];
  noText.textContent = randomPhrase;
});

yesBtn.addEventListener("click", () => {
  card.classList.add("hidden");
  result.classList.remove("hidden");
});
</script>

</body>
</html>
