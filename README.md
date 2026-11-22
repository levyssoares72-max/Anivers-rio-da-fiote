# Anivers-rio-da-fiote
Feliz aniversário!!!
<!DOCTYPE html>
 <html>
 <head>
     <title>🎉 Feliz Aniversário!</title>
     <style>
         body {
             background: linear-gradient(45deg, #ff9a9e, #fad0c4, #ffecd2);
             font-family: Arial, sans-serif;
             text-align: center;
             padding-top: 50px;
         }
         h1 {
             color: #e63946;
             font-size: 45px;
             animation: pulse 1.5s infinite;
         }
         @keyframes pulse {
             0% { transform: scale(1); }
             50% { transform: scale(1.1); }
             100% { transform: scale(1); }
         }
         .coracao {
             font-size: 80px;
             margin: 30px;
         }
         .mensagem {
             font-size: 22px;
             color: #2b2d42;
             max-width: 500px;
             margin: 0 auto;
             line-height: 1.6;
         }
         .confete {
             position: fixed;
             width: 10px;
             height: 10px;
             opacity: 0;
             animation: cair 5s ease-in infinite;
         }
         @keyframes cair {
             0% { transform: translateY(-100px); opacity: 1; }
             100% { transform: translateY(100vh); opacity: 0; }
         }
     </style>
 </head>
 <body>
     <h1>🎉 Feliz Aniversário! 🎂</h1>
     <div class="coracao">💖🎈🎁</div>
     
     <div class="mensagem">
         <p>Parabéns, minha amiga! 🥳</p>
         <p>Que seu dia seja tão especial quanto você.</p>
         <p>Que a vida te traga muitas alegrias, amor e sucesso! ✨</p>
         <p>Você merece tudo de bom! 🌟</p>
     </div>
     <script>
         const cores = ['#ff6b6b','#ffd93d','#6bcb77','#4d96ff','#ff6b9d'];
         setInterval(() => {
             const confete = document.createElement('div');
             confete.classList.add('confete');
             confete.style.left = Math.random() * 100 + 'vw';
             confete.style.backgroundColor = cores[Math.floor(Math.random() * cores.length)];
             confete.style.animationDuration = (Math.random() * 3 + 2) + 's';
             document.body.appendChild(confete);
             setTimeout(() => confete.remove(), 5000);
         }, 300);
     </script>
 </body>
 </html>
