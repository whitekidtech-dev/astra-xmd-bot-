<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Astra XMD</title>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600;700&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Orbitron',sans-serif;
}

body{
    min-height:100vh;
    background:#050816;
    overflow:hidden;
    display:flex;
    align-items:center;
    justify-content:center;
    color:white;
}

body::before{
    content:'';
    position:absolute;
    width:600px;
    height:600px;
    background:radial-gradient(circle,#00f7ff33,transparent 70%);
    animation:spin 12s linear infinite;
}

@keyframes spin{
    from{transform:rotate(0deg);}
    to{transform:rotate(360deg);}
}

.container{
    position:relative;
    width:90%;
    max-width:900px;
    padding:40px;
    border:1px solid rgba(255,255,255,0.1);
    background:rgba(255,255,255,0.05);
    backdrop-filter:blur(20px);
    border-radius:30px;
    text-align:center;
    box-shadow:0 0 40px #00f7ff44;
    z-index:2;
}

.profile-img{
    width:180px;
    height:180px;
    border-radius:50%;
    object-fit:cover;
    border:4px solid #00f7ff;
    box-shadow:0 0 30px #00f7ff;
    animation:float 4s ease-in-out infinite;
}

@keyframes float{
    0%,100%{transform:translateY(0px);}
    50%{transform:translateY(-15px);}
}

h1{
    margin-top:20px;
    font-size:3rem;
    color:#00f7ff;
    text-shadow:0 0 20px #00f7ff;
}

.subtitle{
    margin-top:10px;
    color:#d0d0ff;
    font-size:1rem;
    line-height:1.8;
}

.words{
    margin-top:25px;
    display:flex;
    flex-wrap:wrap;
    gap:15px;
    justify-content:center;
}

.words span{
    padding:10px 18px;
    border-radius:30px;
    background:rgba(0,247,255,0.1);
    border:1px solid #00f7ff55;
    box-shadow:0 0 15px #00f7ff55;
    animation:glow 3s infinite alternate;
}

@keyframes glow{
    from{
        box-shadow:0 0 10px #00f7ff55;
    }
    to{
        box-shadow:0 0 25px #00f7ff;
    }
}

.links{
    margin-top:40px;
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:25px;
}

.links a{
    position:relative;
    text-decoration:none;
    color:white;
    padding:18px 35px;
    border-radius:50px;
    overflow:hidden;
    font-size:1rem;
    letter-spacing:1px;
    transition:0.4s ease;
    animation:float 3s ease-in-out infinite;
}

.links a:nth-child(1){
    background:linear-gradient(45deg,#00f7ff,#0077ff);
    box-shadow:0 0 25px #00f7ff;
}

.links a:nth-child(2){
    background:linear-gradient(45deg,#ff00ff,#7a00ff);
    box-shadow:0 0 25px #ff00ff;
}

.links a:nth-child(3){
    background:linear-gradient(45deg,#00ff99,#00cc66);
    box-shadow:0 0 25px #00ff99;
}

.links a:hover{
    transform:scale(1.1) translateY(-8px);
    filter:brightness(1.2);
}

.links a::before{
    content:'';
    position:absolute;
    top:-100%;
    left:-100%;
    width:300%;
    height:300%;
    background:rgba(255,255,255,0.15);
    transform:rotate(25deg);
    transition:0.7s;
}

.links a:hover::before{
    top:-20%;
    left:-20%;
}

.footer{
    margin-top:35px;
    color:#aaa;
    font-size:0.9rem;
}

.particles span{
    position:absolute;
    display:block;
    width:6px;
    height:6px;
    background:#00f7ff;
    border-radius:50%;
    box-shadow:0 0 10px #00f7ff;
    animation:particle 10s linear infinite;
}

@keyframes particle{
    0%{
        transform:translateY(100vh) scale(0);
        opacity:0;
    }
    50%{
        opacity:1;
    }
    100%{
        transform:translateY(-100vh) scale(1);
        opacity:0;
    }
}
</style>
</head>

<body>

<div class="particles">
    <span style="left:10%; animation-delay:0s;"></span>
    <span style="left:25%; animation-delay:2s;"></span>
    <span style="left:40%; animation-delay:4s;"></span>
    <span style="left:60%; animation-delay:1s;"></span>
    <span style="left:80%; animation-delay:3s;"></span>
    <span style="left:90%; animation-delay:5s;"></span>
</div>

<div class="container">

    <img src="https://files.catbox.moe/skf1qc.jpg" class="profile-img">

    <h1>ASTRA XMD</h1>

    <p class="subtitle">
        ⚡ Fast • Smart • Futuristic • Powerful ⚡<br>
        Your ultimate next generation Telegram bot experience.
    </p>

    <div class="words">
        <span>POWER BEYOND LIMITS</span>
        <span>CYBER FUTURE</span>
        <span>AI AUTOMATION</span>
        <span>SMART SYSTEM</span>
        <span>DIGITAL LEGEND</span>
        <span>NEON ENERGY</span>
    </div>

    <div class="links">
        <a href="https://t.me/astraxmd_bot" target="_blank">🤖 OPEN BOT</a>

        <a href="https://github.com/whitekidtech-dev/astra-xmd-bot-" target="_blank">💻 VIEW REPOSITORY</a>

        <a href="https://whitekid-ai.onrender.com/" target="_blank">🌐 OTHER PROJECT</a>
    </div>

    <div class="footer">
        ✨ Built By Whitekid Tech ✨
    </div>

</div>

</body>
</html>