<script setup>
defineProps({
  nama: String,
  jabatan: String,
  inisial: String
});
</script>

<template>
  <div class="team-card">
    <div class="avatar">{{ inisial }}</div>
    <h3>{{ nama }}</h3>
    <p>{{ jabatan }}</p>
  </div>
  </template>

<style scoped>
.team-card {
  background: white;
  padding: 25px 20px;
  border-radius: 12px;
  text-align: center;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
  flex: 1;
  min-width: 200px;
}

.avatar {
  width: 70px;
  height: 70px;
  background-color: #e012fc;
  color: white;
  font-size: 1.5rem;
  font-weight: bold;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  margin: 0 auto 15px auto;
}

.team-card h3 {
  font-size: 1.1rem;
  margin-bottom: 5px;
  color: #1f2937;
}

.team-card p {
  font-size: 0.9rem;
  color: #6b7280;
}
</style>