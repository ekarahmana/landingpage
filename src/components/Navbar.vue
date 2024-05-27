<template>
  <nav class="navbar">
    <div class="container">
      <a href="#" class="navbar-brand">Eka Olshop</a>
      <ul class="navbar-nav">
        <li class="nav-item"><a href="#" class="nav-link">Home</a></li>
        <li class="nav-item"><a href="#" class="nav-link">Products</a></li>
        <li class="nav-item"><a href="#" class="nav-link">Contact</a></li>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
.navbar {
  background-color: #004E9B;
  padding: 1rem;
}
.navbar-brand {
  color: #ffffff;
  font-size: 2rem;
  font-family: Slab Serif;
}
.navbar-nav {
  list-style: none;
  display: flex;
  gap: 1rem;
}
.nav-item .nav-link {
  color: #fff;
  text-decoration: none;
}
</style>
