<template>
  <nav class="navbar">
    <div class="logo">MiLogo</div>
    <ul class="nav-links">
      <li><a href="#">Inicio</a></li>
      <li><a href="#">Categorias</a></li>
      <li><a href="#">Servicios</a></li>
      <li><a href="#">Contacto</a></li>
    </ul>
    <button class="btn-login">Iniciar Sesión</button>
  </nav>
</template>

<script setup>
let uno = 5;
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: linear-gradient(90deg, #1f4037, #99f2c8);
  padding: 1rem 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
}

/* Logo */
.logo {
  font-size: 1.5rem;
  font-weight: bold;
  color: white;
  letter-spacing: 2px;
}

/* Links */
.nav-links {
  list-style: none;
  display: flex;
  gap: 2rem;
}

.nav-links li a {
  color: white;
  text-decoration: none;
  font-weight: 500;
  position: relative;
  transition: color 0.3s ease;
}

.nav-links li a:hover {
  color: #ffe600;
}

.nav-links li a::after {
  content: "";
  position: absolute;
  width: 0%;
  height: 2px;
  background: #ffe600;
  left: 0;
  bottom: -4px;
  transition: width 0.3s ease;
}

.nav-links li a:hover::after {
  width: 100%;
}

/* Botón */
.btn-login {
  padding: 0.5rem 1rem;
  background: #ffe600;
  color: #1f4037;
  border: none;
  border-radius: 20px;
  font-weight: bold;
  cursor: pointer;
  transition: all 0.3s ease;
}

.btn-login:hover {
  background: white;
  color: #1f4037;
  transform: scale(1.05);
}
</style>
