
<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Shorif Topup Center BD</title>
<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial,sans-serif;background:#0b1020;color:#fff}
header{padding:24px 14px;text-align:center;background:linear-gradient(135deg,#171b42,#472080)}
header h1{color:#ffe66d;margin:8px 0}
header p{color:#ddd}
nav{text-align:center;padding:12px;background:#171b2e}
nav a{color:#ffe66d;text-decoration:none;margin:0 8px}
main{max-width:850px;margin:auto;padding:16px}
.panel{background:#171d31;border:1px solid #303957;border-radius:14px;padding:17px;margin:16px 0}
h2{color:#ffe66d}
.admin{text-align:center}
.avatar{font-size:55px}
.packages{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:12px}
.package{background:#222b46;border-radius:12px;padding:15px;text-align:center}
.package h3{margin:5px;color:#ffe66d}
.price{font-size:21px;font-weight:bold;margin:10px}
button{background:#ffe66d;color:#17152a;border:0;border-radius:9px;padding:12px;font-weight:bold;cursor:pointer}
.package button{width:100%}
label{display:block;margin:12px 0 6px}
input,select{width:100%;padding:12px;border-radius:8px;border:1px solid #47516c;background:#0d1426;color:white}
.pay{line-height:1.9;overflow-wrap:anywhere}
.note{color:#cbd2e5;font-size:13px;line-height:1.6}
footer{text-align:center;padding:24px;color:#b8bfd5}
@media(max-width:400px){.packages{grid-template-columns:1fr}}
</style>
</head>
<body>

<header>
<div style="font-size:38px">💎</div>
<h1>SHORIF TOPUP CENTER BD</h1>
<p>Free Fire Diamond Top-Up Center</p>
<p>⚡ সহজ অর্ডার • দ্রুত সেবা</p>
</header>

<nav>
<a href="#packages">Diamond</a>
<a href="#order">অর্ডার</a>
<a href="#payment">পেমেন্ট</a>
</nav>

<main>
<section class="panel admin">
<div class="avatar">👑</div>
<h2>Shorif</h2>
<p>Owner &amp; Top-Up Manager</p>
<p>স্বাগতম আমার Top-Up Center-এ!</p>
</section>

<section class="panel" id="packages">
<h2>💎 Diamond Packages</h2>
<div class="packages">
<div class="package"><h3>25 Diamonds</h3><div class="price">৳25</div><button onclick="choose('25 Diamonds',25)">অর্ডার</button></div>
<div class="package"><h3>50 Diamonds</h3><div class="price">৳40</div><button onclick="choose('50 Diamonds',40)">অর্ডার</button></div>
<div class="package"><h3>115 Diamonds</h3><div class="price">৳80</div><button onclick="choose('115 Diamonds',80)">অর্ডার</button></div>
<div class="package"><h3>240 Diamonds</h3><div class="price">৳160</div><button onclick="choose('240 Diamonds',160)">অর্ডার</button></div>
<div class="package"><h3>Weekly Lite</h3><div class="price">৳50</div><button onclick="choose('Weekly Lite',50)">অর্ডার</button></div>
<div class="package"><h3>Weekly</h3><div class="price">৳160</div><button onclick="choose('Weekly',160)">অর্ডার</button></div>
<div class="package"><h3>Monthly</h3><div class="price">৳770</div><button onclick="choose('Monthly',770)">অর্ডার</button></div>
<div class="package"><h3>Level Up Pass</h3><div class="price">৳420</div><button onclick="choose('Level Up Pass',420)">অর্ডার</button></div>
</div>
<p class="note">দাম ও প্যাকেজের প্রাপ্যতা অর্ডারের আগে যাচাই করে নিন।</p>
</section>

<section class="panel" id="payment">
<h2>💳 Payment Information</h2>
<div class="pay">
<b>bKash Personal:</b> 01781893290<br>
<b>Nagad Personal:</b> 01781893290
</div>
<p class="note">পেমেন্ট করার আগে নম্বরটি মালিকের সঙ্গে নিশ্চিত করুন। পেমেন্টের পর Transaction ID দিন। PIN বা OTP কখনো দেবেন না।</p>
</section>

<section class="panel" id="order">
<h2>🛒 অর্ডার ফর্ম</h2>
<form id="orderForm">
<label for="player">Free Fire Player UID</label>
<input id="player" required inputmode="numeric" placeholder="আপনার Player UID">

<label for="pack">প্যাকেজ</label>
<select id="pack" required>
<option value="">প্যাকেজ নির্বাচন করুন</option>
<option value="25 Diamonds|25">25 Diamonds - ৳25</option>
<option value="50 Diamonds|40">50 Diamonds - ৳40</option>
<option value="115 Diamonds|80">115 Diamonds - ৳80</option>
<option value="240 Diamonds|160">240 Diamonds - ৳160</option>
<option value="Weekly Lite|50">Weekly Lite - ৳50</option>
<option value="Weekly|160">Weekly - ৳160</option>
<option value="Monthly|770">Monthly - ৳770</option>
<option value="Level Up Pass|420">Level Up Pass - ৳420</option>
</select>

<label for="method">পেমেন্ট মাধ্যম</label>
<select id="method" required>
<option value="">নির্বাচন করুন</option>
<option>bKash</option>
<option>Nagad</option>
</select>

<label for="trx">Transaction ID</label>
<input id="trx" required placeholder="পেমেন্টের Transaction ID">

<button type="submit" style="width:100%;margin-top:18px">অর্ডার তথ্য তৈরি করুন</button>
</form>
<p class="note">এই ফর্ম অর্ডারের মেসেজ তৈরি করবে। এটি নিজে থেকে পেমেন্ট যাচাই বা অর্ডার সংরক্ষণ করে না।</p>
<div id="result" style="display:none;margin-top:16px">
<p>আপনার অর্ডারের তথ্য তৈরি হয়েছে:</p>
<textarea id="message" rows="7" style="width:100%;padding:10px" readonly></textarea>
<button type="button" onclick="copyOrder()">অর্ডার কপি করুন</button>
</div>
</section>

<section class="panel">
<h2>📞 যোগাযোগ</h2>
<p>অর্ডার বা পেমেন্ট বিষয়ে সাহায্যের জন্য দোকানের মালিকের সঙ্গে যোগাযোগ করুন।</p>
<p class="note">এখানে এখনো আলাদা WhatsApp বা Facebook যোগাযোগের লিংক যোগ করা হয়নি।</p>
</section>
</main>

<footer>
© <span id="year"></span> Shorif Topup Center BD
<p>Unofficial Free Fire top-up service.</p>
</footer>

<script>
document.getElementById("year").textContent=new Date().getFullYear();

function choose(name,price){
document.getElementById("pack").value=name+"|"+price;
document.getElementById("order").scrollIntoView({behavior:"smooth"});
}

document.getElementById("orderForm").addEventListener("submit",function(e){
e.preventDefault();
const uid=document.getElementById("player").value.trim();
const selected=document.getElementById("pack").value.split("|");
const method=document.getElementById("method").value;
const trx=document.getElementById("trx").value.trim();

const msg="Shorif Topup Center BD - Order Request\n"+
"Player UID: "+uid+"\n"+
"Package: "+selected[0]+"\n"+
"Price: ৳"+selected[1]+"\n"+
"Payment: "+method+"\n"+
"Transaction ID: "+trx+"\n"+
"Please verify my payment and order.";

document.getElementById("message").value=msg;
document.getElementById("result").style.display="block";
});

function copyOrder(){
const field=document.getElementById("message");
field.select();
if(navigator.clipboard && window.isSecureContext){
navigator.clipboard.writeText(field.value).then(()=>alert("অর্ডার কপি হয়েছে।"));
}else{
document.execCommand("copy");
alert("অর্ডার কপি করার চেষ্টা করা হয়েছে।");
}
}
</script>
</body>
</html>
# shorif-topup-center-bd
