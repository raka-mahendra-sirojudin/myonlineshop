<template>
  <div class="landing-page">

    <section class="hero">
      <h1>Belanja Perlengkapan Sekolah, Gampang & Terpercaya</h1>
      <p>Dari kaos, topi, sampai tas sekolah — semua ada di satu tempat.</p>
      <router-link to="/product" class="btn-primary">Lihat Produk</router-link>
      
      <div class="video-container">
        <video controls width="480" muted loop>
          <source src="/video/promo-toko.mp4" type="video/mp4" />
          Browser kamu tidak mendukung pemutaran video.
        </video>
      </div>
    </section>

    <section class="features">
      <div class="feature-card">
        <div class="icon">⭐</div>
        <h3>Kualitas Terjamin</h3>
        <p>Dipilih dan dikurasi langsung oleh tim sekolah.</p>
      </div>

      <div class="feature-card">
        <div class="icon">🏷️</div>
        <h3>Harga Bersahabat</h3>
        <p>Harga ramah di kantong siswa.</p>
      </div>

      <div class="feature-card">
        <div class="icon">🏫</div>
        <h3>Ambil di Sekolah</h3>
        <p>Tidak perlu ongkir, ambil langsung di koperasi.</p>
      </div>
    </section>
  </div>
</template>

<style scoped>
.landing-page {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #333;
}

.hero {
  background: linear-gradient(135deg, #37ff47, #02b145);
  color: white;
  padding: 80px 20px;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center; 
}

.hero h1 {
  font-size: 2.5rem;
  margin-bottom: 15px;
}

.hero p {
  font-size: 1.1rem;
  margin-bottom: 30px;
  opacity: 0.9;
}

.btn-primary {
  display: inline-block;
  background-color: white;
  color: #4f46e5;
  padding: 12px 30px;
  border-radius: 999px;
  text-decoration: none;
  font-weight: bold;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

.video-container {
  margin-top: 30px;
}

video {
  margin-top: 16px;
  border-radius: 10px;
  display: block;
  max-width: 100%;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
}

.features {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  justify-content: center;
  padding: 60px 20px;
  max-width: 1100px;
  margin: 0 auto;
}

.feature-card {
  background: white;
  flex: 1;
  min-width: 250px;
  max-width: 320px;
  padding: 30px 20px;
  border-radius: 12px;
  text-align: center;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
  transition: transform 0.2s ease;
}

.feature-card:hover {
  transform: translateY(-5px);
}

.feature-card .icon {
  font-size: 2.5rem;
  margin-bottom: 15px;
}

.feature-card h3 {
  margin-bottom: 10px;
  color: #1f2937;
}

.feature-card p {
  color: #6b7280;
  font-size: 0.95rem;
  line-height: 1.5;
}
</style>