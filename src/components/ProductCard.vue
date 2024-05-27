<template>
    <div class="card">
      <img :src="product.image" :alt="product.name" class="card-img">
      <div class="card-body">
        <h5 class="card-title">{{ product.name }}</h5>
        <p class="card-text">{{ product.description }}</p>
        <p class="card-price">{{ product.price }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      product: Object
    }
  };
  </script>
  
  <style scoped>
  .card {
    border: 1px solid #ddd;
    border-radius: 5px;
    overflow: hidden;
    margin: 1rem;
    width: 200px;
  }
  .card-img {
    width: 100%;
    height: 150px;
    object-fit: cover;
  }
  .card-body {
    padding: 1rem;
  }
  .card-title {
    font-size: 1.25rem;
    margin: 0 0 0.5rem;
  }
  .card-price {
    font-weight: bold;
    color: #d9534f;
  }
  </style>
  