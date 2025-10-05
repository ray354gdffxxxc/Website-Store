<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Rayyan Store - Demo</title>
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@300;700&family=Montserrat:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#ffffff;
      --nav-bg:#424141;
      --accent-start:#ff5a5f;
      --accent-end:#f14ea0;
      --card-shadow: 0 6px 18px rgba(0,0,0,0.08);
    }
    *{box-sizing:border-box}
    html,body{height:100%;}
    body{
      margin:0;
      font-family: "Montserrat", sans-serif;
      background:var(--bg);
      color:#222;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      scroll-behavior:smooth;
    }

    /* Header / Nav */
    .header{
      background:var(--nav-bg);
      color:white;
      padding:18px 20px;
      display:flex;
      align-items:center;
      gap:20px;
      border-bottom-left-radius:18px;
      border-bottom-right-radius:18px;
      position:sticky;
      top:0;
      z-index:20;
    }
    .logo{
      font-family: "Merriweather", serif;
      font-weight:700;
      font-size:28px;
      letter-spacing:1px;
    }
    nav{
      margin-left:auto;
    }
    nav a{
      color:rgba(255,255,255,0.9);
      text-decoration:none;
      margin-left:18px;
      font-size:18px;
      font-weight:500;
    }
    nav a:hover{opacity:0.85}

    main{padding:26px; max-width:920px; margin:0 auto;}

    /* Buttons like Instagram sample */
    .link-btn{
      display:block;
      width:100%;
      max-width:820px;
      margin:18px auto;
      padding:18px 24px;
      text-align:center;
      font-family:"Merriweather", serif;
      font-size:44px;
      color:white;
      border-radius:18px;
      background: linear-gradient(90deg, var(--accent-start) 0%, var(--accent-end) 100%);
      text-decoration:none;
      box-shadow: 0 8px 20px rgba(241,78,160,0.15);
      transition: transform .13s ease, box-shadow .13s ease;
    }
    .link-btn:active{transform:translateY(2px)}
    .link-btn:hover{box-shadow: 0 12px 28px rgba(241,78,160,0.2)}

    /* Products */
    .products{
      margin-top:14px;
      display:grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap:18px;
    }
    .card{
      background:white;
      border-radius:12px;
      padding:12px;
      box-shadow:var(--card-shadow);
      display:flex;
      flex-direction:column;
      gap:8px;
      align-items:center;
    }
    .card img{
      width:100%;
      height:150px;
      object-fit:cover;
      border-radius:8px;
    }
    .card h3{
      margin:6px 0 0;
      font-size:18px;
    }
    .card p{margin:0;color:#666;font-size:14px}
    .buy{
      margin-top:8px;
      width:100%;
      text-align:center;
      padding:10px;
      border-radius:10px;
      background: linear-gradient(90deg, #ff8364 0%, #ff5a99 100%);
      color:white;
      font-weight:600;
      text-decoration:none;
      display:inline-block;
      box-shadow:0 6px 16px rgba(255,90,153,0.12);
    }

    /* About section */
    .about{
      margin-top:36px;
      background:#fff9fb;
      padding:18px;
      border-radius:12px;
      box-shadow:var(--card-shadow);
    }
    .socials{
      display:flex;
      gap:12px;
      flex-wrap:wrap;
      margin-top:8px;
    }
    .socials a{
      flex:1 1 180px;
      text-decoration:none;
      padding:12px;
      border-radius:12px;
      background:linear-gradient(90deg, var(--accent-start) 0%, var(--accent-end) 100%);
      color:white;
      text-align:center;
      font-weight:600;
      box-shadow:0 8px 18px rgba(0,0,0,0.06);
    }

    footer{
      margin:28px auto 60px;
      text-align:center;
      color:#666;
      font-size:14px;
    }

    /* Responsive tweaks */
    @media (max-width:520px){
      .link-btn{font-size:36px; padding:16px}
      nav a{font-size:16px}
      .card img{height:140px}
    }
  </style>
</head>
<body>

  <header class="header">
    <div class="logo">Rayyan Store<br><small style="font-size:12px;opacity:.9"></small></div>
    <nav>
      <a href="#pproduk">Produk</a>
      <a href="#tentang">Tentang</a>
    </nav>
  </header>

  <main>
    <!-- Large gradient buttons (mirip gambar contoh) -->
      <footer>Di Clik Otomatis Beralih ke:</footer>
      <section id="pproduk" aria-label="Produk" style="margin-top:28px">
      <a class="link-btn" href="https://s.shopee.co.id/9fC1yQglQb" target="_blank" rel="noopener noreferrer">Followers Ig</a>
      <a class="link-btn" href="https://s.shopee.co.id/40XfE4eW28" target="_blank" rel="noopener noreferrer">Like Ig</a>
      <a class="link-btn" href="https://s.shopee.co.id/4fnM1PDQX1" target="_blank" rel="noopener noreferrer">View Ig</a>
      <a class="link-btn" href="https://s.shopee.co.id/gHDGCkwru" target="_blank" rel="noopener noreferrer">Like & View Ig</a>
      <a class="link-btn" href="https://s.shopee.co.id/4LAVd72d4p" target="_blank" rel="noopener noreferrer">View Story Ig</a>
      <a class="link-btn" href="https://s.shopee.co.id/4VTvpgd7HJ" target="_blank" rel="noopener noreferrer">View++ Ig</a>
    </section>

    <!-- Produk -->
    <!-- Tentang Kami -->
    <section id="tentang" class="about" aria-label="Tentang Kami">
      <h2 style="font-family:'Merriweather', serif; font-weight:700; font-size:22px; margin:0"></h2>
      <p style="margin-top:8px">Halo! Kami Rayyan Store. Hubungi kami lewat salah satu media sosial di bawah ini:</p>

      <div class="socials">
        <!-- WhatsApp: ganti nomor dengan format internasional tanpa +, contoh: 6281234567890 -->
        <a href="https://wa.me/6289517737408?text=Halo%20Rayyan%20Store%2C%20saya%20ingin%20memesan" target="_blank" rel="noopener noreferrer">WhatsApp</a>

        <!-- Instagram: ganti yourusername -->
        <a href="https://www.instagram.com/ryhn_1bs?igsh=YmhvbjV4d2p0Nm16" target="_blank" rel="noopener noreferrer">Instagram</a>

        <!-- TikTok: ganti @yourusername (atau path sesuai akun) -->
        <a href="https://www.tiktok.com/@yourusername" target="_blank" rel="noopener noreferrer">TikTok</a>
      </div>
    </section>

    <footer>
      © <span id="year"></span> Rayyan Store
    </footer>
  </main>

  <script>
    // set tahun di footer
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
