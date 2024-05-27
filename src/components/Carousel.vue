<template>
    <div class="carousel">
      <div class="carousel-item" v-for="(item, index) in items" :key="index">
        <img :src="item.image" :alt="item.title">
        <div class="carousel-caption">
          <h3>{{ item.title }}</h3>
          <p>{{ item.description }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        items: [
          { image: 'https://cdn1.productnation.co/optimized/1024w/stg/sites/5/6423be98aa90a.webp' ,title: 'Emina Bright Stuff productnation', description: 'Emina dikenal sebagai brand kecantikan yang remaja-friendly dengan dibanderol harga sesuai kantong pelajar. Bright Stuff series sendiri merupakan rangkat paket Emina skincare yang akan merawat kulit menjadi lebih cerah dan sehat productnation' },
          { image: 'https://cdn1.productnation.co/optimized/1024w/stg/sites/5/6423bbec28093.webp', title: 'Wardah Nature Daily Aloe Vera productnation', description: 'Aloe vera atau lidah buaya merupakan salah satu bahan alami yang kaya akan kandungan nutrisi baik meliputi vitamin, antioksidan, kalsium, hingga asam amino esensial productnation' },
          { image: 'https://cdn1.productnation.co/optimized/1024w/stg/sites/5/6423c405240b0.webp', title: 'MS Glow For Men productnation', description: 'Siapa bilang skincare hanya untuk wanita? Di zaman sekarang ini, para pria pun juga perlu merawat kulit agar tetap terjaga bersih dan sehat. Nah, kalau kamu mencari paket skincare pria untuk memenuhi kebutuhan perawatan wajahmu, maka produk MS Glow ini bisa menjadi opsi terbaik.  productnation' },
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .carousel {
    display: flex;
    overflow: auto;
    width: 100%;
  }
  .carousel-item {
    min-width: 100%;
    position: relative;
    text-align: center;
  }
  .carousel-caption {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    background:#009189;
    color: #BAE4F0;
    padding: 1rem;
    border-radius: 30px;
  }
  </style>
  