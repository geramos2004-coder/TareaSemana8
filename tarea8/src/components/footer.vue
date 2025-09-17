<template>
  <footer class="footer">
    <div class="footer-content">
      <p>© 2025 Todos los derechos reservados.</p>
      <p>Santa Tecla, El Salvador · Diseñado por Noé</p>
    </div>
  </footer>
</template>

<script setup>
</script>

<style scoped>
.footer {
  background: linear-gradient(135deg, #1e3c72, #2a5298);
  color: #f1f1f1;
  text-align: center;
  padding: 1.2rem 1rem;
  border-radius: 12px 12px 0 0;
  box-shadow: 0px -3px 12px rgba(0, 0, 0, 0.25);
  transition: all 0.4s ease;
  position: relative;
  overflow: hidden;
}

.footer::before {
  content: "";
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
  animation: pulse 6s infinite;
}

@keyframes pulse {
  0% { transform: scale(0.8); opacity: 0.5; }
  50% { transform: scale(1.2); opacity: 0.2; }
  100% { transform: scale(0.8); opacity: 0.5; }
}

.footer-content {
  position: relative;
  z-index: 2;
}

.footer p {
  margin: 0.3rem 0;
  font-size: 1rem;
  letter-spacing: 0.5px;
  text-shadow: 0px 1px 2px rgba(0,0,0,0.4);
}

/* Efecto al pasar el mouse */
.footer:hover {
  background: linear-gradient(135deg, #2a5298, #1e3c72);
  box-shadow: 0px -4px 16px rgba(0, 0, 0, 0.4);
  transform: translateY(-2px);
}
</style>
