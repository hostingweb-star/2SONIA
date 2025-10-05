<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Blog Galaxy — Profil & 4 Post Tes</title>
  <style>
    :root{
      --bg-deep:#b24281;
      --bg-mid:#07112a;
      --accent:#b24281;
      --accent-2:#b9d2ff;
      --muted:#b8c9e8;
      --card:#081226;
      --glass: rgba(255,255,255,0.04);
      --radius:16px;
      --maxw:920px;
      --gap:20px;
    }
    *{box-sizing:border-box;margin:0;padding:0}
    body{
      font-family: 'Poppins', sans-serif;
      background: radial-gradient(circle at top left, rgba(110,168,255,0.08), transparent 40%),
                  radial-gradient(circle at bottom right, rgba(255,142,192,0.05), transparent 40%),
                  linear-gradient(180deg,var(--bg-mid),var(--bg-deep));
      color:#eef6ff;
      padding:32px 20px;
      display:flex;justify-content:center;
    }
    .wrap{width:100%;max-width:var(--maxw)}

    header{
      display:flex;align-items:center;gap:18px;
      background:linear-gradient(135deg, rgba(255,255,255,0.06), rgba(255,255,255,0.01));
      padding:22px;border-radius:20px;border:1px solid var(--glass);
      box-shadow:0 10px 40px rgba(3,7,20,0.7), 0 0 60px rgba(110,168,255,0.15);
      backdrop-filter: blur(12px);
    }
    .avatar{width:110px;height:110px;border-radius:16px;overflow:hidden;border:3px solid rgba(110,168,255,0.3);flex:0 0 110px;box-shadow:0 0 20px rgba(110,168,255,0.2)}
    .avatar img{width:100%;height:100%;object-fit:cover;display:block}
    .meta{flex:1}
    .meta h1{font-size:24px;margin-bottom:6px;color:var(--accent)}
    .meta p{color:var(--muted);font-size:15px;margin-bottom:12px}
    .meta .tags{display:flex;gap:10px;flex-wrap:wrap}
    .tag{background:linear-gradient(90deg, rgba(110,168,255,0.1), rgba(154,208,255,0.05));padding:6px 12px;border-radius:999px;font-size:13px;color:var(--muted);border:1px solid rgba(255,255,255,0.05)}

    .hero {text-align: center;margin-top: 20px;}
    .hero iframe {
      width: 100%;
      max-width: 720px;
      height: 405px;
      border-radius: 12px;
      border: none;
      box-shadow: var(--card-shadow);
    }
    main{margin-top:var(--gap)}
    .grid{display:grid;grid-template-columns:repeat(2,1fr);gap:20px;margin-top:14px}
    .card{
      background:linear-gradient(160deg, rgba(255,255,255,0.04), rgba(255,255,255,0.015));
      border-radius:var(--radius);
      padding:18px;
      border:1px solid var(--glass);
      min-height:160px;
      position:relative;
      overflow:hidden;
      box-shadow:0 8px 28px rgba(3,7,20,0.6), inset 0 0 40px rgba(110,168,255,0.04);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .card:hover{transform:translateY(-6px);box-shadow:0 12px 40px rgba(3,7,20,0.7), 0 0 50px rgba(110,168,255,0.2)}
    .card h3{font-size:17px;margin-bottom:8px;color:var(--accent)}
    .card p{color:rgb(255, 255, 255);font-size:14px;line-height:1.5}
    .num{position:absolute;right:14px;top:14px;font-size:13px;color:rgba(255,255,255,0.1);font-weight:700}

    @media (max-width:860px){
      .grid{grid-template-columns:1fr}
      header{flex-direction:column;align-items:center;text-align:center}
    }

    footer{margin-top:24px;text-align:center;color:var(--muted);font-size:13px}
    footer a{color:#b9d2ff;text-decoration:none;font-weight:600}
    footer a:hover{text-decoration:underline}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="avatar">
        <img src="image2.jpg" alt="Foto Pembuat">
      </div>
      <div class="meta">
        <h1>SONIA KEMALA PUTRI</h1>
        <p>Mahasiswa Teknik Informatika UBP Karawang</p>
        <div class="tags">
          <div class="tag">NIM : 24416255201103</div>
          <div class="tag">if24.soniaputri@mhs.ubpkarawang.ac.id</div>
          <div class="tag">Basis Data</div>
        </div>
      </div>
    </header>

      <div class="hero">
    <iframe src="https://www.youtube.com/embed/lI3t8a3YoVQ?si=TqQirVeOWTC6CoiA" 
      title="YouTube video" allowfullscreen></iframe>
  </div>

    <main id="posts">
      <div class="grid">
        <article class="card">
          <h3>Post 2: Apa itu Attribute, Entitas, dan Relasi dalam ERD?</h3>
          <p>Dalam <em>Entity Relationship Diagram (ERD)</em>, ada tiga komponen utama yang digunakan untuk memodelkan data:</p>
      <ul>
        <li><strong>Atribut (Attribute)</strong> → Atribut adalah ciri atau informasi yang dimiliki entitas.  
          <br>Contoh:</li>
          <p>Produk → <strong>ID Produk, Nama Produk, Harga, Stok</strong></p> 
          <p>Pelanggan → <strong>Pelanggan, Nama, Email, Alamat</strong></p>
          <p>Pesanan → <strong>Pesanan, Tanggal Pesan, Total Harga</strong></p> 
        <li><strong>Entitas (Entity)</strong> → Entitas adalah objek nyata atau konsep yang datanya ingin disimpan.  
          <br>Contoh di toko online : <em>Produk, Pelanggan, Pesanan.</em>.</li>
          <p>Produk = barang yang dijual.</p> 
          <p>Pelanggan = orang yang membeli.</p> 
          <p>Pesanan = transaksi pembelian.</p>
        <li><strong>Relasi (Relationship)</strong> → Relasi adalah hubungan antar entitas.  
          <br>Contoh:</li>
          <p>Pelanggan membuat Pesanan</p> 
          <p>Pesanan berisi Produk</p> 
      </ul>
        </article>
      </div>

      <footer>
      © 2025 Blog Basis Data | <a href="https://www.ubpkarawang.ac.id" target="_blank">UBP Karawang</a></p>
      </footer>
    </main>
  </div>
</body>
</html>
