<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>PK TOP UP</title>

<style>
body{
    margin:0;
    font-family:Arial,sans-serif;
    background:#f4f6fb;
    color:#172033;
}

header{
    background:#151a2d;
    color:white;
    text-align:center;
    padding:25px;
}

.logo{
    font-size:30px;
    font-weight:bold;
}

.diamond{
    font-size:45px;
}

.card{
    background:white;
    margin:18px;
    padding:20px;
    border-radius:16px;
    box-shadow:0 4px 15px #0002;
}

label{
    display:block;
    margin-top:15px;
    margin-bottom:7px;
    font-weight:bold;
}

input,select,button{
    width:100%;
    padding:14px;
    box-sizing:border-box;
    border-radius:10px;
    font-size:16px;
}

input,select{
    border:1px solid #ccd2df;
}

button{
    margin-top:20px;
    border:0;
    background:#151a2d;
    color:white;
    font-weight:bold;
}

#message{
    margin-top:15px;
    font-weight:bold;
}
</style>
</head>

<body>

<header>
    <div class="diamond">💎</div>
    <div class="logo">PK TOP UP</div>
    <p>Fast & Simple Top Up</p>
</header>

<div class="card">

<h2>💎 Free Fire Diamond</h2>

<label>Player ID</label>
<input
    type="text"
    id="playerID"
    placeholder="আপনার Player ID লিখুন"
>

<label>Diamond Package</label>

<select id="package">
    <option>25 Diamonds — ৳25</option>
    <option>50 Diamonds — ৳45</option>
    <option>115 Diamonds — ৳90</option>
    <option>240 Diamonds — ৳180</option>
</select>

<label>Payment Method</label>

<select id="payment">
    <option>bKash</option>
    <option>Nagad</option>
</select>

<button onclick="topup()">
    TOP UP NOW
</button>

<div id="message"></div>

</div>

<script>

function topup(){

    let id =
    document.getElementById("playerID").value.trim();

    let pack =
    document.getElementById("package").value;

    let payment =
    document.getElementById("payment").value;

    let message =
    document.getElementById("message");

    if(id === ""){
        message.innerHTML =
        "❌ আগে Player ID দিন।";
        return;
    }

    message.innerHTML =
    "✅ অর্ডার প্রস্তুত!<br><br>" +
    "Player ID: " + id + "<br>" +
    "Package: " + pack + "<br>" +
    "Payment: " + payment;

}

</script>

</body>
</html># Acode Plugin Docs

A development guide for Acode plugins, fully updated with comprehensive documentation and examples for all the latest APIs.

## Contribution

Want to help improve these docs? Simply open an issue describing what you'd like to add. This helps avoid conflicts and ensures smooth collaboration between contributors.
