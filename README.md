<head>
  
  <style>
    body {
      margin: 0;
      font-family: 'Open Sans', sans-serif;
      background-color: #000;
      color: #fff;
    }
    header {
      background-color: rgb(0, 0, 0);
      color: rgb(1, 204, 255, 0.7);
      padding: 1rem 2rem;
      position: sticky;
      top: 0;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 1000;
      box-shadow: 0 2px 5px rgba(212, 175, 55, 0.2);
    }
    nav a {
      color: white;
      margin-left: 1.5rem;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover {
      color: rgb(1, 204, 255, 0.7);
    }
    h1, h2, h3 {
      font-family: 'Playfair Display', serif;
    }
    section {
      padding: 4rem 2rem;
    }
.hero {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 450px;
    padding: 5rem 4vw 5rem 4vw;
    background: 
      linear-gradient(90deg, rgba(1, 204, 255, 0.7) 0%, rgb(0, 0, 0) 100%),
      url('p.jpg') right center/cover no-repeat;
    position: relative;
    overflow: hidden;
    box-shadow: 0 8px 32px rgba(0,0,0,0.25);
    text-align: center;
  }
  
.hero-content h2 {
    font-size: 3.5rem;
    background: linear-gradient(270deg, #000000, #fffbe6,rgb(1, 204, 255, 0.7), #000000);
    background-size: 800% 800%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    color: transparent;
    animation: gradientmove 4s linear infinite;
    text-shadow: 0 2px 12px rgba(0,0,0,0.28);
    font-weight: bold;
}
  @keyframes gradientmove {
    0% {background-position:0% 50%;}
    100% {background-position:100% 50%;}
  }
  .hero-content p {
    font-size: 1.5rem;
    background: linear-gradient(270deg, rgb(1, 204, 255, 0.7), #000000, rgb(1, 204, 255, 0.7), #fffefe);
    background-size: 800% 800%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    color: transparent;
    animation: gradientmove 4s linear infinite;
    text-shadow: 0 2px 12px rgba(0,0,0,0.28);
    font-weight: bold;
  }
  .hero-image {
    display: none;
  }
  @media (max-width: 900px) {
    .hero {
      padding: 3rem 2vw 3rem 2vw;
      background: 
        linear-gradient(to bottom, rgba(1, 153, 254, 0.7) 0%, rgba(0,0,0,0.7) 100%),
        url('p.jpg') center center/cover no-repeat;
      border-radius: 0 0 24px 24px;
      flex-direction: column;
      text-align: center;
    }
    .hero-content {
      padding: 1.5rem 1rem;
      max-width: 100%;
    }
  }
  section#produk {
  background-image: url('ombak.gif');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
  .produk-grid {
  display: flex;
  flex-direction: column;
  gap: 2.5rem;
  align-items: center;
 
}
.produk-kiri {
  display: flex;
  align-items: center;
  background-color: #1a1a1a;
  border: 1px solid linear-gradient(270deg, #d4af37, #000000, #d4af37, #fffefe);
  animation: alternate 3s infinite alternate;
  padding: 1.5rem 2rem;
  width: 900px;
  border-radius: 16px;
  box-shadow: 0 4px 24px rgba(212,175,55,0.08);
  transition: transform 0.3s;
  margin: 0 auto;
  justify-content: center;
  border-left: 20px solid rgba(1, 153, 254, 0.7) ;
  border-bottom:20px solid rgba(1, 153, 254, 0.7);
  border-style:groove
}
.produk-kanan{
  display: flex;
  align-items: center;
  background-color: #1a1a1a;
  border: 1px solid linear-gradient(270deg, #d4af37, #000000, #d4af37, #fffefe);
  animation: alternate 3s infinite alternate;
  padding: 1.5rem 2rem;
  width: 900px;
  border-radius: 16px;
  box-shadow: 0 4px 24px rgba(212,175,55,0.08);
  transition: transform 0.3s;
  margin: 0 auto;
  justify-content: center;
  border-right: 20px solid rgba(1, 153, 254, 0.7) ;
  border-bottom:20px solid rgba(1, 153, 254, 0.7) ;
  border-style:groove
}
.produk:hover {
  transform: translateY(-5px) scale(1.02);
}
.produk-img {
  width: 120px;
  height: 150px;
  object-fit: cover;
  border-radius: 12px;
  margin: 0 2rem;
  background: #222;
  box-shadow: 0 2px 12px rgba(212,175,55,0.12);
}
.produk-notes {
  flex: 1;
  color: #fff;
  text-align: left;
}
.produk h3 {
  color: #d4af37;
  margin-bottom: 0.5rem;
}
.produk p {
  margin: 0.3rem 0;
  font-size: 1rem;
}
@media (max-width: 900px) {
  .produk {
    flex-direction: column;
    width: 98vw;
    padding: 1.2rem 0.5rem;
  }
  .produk-img {
    margin: 0 0 1rem 0;
    width: 90vw;
    height: 180px;
    max-width: 320px;
    object-fit: cover;
  }
  .produk-notes {
    text-align: center;
  }
}

    section#about {
      background-color: #111;
      padding: 3rem 0 0 0;
      text-align: center;
    }
    section#about p {
      max-width: 800px;
      margin: 0 auto;
      font-size: 1.2rem;
      line-height: 1.6;
    }
     .footer-fullwidth {
      width: 100vw;
      position: relative;
      left: 50%;
      right: 50%;
      margin-left: -50vw;
      margin-right: -50vw;
      background: #0a1a3a;
      color: #fff;
      padding: 3rem 2rem 2rem 2rem;
      margin-top: 3rem;
    }
  </style>
</head>
<body>

<header>
  <h1>Fragrance World</h1>
  <nav>
    <a href="#home">Home</a>
    <a href="#produk">Produk</a>
    <a href="#about">About</a>
  </nav>
</header>

<section id="home" class="hero">
  <div class="hero-content">
    <h2>Selamat datang di dunia aroma elegan</h2>
    <p>Temukan parfum yang mencerminkan kepribadianmu</p>
  </div>
  <div class="hero-image">
    <img src="p.jpg" alt="Parfum Elegan">
  </div>
</section>

<section id="produk">
 <h1 style="text-align:center; font-size: 54px; font-weight: bold; letter-spacing:2px ;" >
    <b>Produk Unggulan</b>
  </h1>
  <div class="produk-grid">
    <div class="produk-kiri">
      <img class="produk-img" src="blue point.jpg" alt="BSP Blue Point">
      <div class="produk-notes">
        <h3>BSP Blue Point</h3>
        <p><strong>Top Notes:</strong> Citrus, Fruity, Oceanic</p>
        <p><strong>Middle Notes:</strong> Floral, Spicy, Marine</p>
        <p><strong>Base Notes:</strong> Musk, Woody</p>
        <p><strong>Harga:</strong> Rp 225.000</p>
      </div>
    </div>
    <div class="produk-kanan">
      <div class="produk-notes">
        <h3>LV Imagination</h3>
        <p><strong>Top Notes:</strong> Calabrian Bergamot, Sicilian Orange, Nigerian Ginger</p>
        <p><strong>Middle Notes:</strong> Tunisian Neroli, Ceylon Cinnamon, Black Tea</p>
        <p><strong>Base Notes:</strong> Ambrox, Gaiac Wood</p>
        <p><strong>Harga:</strong> Rp 7.750.000</p>
      </div>
      <img class="produk-img" src="lvimagination.jpg" alt="LV Imagination">
    </div>
    <div class="produk-kiri">
      <img class="produk-img" src="blue.jpg" alt="Mykonos California Blue">
      <div class="produk-notes">
        <h3>Mykonos California Blue</h3>
        <p><strong>Top Notes:</strong> Lavender, Pear, Grapefruit, Pink Salt</p>
        <p><strong>Middle Notes:</strong> Rhubarb, Water Blossoms, Marine Notes</p>
        <p><strong>Base Notes:</strong> Moss, Softwood, Caramel</p>
        <p><strong>Harga:</strong> Rp 229.000</p>
      </div>
    </div>
    <div class="produk-kanan">
      <div class="produk-notes">
        <h3>Versace Eros</h3>
        <p><strong>Top Notes:</strong> Mint, Green Apple, Lemon</p>
        <p><strong>Middle Notes:</strong> Tonka Bean, Geranium, Ambroxan</p>
        <p><strong>Base Notes:</strong> Vanilla, Vetiver, Oakmoss, Cedar</p>
        <p><strong>Harga:</strong> Rp 1.350.000</p>
      </div>
      <img class="produk-img" src="eros.jpg" alt="Versace Eros">
    </div>
    <div class="produk-kiri">
      <img class="produk-img" src="ice.jpg" alt="Rasasi Hawas Ice">
      <div class="produk-notes">
        <h3>Rasasi Hawas Ice</h3>
        <p><strong>Top Notes:</strong> Bergamot, Lemon, Apple</p>
        <p><strong>Middle Notes:</strong> Cardamom, Orange Blossom, Plum</p>
        <p><strong>Base Notes:</strong> Ambergris, Musk, Patchouli</p>
        <p><strong>Harga:</strong> Rp 950.000</p>
      </div>
    </div>
    <div class="produk-kanan">
      <div class="produk-notes">
        <h3>Blue Seduction</h3>
        <p><strong>Top Notes:</strong> Bergamot, Melon, Mint, Black Currant</p>
        <p><strong>Middle Notes:</strong> Ocean Accord, Cardamom, Nutmeg, Cappuccino</p>
        <p><strong>Base Notes:</strong> Amber, Musk, Woodsy Notes</p>
        <p><strong>Harga:</strong> Rp 450.000</p>
      </div>
      <img class="produk-img" src="seduction.jpg" alt="Blue Seduction">
    </div>
    <div class="produk-kiri">
      <img class="produk-img" src="nautica.jpg" alt="Nautica Voyage">
      <div class="produk-notes">
        <h3>Nautica Voyage</h3>
        <p><strong>Top Notes:</strong> Green Leaves, Apple</p>
        <p><strong>Middle Notes:</strong> Lotus, Mimosa</p>
        <p><strong>Base Notes:</strong> Musk, Cedar, Oakmoss, Amber</p>
        <p><strong>Harga:</strong> Rp 350.000</p>
      </div>
    </div>
  </div>
</section>
<section id="about" style="background:#111; padding:4rem 0 0 0;">
  <div style="max-width:800px; margin:0 auto 3rem auto; text-align:center;">
    <h1 style="color:#01ccff; margin-bottom:1.5rem;">Mengapa Memilih Kami?</h1>
    <p style="color:#fff; font-size:1.2rem; line-height:1.7;">
      Kami percaya setiap aroma adalah bagian dari cerita hidup.  
      <br><br>
      Pilihan parfum kami dikurasi untuk berbagai kepribadian dan suasana hati, mulai dari aroma segar, maskulin, feminin, hingga eksotis.  
      <br><br>
      Nikmati pengalaman belanja parfum yang mudah, aman, dan penuh inspirasi.  
      <br><br>
      Temukan aroma favoritmu dan ekspresikan dirimu setiap hari!
    </p>
  </div>
  <div class="footer-fullwidth">
    <div style="max-width:1200px; margin:auto;">
      <h2 style="font-size:2rem; margin-bottom:0.5rem;">Subscribe to our newsletter</h2>
      <p style="margin-bottom:1.5rem; color:#cfd8e3;">Dapatkan info parfum terbaru, promo, dan tips eksklusif langsung ke email Anda.</p>
      <form style="display:flex; gap:1rem; max-width:500px; margin-bottom:1.5rem;">
        <input type="email" placeholder="Masukkan email Anda" style="flex:1; padding:0.7rem 1rem; border-radius:6px; border:none; font-size:1rem;">
        <button type="submit" style="background:#01ccff; color:#111; border:none; border-radius:6px; padding:0.7rem 2rem; font-size:1rem; font-weight:bold; cursor:pointer;">Subscribe</button>
      </form>
      <p style="font-size:0.9rem; color:#b0b8c1; max-width:500px; margin-bottom:2.5rem;">
        Dengan berlangganan, Anda setuju menerima email promosi. Anda dapat berhenti berlangganan kapan saja.
      </p>
      <hr style="border:0; border-top:1px solid #22305a; margin-bottom:2rem;">
      <div style="display:flex; flex-wrap:wrap; gap:2rem; justify-content:space-between;">
        <div style="flex:1; min-width:180px;">
          <div style="font-weight:bold; font-size:1.2rem; margin-bottom:0.7rem;">Nilai Kami</div>
          <div style="color:#b0b8c1;">Kualitas, keaslian, dan pelayanan terbaik untuk setiap pelanggan.</div>
        </div>
        <div style="flex:1; min-width:180px;">
          <div style="font-weight:bold; margin-bottom:0.7rem;">Menu</div>
          <div style="color:#b0b8c1;">
            <a href="#home" style="color:#b0b8c1; text-decoration:none;">Home</a><br>
            <a href="#produk" style="color:#b0b8c1; text-decoration:none;">Produk</a><br>
            <a href="#about" style="color:#b0b8c1; text-decoration:none;">About</a>
          </div>
        </div>
        <div style="flex:1; min-width:180px;">
          <div style="font-weight:bold; margin-bottom:0.7rem;">Layanan</div>
          <div style="color:#b0b8c1;">
            Konsultasi Parfum<br>
            Gift Wrapping<br>
            Pengiriman Seluruh Indonesia<br>
            Membership & Promo
          </div>
        </div>
        <div style="flex:1; min-width:180px;">
          <div style="font-weight:bold; margin-bottom:0.7rem;">Kontak</div>
          <div style="color:#b0b8c1;">
            Email: info@fragranceworld.com<br>
            WhatsApp: 0812-3456-7890<br>
            Instagram: @fragranceworld.id<br>
          </div>
        </div>
      </div>
      <hr style="border:0; border-top:1px solid #22305a; margin:2rem 0 1rem 0;">
      <div style="display:flex; justify-content:space-between; align-items:center; flex-wrap:wrap;">
        <div style="color:#b0b8c1;">©2025 Fragrance World - All rights reserved.</div>
        <div>
          <a href="#" style="margin-left:1rem; color:#b0b8c1; font-size:1.3rem; text-decoration:none;">&#x1F4F7;</a>
          <a href="#" style="margin-left:1rem; color:#b0b8c1; font-size:1.3rem; text-decoration:none;">&#x1F4F1;</a>
          <a href="#" style="margin-left:1rem; color:#b0b8c1; font-size:1.3rem; text-decoration:none;">&#x1F4E7;</a>
        </div>
      </div>
    </div>
  </div>
  <div style="text-align:center; margin-top:1rem; font-size:0.9rem; color:#b0b8c1;">
    Dibuat dengan <span style="color:#ff6f61;">&#10084;</span> oleh Tim Kami
  </div>
</section>

</body>
