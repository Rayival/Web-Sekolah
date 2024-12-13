<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-content">
        <div class="footer-logo">
          <h1>Nama Sekolah</h1>
        </div>
        <div class="footer-links">
          <ul>
            <li><a href="#about">Tentang Kami</a></li>
            <li><a href="#program">Program</a></li>
            <li><a href="#kontak">Kontak</a></li>
            <li><a href="#berita">Berita</a></li>
          </ul>
        </div>
        <div class="footer-social">
          <a href="https://www.facebook.com/4smkn" target="_blank">Facebook</a>
          <a href="https://x.com/4_smkn" target="_blank">Twitter</a>
          <a href="https://www.instagram.com/smkn4tasikmalaya/" target="_blank">Instagram</a>
        </div>
      </div>
      <div class="footer-bottom">
        <p>&copy; {{ currentYear }} Nama Sekolah. All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      currentYear: new Date().getFullYear(),
    };
  },
};
</script>

<style scoped>
.footer {
  background-color: #333;
  color: white;
  padding: 20px 0;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  width: 100%;
  max-width: 1200px;
  flex-wrap: wrap; /* Allow wrapping for responsiveness */
}

.footer-links ul {
  list-style: none;
  padding: 0;
  display: flex; /* Use flexbox for links */
  flex-wrap: wrap; /* Allow wrapping for smaller screens */
  justify-content: center; /* Center the links */
}

.footer-links li {
  margin: 0 10px;
}

.footer-links a {
  color: white;
  text-decoration: none;
}

.footer-social {
  display: flex;
  justify-content: center; 
  margin-top: 10px; 
}

.footer-social a {
  margin: 0 10px;
  color: white;
  text-decoration: none;
}

.footer-bottom {
  text-align: center;
  margin-top: 20px;
}

/* Media Query untuk Responsivitas */
@media (max-width: 768px) {
  .footer-content {
    flex-direction: column; /* Stack items vertically on small screens */
    align-items: center; /* Center items */
  }

  .footer-links ul {
    justify-content: center; /* Center links on small screens */
  }

  .footer-social {
    margin-top: 15px; /* Add more space for social links */
  }
}
</style>
