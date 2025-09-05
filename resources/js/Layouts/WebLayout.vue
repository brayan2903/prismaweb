<template>
  <div class="web-layout">
    <Header />
    <main>
      <slot />
    </main>
    <Footer />

    <!-- Botón flotante de WhatsApp (fuera del flujo del Header y Footer) -->
    <WhatsAppButton />
  </div>
</template>

<script setup>
import Header from '@/Components/Publico/Header.vue';
import Footer from '@/Components/Publico/Footer.vue';
import WhatsAppButton from '@/Components/WhatsAppButton.vue'; // Importa el componente
</script>

<style scoped>
.web-layout {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

main {
  flex: 1;
}

/* Puedes personalizar aún más el layout aquí */
</style>
