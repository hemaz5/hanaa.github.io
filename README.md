# love in girl her name is honhon 

<html lang="ar">
<head>
<meta charset="UTF-8">
<title>💖 Love Story</title>

<style>
body{
  margin:0;
  font-family:Arial;
  color:white;
  background: linear-gradient(-45deg,#ff4d6d,#ff8fa3,#ffb3c6,#ff4d6d);
  background-size: 400% 400%;
  animation: bg 10s infinite;
  overflow-x:hidden;
}

@keyframes bg{
  0%{background-position:0% 50%}
  50%{background-position:100% 50%}
  100%{background-position:0% 50%}
}

/* أول صفحة */
.header{
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  flex-direction:column;
  text-align:center;
}

.header h1{
  font-size:40px;
}

.scroll{
  opacity:0.8;
}

/* الأقسام */
.section{
  min-height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  padding:20px;
}

.card{
  background: rgba(0,0,0,0.4);
  padding:25px;
  border-radius:20px;
  max-width:500px;
  text-align:center;
  box-shadow:0 0 20px rgba(0,0,0,0.3);
  animation: fade 1s ease-in;
}

@keyframes fade{
  from{opacity:0; transform:translateY(30px);}
  to{opacity:1; transform:translateY(0);}
}

img{
  width:100%;
  border-radius:15px;
  margin-top:10px;
}

.heart{
  font-size:50px;
  animation: beat 1s infinite;
}

@keyframes beat{
  0%{transform:scale(1);}
  50%{transform:scale(1.3);}
  100%{transform:scale(1);}
}

/* قلوب الخلفية */
.heart-bg{
  position:fixed;
  bottom:-20px;
  color:white;
  font-size:20px;
  animation: floatUp 6s linear forwards;
  opacity:0.7;
  z-index:0;
}

@keyframes floatUp{
  from{transform:translateY(0);}
  to{transform:translateY(-110vh);}
}

.content{
  position:relative;
  z-index:1;
}
</style>
</head>

<body>

<div class="content">

<!-- أول صفحة -->
<div class="header">
  <div class="heart">❤️</div>
  <h1>اجمل كل سنه وانتي طيبه يحبيبة قلبي وربنا يخليكي العمر كله ليا ونفضل ف وش بعض كده علطول </h1>
  <p class="scroll">⬇️ انزلي يبت </p>
</div>

<!-- أول صورة -->
<div class="section">
  <div class="card">
    <h2>📸 أول صورة لينا</h2>
    <p>أجمل بداية لحكايتنا ❤️</p>
    <img src="20250329j.jpg">
  </div>
</div>

<!-- أول بحبك -->
<div class="section">
  <div class="card">
    <h2>💬 أول مرة قولتلك بحبك</h2>
    <p>لحظة عمرها ما تتنسي 💖</p>
        <p> 3 May 2026 </p>
  </div>
</div>

<!-- أول خروجة -->
<div class="section">
  <div class="card">
    <h2>🌹 انا بحبك</h2>
    <p>عمري ما حسيت بالراحه والحنيه غير من جوا ايديكي</p>
  </div>
</div>

<!-- النهاية -->
<div class="section">
  <div class="card">
    <h2>💞 ولسه القصة مكملة</h2>
    <p>دي مش نهاية... دي البداية لحد ما هجيلك البيت واتجوزك يهنهونتي💖</p>
  </div>
</div>

</div>

<script>
// قلوب بتطلع
function createHeart(){
  const heart = document.createElement("div");
  heart.classList.add("heart-bg");
  heart.innerHTML = "❤️";
  heart.style.left = Math.random()*100 + "vw";
  heart.style.fontSize = (Math.random()*20 + 10) + "px";
  document.body.appendChild(heart);

  setTimeout(()=>heart.remove(),6000);
}

setInterval(createHeart,300);
</script>

</body>
</html>
