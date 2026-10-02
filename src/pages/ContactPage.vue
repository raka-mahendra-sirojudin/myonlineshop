<template>
  <div class="contact-page">

    <section class="contact-banner">
      <h1>Hubungi Kami</h1>
    </section>

    <section class="contact-container">
      
      <div class="info-box">
        <h2>Info Kontak</h2>
        <div class="info-item">
          <span class="icon">📍</span>
          <div>
            <strong>Alamat</strong>
            <p>Jl. Pameran Pendidikan No. 1, Soreang, Kab. Bandung</p>
          </div>
        </div>
        <div class="info-item">
          <span class="icon">📞</span>
          <div>
            <strong>Telepon</strong>
            <p>0895 6058 66615</p>
          </div>
        </div>
        <div class="info-item">
          <span class="icon">✉️</span>
          <div>
            <strong>Email</strong>
            <p>buniiversity@gmail.com</p>
          </div>
        </div>
      </div>

      <div class="form-box">
        <h2>Kirim Pesan</h2>
        <form @submit.prevent>
          <div class="form-group">
            <label for="nama">Nama</label>
            <input type="text" id="nama" placeholder="Masukkan nama Anda" />
          </div>

          <div class="form-group">
            <label for="email">Email</label>
            <input type="email" id="email" placeholder="Masukkan email Anda" />
          </div>

          <div class="form-group">
            <label for="pesan">Pesan</label>
            <textarea id="pesan" rows="4" placeholder="Tuliskan pesan atau pertanyaan..."></textarea>
          </div>

          <button type="submit" class="btn-submit">Kirim</button>
        </form>
      </div>
    </section>
  </div>
</template>

<style scoped>
.contact-page {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #333;
}

.contact-banner {
  background: linear-gradient(135deg, #d91dff, #3d1bff);
  color: white;
  padding: 50px 20px;
  text-align: center;
}

.contact-banner h1 {
  font-size: 2rem;
}


.contact-container {
  display: flex;
  gap: 30px;
  max-width: 1000px;
  margin: 50px auto;
  padding: 0 20px;
  flex-wrap: wrap;
}

.info-box, .form-box {
  flex: 1;
  min-width: 280px;
  background: white;
  padding: 30px;
  border-radius: 12px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
}

.info-box h2, .form-box h2 {
  margin-bottom: 20px;
  color: #1f2937;
  font-size: 1.3rem;
}

.info-item {
  display: flex;
  gap: 15px;
  margin-bottom: 20px;
  align-items: flex-start;
}

.info-item .icon {
  font-size: 1.4rem;
}

.info-item strong {
  display: block;
  color: #374151;
  margin-bottom: 3px;
}

.info-item p {
  color: #6b7280;
  font-size: 0.95rem;
  margin: 0;
}

.form-group {
  margin-bottom: 15px;
}

.form-group label {
  display: block;
  font-size: 0.9rem;
  font-weight: 600;
  color: #374151;
  margin-bottom: 5px;
}

.form-group input,
.form-group textarea {
  width: 100%;
  padding: 10px 15px;
  border-radius: 8px;
  border: 1px solid #d1d5db;
  font-size: 0.95rem;
  font-family: inherit;
  box-sizing: border-box;
  outline: none;
  transition: border-color 0.2s;
}

.form-group input:focus,
.form-group textarea:focus {
  border-color: #4f46e5;
}

.btn-submit {
  background-color: #4f46e5;
  color: white;
  border: none;
  padding: 12px 30px;
  border-radius: 999px;
  font-weight: bold;
  cursor: pointer;
  transition: background-color 0.2s, transform 0.2s;
  width: 100%;
}

.btn-submit:hover {
  background-color: #4338ca;
  transform: translateY(-2px);
}
</style>