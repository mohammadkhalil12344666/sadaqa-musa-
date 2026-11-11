
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>صدقة جارية | الحاج موسى عبد خليل</title>
<style>
*{box-sizing:border-box}
body{
 margin:0;background:#f7f7f8;color:#292929;
 font-family:Tahoma,Arial,sans-serif;line-height:1.9
}
header{
 height:65px;background:#fff;border-bottom:1px solid #e5e5e5;
 display:flex;align-items:center;justify-content:space-between;
 padding:0 7%;position:sticky;top:0;z-index:5
}
.logo{font-size:19px;font-weight:bold;color:#167b60}
nav{display:flex;gap:22px}
nav a{color:#555;text-decoration:none;font-size:14px}
nav a:hover{color:#167b60}
main{max-width:900px;margin:35px auto;padding:0 18px}
.hero{
 text-align:center;background:#fff;border:1px solid #e8e8e8;
 border-radius:20px;padding:45px 20px;margin-bottom:30px
}
.icon{font-size:35px;color:#168267}
h1{font-size:34px;margin:5px 0}
.name{color:#168267;font-size:21px;font-weight:bold}
.desc{color:#777;max-width:600px;margin:12px auto 22px}
button{
 cursor:pointer;border:0;border-radius:10px;padding:11px 20px;
 font-family:inherit;font-size:14px;transition:.2s
}
.green{background:#167b60;color:white}
.green:hover{background:#105d49}
.gray{background:#f0f0f0;color:#333}
.gray:hover{background:#e5e5e5}
.section-title{font-size:23px;margin:35px 0 15px}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:15px}
.card{
 background:white;border:1px solid #e8e8e8;border-radius:15px;
 padding:22px;transition:.2s
}
.card:hover{border-color:#c5dcd3}
.card h3{font-size:17px;margin:0 0 10px;color:#167b60}
.dua{font-size:18px;color:#333;margin:0 0 15px}
.copy{background:#f1f4f2;color:#167b60;padding:7px 13px}
.dhikr{display:flex;align-items:center;justify-content:space-between;gap:10px}
.dhikr p{margin:0;font-size:16px}
.counter{display:flex;align-items:center;gap:9px}
.number{font-size:20px;font-weight:bold;color:#167b60;min-width:25px;text-align:center}
.plus{
 width:38px;height:38px;padding:0;border-radius:50%;
 background:#e5f2ed;color:#167b60;font-size:23px
}
.reset{background:transparent;color:#777;padding:8px 0}
.message{
 background:#edf5f1;border:1px solid #dcebe3;
 border-radius:15px;padding:20px;text-align:center;
 margin-top:25px;color:#416456
}
footer{text-align:center;color:#888;font-size:13px;padding:35px 10px}
@media(max-width:650px){
 header{padding:0 15px}nav{gap:10px}nav a{font-size:12px}
 main{margin:20px auto}.hero{padding:32px 15px}
 h1{font-size:28px}.grid{grid-template-columns:1fr}
 .section-title{font-size:21px}
}
</style>
</head>
<body>

<header>
 <div class="logo">۞ صدقة جارية</div>
 <nav>
  <a href="#duas">الأدعية</a>
  <a href="#dhikr">الأذكار</a>
  <a href="#share">مشاركة</a>
 </nav>
</header>

<main>
 <section class="hero">
  <div class="icon">۞</div>
  <h1>صدقة جارية</h1>
  <div class="name">عن روح الحاج موسى عبد خليل</div>
  <p class="desc">
   اللهم ارحمه واغفر له واجعل هذا العمل صدقة جارية في ميزان حسناته،
   واجعل قبره روضة من رياض الجنة.
  </p>
  <button class="green" onclick="shareSite()">مشاركة الموقع</button>
  <button class="gray" onclick="document.getElementById('duas').scrollIntoView({behavior:'smooth'})">قراءة الأدعية</button>
 </section>

 <h2 class="section-title" id="duas">الأدعية</h2>
 <section class="grid">
  <article class="card">
   <h3>دعاء الرحمة</h3>
   <p class="dua">اللهم ارحمه رحمة واسعة واغفر له واعف عنه وأكرم نزله ووسع مدخله.</p>
   <button class="copy" onclick="copyDua(this)">نسخ الدعاء</button>
  </article>
  <article class="card">
   <h3>دعاء المغفرة</h3>
   <p class="dua">اللهم اغفر له وارحمه وعافه واعف عنه وأدخله فسيح جناتك.</p>
   <button class="copy" onclick="copyDua(this)">نسخ الدعاء</button>
  </article>
  <article class="card">
   <h3>دعاء القبر</h3>
   <p class="dua">اللهم نوّر قبره وآنس وحشته واجعل قبره روضة من رياض الجنة.</p>
   <button class="copy" onclick="copyDua(this)">نسخ الدعاء</button>
  </article>
  <article class="card">
   <h3>دعاء الجنة</h3>
   <p class="dua">اللهم ارزقه الفردوس الأعلى واجمعنا به في جنات النعيم.</p>
   <button class="copy" onclick="copyDua(this)">نسخ الدعاء</button>
  </article>
 </section>

 <h2 class="section-title" id="dhikr">الأذكار والاستغفار</h2>
 <section class="grid">
  <article class="card dhikr">
   <div><h3>الاستغفار</h3><p>أستغفر الله العظيم وأتوب إليه</p></div>
   <div class="counter"><span class="number" id="n1">0</span><button class="plus" onclick="count('n1')">+</button></div>
  </article>
  <article class="card dhikr">
   <div><h3>التسبيح</h3><p>سبحان الله وبحمده</p></div>
   <div class="counter"><span class="number" id="n2">0</span><button class="plus" onclick="count('n2')">+</button></div>
  </article>
  <article class="card dhikr">
   <div><h3>الحمد</h3><p>الحمد لله</p></div>
   <div class="counter"><span class="number" id="n3">0</span><button class="plus" onclick="count('n3')">+</button></div>
  </article>
  <article class="card dhikr">
   <div><h3>التهليل</h3><p>لا إله إلا الله</p></div>
   <div class="counter"><span class="number" id="n4">0</span><button class="plus" onclick="count('n4')">+</button></div>
  </article>
 </section>

 <button class="reset" onclick="resetCounts()">إعادة تصفير العدادات</button>

 <div class="message" id="share">
  ساهم في نشر الخير وشارك رابط هذه الصفحة مع من تحب.
  <br>نسأل الله أن يتقبل الدعاء ويجعله في ميزان حسنات المرحوم.
  <br><br>
  <button class="green" onclick="shareSite()">شارك الموقع الآن</button>
 </div>
</main>

<footer>
اللهم ارحم الحاج موسى عبد خليل وأسكنه فسيح جناتك
</footer>

<script>
function count(id){
 const el=document.getElementById(id);
 el.textContent=Number(el.textContent)+1;
}
function resetCounts(){
 ['n1','n2','n3','n4'].forEach(id=>{
  document.getElementById(id).textContent='0';
 });
}
async function shareSite(){
 const data={
  title:document.title,
  text:'صدقة جارية عن روح الحاج موسى عبد خليل',
  url:location.href
 };
 try{
  if(navigator.share){
   await navigator.share(data);
  }else{
   await navigator.clipboard.writeText(location.href);
   alert('تم نسخ رابط الموقع');
  }
 }catch(e){
  if(e.name!=='AbortError')alert('انسخ رابط الموقع من شريط المتصفح');
 }
}
async function copyDua(btn){
 const text=btn.parentElement.querySelector('.dua').textContent;
 try{
  await navigator.clipboard.writeText(text);
  alert('تم نسخ الدعاء');
 }catch(e){
  alert(text);
 }
}
</script>
</body>
</html>
