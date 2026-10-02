<script setup>
import { ref } from 'vue';
import TeamCard from '../components/TeamCard.vue';

const daftarTim = ref([
  { nama: 'Faris', jabatan: 'Ketua Tim', inisial: 'F' },
  { nama: 'Niccolo Terre', jabatan: 'Desain & UI/UX', inisial: 'N' },
  { nama: 'Stephen Faulkner', jabatan: 'Logistik', inisial: 'S', image: 'https://placehold.co/150' },
  { nama: 'Dimas', jabatan: 'Pengembangan Produk', inisial: 'D' },
  { nama: 'Rizky', jabatan: 'Pemasaran & Media Sosial', inisial: 'R' },
]);
</script>

<template>
  <div class="about-page">
    
    <section class="about-banner">
      <h1>Tentang Kami</h1>
    </section>

    <section class="story-section">
      <div class="story-text">
        <h2>Cerita Kami</h2>
        <p>
          Onlineshop ini dikelola langsung oleh siswa SMK Yadika Soreang Jurusan Rekayasa Perangkat Lunak (RPL), 
          sebagai proyek belajar sekaligus membantu teman-teman mendapatkan perlengkapan sekolah dengan mudah dan harga terjangkau.
        </p>
        <p>
          Setiap produk dipilih dan dikurasi oleh tim kecil siswa dengan pengawasan langsung di koperasi sekolah.
        </p>
      </div>
      <div class="story-image">
        <div class="image-placeholder">📷 Foto Ilustrasi Toko</div>
      </div>
    </section>

    <section class="team-section">
      <h2>Tim Kami</h2>
      <div class="team-grid">
        <TeamCard 
          v-for="(anggota, index) in daftarTim" 
          :key="index"
          :nama="anggota.nama"
          :jabatan="anggota.jabatan"
          :inisial="anggota.inisial"
        />
      </div>
    </section>
  </div>
</template>

<style scoped>
.about-page {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #333;
}

.about-banner {
  background: linear-gradient(135deg, #9718ff, #3a2df5);
  color: white;
  padding: 50px 20px;
  text-align: center;
}

.about-banner h1 {
  font-size: 2rem;
}

.story-section {
  display: flex;
  align-items: center;
  gap: 40px;
  max-width: 1000px;
  margin: 60px auto;
  padding: 0 20px;
  flex-wrap: wrap;
}

.story-text, .story-image {
  flex: 1;
  min-width: 280px;
}

.story-text h2 {
  margin-bottom: 15px;
  color: #1f2937;
}

.story-text p {
  color: #4b5563;
  line-height: 1.6;
  margin-bottom: 15px;
}

.image-placeholder {
  width: 100%;
  height: 220px;
  background-color: #e5e7eb;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #6b7280;
  font-weight: 500;
}

.team-section {
  max-width: 1000px;
  margin: 0 auto 60px auto;
  padding: 0 20px;
  text-align: center;
}

.team-section h2 {
  margin-bottom: 30px;
  color: #1f2937;
}

.team-grid {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  justify-content: center;
}
img {
  max-width: 100%;
  border-radius: 8px;
}
</style>