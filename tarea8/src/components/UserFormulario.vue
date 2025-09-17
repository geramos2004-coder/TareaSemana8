<template>
  <div class="form-container">
    <h2>FORMULARIO PARA NUEVOS USUARIOS</h2>
    <form @submit.prevent="enviarFormulario">
      <div class="form-group">
        <label for="codigo">Código:</label>
        <input type="text" id="codigo" v-model="codigo" required />
      </div>

      <div class="form-group">
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" v-model="nombre" required />
      </div>

      <div class="form-group">
        <label for="categoria">Categoría:</label>
        <select id="categoria" v-model="categoria">
          <option value="">No especificar</option>
          <option value="Electrónica">Electrónica</option>
          <option value="Ropa">Ropa</option>
          <option value="Hogar">Hogar</option>
          <option value="Alimentos">Alimentos</option>
        </select>
      </div>

      <div class="form-group">
        <label for="precioCompra">Precio Compra:</label>
        <input type="number" id="precioCompra" v-model="precioCompra" required min="0" step="0.01" />
      </div>

      <div class="form-group">
        <label for="precioVenta">Precio Venta:</label>
        <input type="number" id="precioVenta" v-model="precioVenta" required min="0" step="0.01" />
      </div>

      <button type="submit">Guardar</button>
    </form>
  </div>
</template>

<script setup>
</script>

<style scoped>
.form-container {
  max-width: 450px;
  margin: 20px auto;
  padding: 1.5rem;
  background: #ffffff;
  border-radius: 12px;
  box-shadow: 0px 6px 18px rgba(0, 0, 0, 0.08);
}

h2 {
  text-align: center;
  color: #086105;
  font-size: 1.5rem;
  margin-bottom: 1.2rem;
}

.form-group {
  display: flex;
  align-items: center;
  margin-bottom: 1rem;
}

label {
  width: 140px; /* ancho fijo para alinear */
  font-weight: 600;
  color: #333;
}

input,
select {
  flex: 1; /* ocupa el espacio restante */
  padding: 0.55rem;
  border: 1px solid #ddd;
  border-radius: 6px;
  font-size: 0.95rem;
  transition: border 0.25s ease, box-shadow 0.25s ease;
}

input:focus,
select:focus {
  border-color: #0077ff;
  outline: none;
  box-shadow: 0 0 6px rgba(0, 119, 255, 0.35);
}

button {
  width: 100%;
  padding: 0.75rem;
  margin-top: 0.5rem;
  background: linear-gradient(90deg, #056d27, #103d09);
  color: white;
  font-weight: bold;
  font-size: 1rem;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  transition: background 0.25s ease, transform 0.2s ease;
}

button:hover {
  background: linear-gradient(90deg, #25282b, #3c3e3f);
  transform: scale(1.02);
}
</style>
