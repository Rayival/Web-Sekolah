<template>
  <main class="container mt-4">
    <section class="mb-4">
      <!-- <div class="relative">
        <img
          alt="A large banner image showing the school building with students in the foreground"
          class="img-fluid"
          src="assets/bgHome.png"
        /><div class="position-absolute top-0 start-0 w-100 h-100 bg-opacity-50 d-flex align-items-center justify-content-center"> -->
        
          <h2 class="text-white text-center">
            Welcome to SMK Negeri 4 Tasikmalaya
          </h2>
        <!-- </div>
      </div> -->
    </section>

    <section class="mb-4">
      <h2 class="h4 font-weight-bold mb-3">Kompetensi Keahlian</h2>
      <div class="row">
        <div class="col-12 col-md-6 col-lg-4 mb-4" v-for="news in latestNews" :key="news.title">
          <div class="card">
            <img
              :alt="news.alt"
              class="card-img-top"
              :src="news.image"
            />
            <div class="card-body">
              <h3 class="card-title">{{ news.title }}</h3>
              <p class="card-text">{{ news.description }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import tbsmImage from'~/assets/tbsm.jpg';
import tjktImage from'~/assets/tjkt.jpg';
import pplgImage from'~/assets/pplg.jpg';
import dkvImage from'~/assets/dkv.jpg';
import toiImage from'~/assets/toi.jpg';

export default {
  data() {
    return {
      latestNews: [
        {
          title: "TJKT",
          description: "TEKNIK JARINGAN KOMPUTER DAN TELEKOMUNIKASI",
          image: tjktImage,
        },
        {
          title: "TBSM",
          description: "TEKNIK DAN BISNIS SEPEDA MOTORㅤㅤㅤ ㅤㅤㅤㅤㅤ",
          image: tbsmImage,
        },
        {
          title: "PPLG",
          description: "PENGEMBANGAN PERANGKAT LUNAK DAN GIMㅤㅤㅤㅤㅤ ㅤㅤㅤㅤㅤ ",
          image: pplgImage,
        },
        {
          title: "DKV",
          description: "DESAIN KOMUNIKASI VISUALㅤㅤㅤ ㅤ ㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤ ㅤㅤㅤㅤㅤ ㅤㅤㅤㅤㅤ ",
          image: dkvImage,
        },
        {
          title: "TOI",
          description: "TEKNIK OTOMASI INDUSTRIㅤㅤㅤ ㅤ ㅤㅤㅤㅤㅤㅤㅤㅤ ㅤ",
          image: toiImage,
        }
      ]
    }
  }
}
      </script>
