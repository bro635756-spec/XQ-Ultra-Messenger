<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>XQ Messenger Ultra | XQ Studio Professional</title>
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;900&display=swap" rel="stylesheet">
    <style>
        :root {
            --xq-bg: #050608; --xq-side: #0e1117; --xq-primary: #5865f2;
            --xq-accent: #00ff9d; --xq-text: #e1e1e1; --xq-glass: rgba(255, 255, 255, 0.03);
            --xq-danger: #ff4757;
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background: var(--xq-bg); color: var(--xq-text); height: 100vh; display: flex; align-items: center; justify-content: center; overflow: hidden; }

        /* AUTH UI - MERKEZİ PANEL */
        .auth-container { width: 100%; max-width: 500px; padding: 45px; background: var(--xq-side); border-radius: 35px; border: 1px solid var(--xq-glass); text-align: center; box-shadow: 0 30px 60px rgba(0,0,0,0.6); }
        .logo-area h1 { font-weight: 900; font-size: 2.8rem; letter-spacing: -1.5px; background: linear-gradient(90deg, var(--xq-primary), var(--xq-accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
        
        .legal-scroll { 
            background: #000; height: 160px; overflow-y: auto; padding: 18px; border-radius: 18px; 
            border: 1px solid #1f232c; font-size: 0.8rem; text-align: left; margin: 25px 0; color: #8b949e; line-height: 1.6;
        }

        .xq-input { 
            width: 100%; background: #000; border: 1px solid #2d3436; color: #fff; padding: 18px; 
            border-radius: 16px; margin-bottom: 18px; outline: none; transition: 0.3s; font-size: 1rem;
        }
        .xq-input:focus { border-color: var(--xq-primary); box-shadow: 0 0 20px rgba(88, 101, 242, 0.15); }

        .btn-main { 
            width: 100%; padding: 18px; border-radius: 16px; border: none; font-weight: 800; cursor: pointer;
            transition: 0.4s; background: linear-gradient(135deg, var(--xq-primary), #a052ff); color: #fff;
        }
        .btn-main:disabled { opacity: 0.15; cursor: not-allowed; }
        .btn-main:hover:not(:disabled) { transform: translateY(-2px); box-shadow: 0 10px 20px rgba(88, 101, 242, 0.3); }

        /* APP INTERFACE */
        #appFrame { display: none; width: 100%; height: 100vh; flex-direction: column; background: #000; }
        .chat-header { padding: 20px; background: var(--xq-side); border-bottom: 1px solid var(--xq-glass); display: flex; justify-content: space-between; align-items: center; }
        .main-chat { flex: 1; display: flex; flex-direction: column; padding: 25px; overflow-y: auto; gap: 12px; background: radial-gradient(circle at top, #0c0e14 0%, #050608 100%); }
        
        .msg { padding: 14px 20px; border-radius: 22px; max-width: 75%; font-size: 0.95rem; line-height: 1.4; position: relative; animation: slideIn 0.3s ease-out; }
        .msg-me { align-self: flex-end; background: var(--xq-primary); color: #fff; border-bottom-right-radius: 4px; }
        .msg-other { align-self: flex-start; background: var(--xq-side); border: 1px solid var(--xq-glass); border-bottom-left-radius: 4px; }

        .input-bar { padding: 25px; background: var(--xq-side); display: flex; gap: 15px; border-top: 1px solid var(--xq-glass); }
        
        @keyframes slideIn { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }
    </style>
</head>
<body>

    <div class="auth-container" id="authBox">
        <div class="logo-area"><h1>XQ ULTRA</h1><p style="color: #636e72;">Secure Messenger v6.0</p></div>
        <div class="legal-scroll">
            <b>TCK & ANAYASAL DENETİM BİLDİRİMİ:</b><br><br>
            Bu uygulama <b>XQ Studio</b> tarafından siber güvenlik standartlarında korunmaktadır.
            TCK 312 ve 216. maddeler uyarınca; suça teşvik, darbe propagandası ve taciz içerikli mesajlar Astrix Denetim Motoru tarafından anlık olarak taranır.
            Tüm ihlaller kimlik bilgileriyle beraber <b>bro635756@gmail.com</b> adresine siber rapor olarak iletilir.
        </div>
        <label style="display:flex; align-items:center; gap:10px; margin-bottom:20px; cursor:pointer;">
            <input type="checkbox" id="legalCheck" style="width:20px; height:20px;"> Şartları kabul ediyorum.
        </label>
        <input type="email" id="userEmail" class="xq-input" placeholder="E-posta Adresiniz">
        <button class="btn-main" id="otpBtn" disabled onclick="triggerOTP()">9 HANELİ KODU GÖNDER</button>
        
        <div id="verifyArea" style="display:none; margin-top:20px;">
            <input type="number" id="otpInput" class="xq-input" placeholder="Kodu Buraya Girin">
            <button class="btn-main" onclick="finalizeAuth()" style="background: var(--xq-accent); color: #000;">SİSTEME GİRİŞ YAP</button>
        </div>
    </div>

    <div id="appFrame">
        <div class="chat-header">
            <span style="font-weight:700; color:var(--xq-accent);">● XQ SİBER DENETÇİ AKTİF</span>
            <span id="userTag" style="font-size:0.8rem; opacity:0.7;"></span>
        </div>
        <div class="main-chat" id="chatBox"></div>
        <div class="input-bar">
            <input type="text" id="chatInput" class="xq-input" style="margin:0" placeholder="Mesajınızı yazın (Siber Denetçi devrede...)">
            <button class="btn-main" style="width:130px;" onclick="sendMessage()">GÖNDER</button>
        </div>
    </div>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/12.12.0/firebase-app.js";
        import { getDatabase, ref, push, onValue, serverTimestamp } from "https://www.gstatic.com/firebasejs/12.12.0/firebase-database.js";

        // FIREBASE ENTEGRASYONU
        const firebaseConfig = { 
            apiKey: "AIzaSyBQdsC8VuoBnFyOLWavV3C8GXomSzDXUzw", 
            databaseURL: "https://des-store-c93e0-default-rtdb.europe-west1.firebasedatabase.app" 
        };
        const app = initializeApp(firebaseConfig);
        const db = getDatabase(app);

        // API ANAHTARLARI
        const RESEND_KEY = "re_29BPLbT4_CA6DrRuvHfAK2f7XJgiarAfR";
        const SPOTIFY_ID = "1a5def3fab8142a79a1d48cd7c260751";
        let generatedOTP = "";
        let activeUser = "";

        document.getElementById('legalCheck').onchange = (e) => document.getElementById('otpBtn').disabled = !e.target.checked;

        // RESEND MAIL MOTORU
        window.triggerOTP = async () => {
            activeUser = document.getElementById('userEmail').value;
            generatedOTP = Math.floor(100000000 + Math.random() * 900000000).toString();
            
            try {
                const response = await fetch('https://api.resend.com/emails', {
                    method: 'POST',
                    headers: { 'Authorization': `Bearer ${RESEND_KEY}`, 'Content-Type': 'application/json' },
                    body: JSON.stringify({
                        from: 'XQ-Security <onboarding@resend.dev>',
                        to: [activeUser],
                        subject: 'XQ Ultra Güvenlik Doğrulaması',
                        html: `Giriş Kodunuz: <h1 style="color:#5865f2">${generatedOTP}</h1>`
                    })
                });
                if(response.ok) {
                    document.getElementById('verifyArea').style.display = 'block';
                    alert("9 haneli güvenlik kodu mailine gönderildi, Burak.");
                } else { throw new Error(); }
            } catch (e) { alert("Hata: Firebase/Resend domain izni eksik!"); }
        };

        window.finalizeAuth = () => {
            if(document.getElementById('otpInput').value === generatedOTP) {
                document.getElementById('authBox').style.display = 'none';
                document.getElementById('appFrame').style.display = 'flex';
                document.getElementById('userTag').innerText = activeUser;
                startXQSync();
            } else { alert("Hatalı kod! Erişim engellendi."); }
        };

        // ASTRIX SİBER DENETİM MOTORU
        async function cyberAudit(text) {
            const dangerWords = ["terör", "darbe", "saldırı", "taciz", "suikast", "bomba"];
            const check = dangerWords.some(w => text.toLowerCase().includes(w));

            if(check) {
                await fetch('https://api.resend.com/emails', {
                    method: 'POST',
                    headers: { 'Authorization': `Bearer ${RESEND_KEY}`, 'Content-Type': 'application/json' },
                    body: JSON.stringify({
                        from: 'SiberDenetci@resend.dev',
                        to: ['bro635756@gmail.com'],
                        subject: '🚨 XQ GÜVENLİK İHLALİ',
                        html: `<b>Kullanıcı:</b> ${activeUser}<br><b>İhlal Mesajı:</b> ${text}`
                    })
                });
            }
        }

        window.sendMessage = () => {
            const msgInput = document.getElementById('chatInput');
            const msgText = msgInput.value.trim();
            if(!msgText) return;

            cyberAudit(msgText);
            push(ref(db, 'messages'), {
                user: activeUser,
                content: msgText,
                timestamp: serverTimestamp()
            });
            msgInput.value = "";
        };

        function startXQSync() {
            onValue(ref(db, 'messages'), (snapshot) => {
                const box = document.getElementById('chatBox');
                box.innerHTML = "";
                snapshot.forEach(child => {
                    const data = child.val();
                    const div = document.createElement('div');
                    div.className = `msg ${data.user === activeUser ? 'msg-me' : 'msg-other'}`;
                    div.innerHTML = `<small style="display:block; font-size:0.6rem; opacity:0.6;">${data.user}</small>${data.content}`;
                    box.appendChild(div);
                });
                box.scrollTop = box.scrollHeight;
            });
        }
    </script>
</body>
</html>
