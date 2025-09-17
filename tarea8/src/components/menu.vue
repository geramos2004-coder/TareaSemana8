<template>

    <nav class="navbar">
    <ul class="nav-links">
      <li><a href="#">Inicio</a></li>
      <li><a href="#">Categorias</a></li>
      <li><a href="#">Servicios</a></li>
      <li><a href="#">Contacto</a></li>
    </ul>
  </nav>

  <!-- <h1>numero:{{ uno }}</h1>-->
    
</template>

<script setup>

var uno=5;

</script>

<style scoped>

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: linear-gradient(90deg, rgb(28, 30, 32), #3c535a);
  padding: 0.8rem 1.5rem;
  border-radius: 8px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);

 

  .nav-links {
    list-style: none;
    display: flex;
    gap: 1.5rem;

    li a {
      color: white;
      text-decoration: none;
      font-weight: 500;
      position: relative;

      &:hover {
        color: #ffeb3b;
      }

      &::after {
        content: "";
        position: absolute;
        width: 0%;
        height: 2px;
        background: #ffeb3b;
        left: 0;
        bottom: -4px;
        transition: width 0.3s ease;
      }

      &:hover::after {
        width: 50%;
      }
    }
  }
}

.content {
  margin-top: 1rem;
  padding: 1rem;
  background: #f8f9fa;
  border-radius: 8px;
  text-align: center;
}

</style>