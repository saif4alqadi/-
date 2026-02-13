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
  display: flex;
  justify-content: center;
  gap: 20px;
  position: relative;
  height: 120px;
}

button {
  padding: 14px 28px;
  font-size: 16px;
  border: none;
  border-radius: 30px;
  cursor: pointer;
  width: 110px;
  height: 50px;
}

#yes {
  background: #ff4d6d;
  color: white;
}

#no {
  background: #ddd;
  position: relative;
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

  <div class="buttons" id="btnArea">
    <button id="yes">Yes 💖</button>
    <button id="no">No 🙃</button>
  </div>
</div>

<div class="container hidden" id="result">
  <h1>Best decision ever 🤍🤍🤍</h1>
  <p style="color:#888; font-size:14px;">14 / 2 / 2026</p>

  <div class="love">
    <p>
حبيبتي حلا 🤍<br><br>
      أنا أكثر إنسان محظوظ بالدنيا لأنه عندي إياكي…ما بتتخيلي يروحي قديش بضل افكر فيكي حبيبي بتعرفي زي الي عنده اشي كثير غالي بضل هيك كل شوي يفكر فيه وبضل يتفقده انا هيك معك<br><br>
      ما عندي بالدنيا أغلى منك، ولا رح يكون ... حبيبي بدعي ربنا من كل قلبي انه امورنا تتيسر واجي اتقدملك باسرع وقت لانه والله بدي اياكي وما بدي غيرك... كمان بدعي انه علاقتنا تضل قوية وعميقة عشان نقدر نعدي كل المشاكل الي بتصير للناس قبل ما ياخذوا بعض وما تأثر فينا هاي المشاكل<br><br>
      حبيبي حلا انا كل يوم بفكر باليوم الي رح اجيب عيلتي واتقدملك عنجد ما بروح من بالي هاض الاشي بضل اتخيل تفاصيل هاض اليوم وعنجد مش مصدق لحد ما يصير هاض اليوم حقيقة<br><br>
      حلا يروحي انتي كتكوتة واصيلة وجدعة ووقفتي معي كثير بحياتك ربنا يقدرني اردلك كل وقفاتك معي واكون حنون عليكي زي ما انتي حنونة علي وربنا يقدرني اعيشك بنفس مستوى عيشتك واحسن يا رب<br><br>
      بوسة على جبينك 😚<br>
      بحبك كثير يا روحي والله
    </p>
  </div>

  <iframe 
    id="song"
    width="100%" 
    height="215"
    allow="autoplay; encrypted-media"
    allowfullscreen>
  </iframe>
</div>

<script>
const noBtn = document.getElementById("no");
const yesBtn = document.getElementById("yes");
const card = document.getElementById("card");
const result = document.getElementById("result");
const song = document.getElementById("song");
const btnArea = document.getElementById("btnArea");

const positions = [
  { top: "0px", left: "0px" },
  { top: "0px", right: "0px" },
  { bottom: "0px", left: "50%" }
];

let index = 0;

function moveNo() {
  const pos = positions[index];

  noBtn.style.position = "absolute";
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

  // نشغل الاغنية بصوت بعد الضغط
  song.src = "https://www.youtube.com/embed/450p7goxZqg?autoplay=1";
});
</script>

</body>
</html>
