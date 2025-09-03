<template>
  <header class="header">
    <div class="container">
      <!-- Logo (enlace relativo a '/') -->
      <a href="/" aria-label="Ir al inicio">
        <img src="/logo.png" alt="Globaltech Logo" />
      </a>

      <!-- Botón de Login -->
      <Link :href="route('login')" class="login-btn" aria-label="Ir a login">
        <a-button type="primary" size="small">Acceder</a-button>
      </Link>
    </div>
  </header>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';
</script>

<style scoped>
/* Estilos básicos */
.header {
  background: #fff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  position: sticky;
  top: 0;
  z-index: 1000;
  padding: 1rem;
}
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
}
.logo img {
  height: 40px;
  width: auto;
}
.login-btn {
  display: inline-flex;
  align-items: center;
}
</style>
