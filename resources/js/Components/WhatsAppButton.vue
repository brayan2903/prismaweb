<template>
  <a
    href="https://wa.me/51961697533?text=Me%20interesa%20los%20m%C3%B3dulos%20del%20sistema%20ERPPRISMA.%20Quiero%20m%C3%A1s%20informaci%C3%B3n."
    target="_blank"
    class="fixed bottom-4 right-4 bg-green-500 text-white p-4 rounded-full shadow-lg hover:bg-green-600 transition float-effect">

    <!-- Imagen de WhatsApp -->
    <img src="/img/whatsapp.png" alt="WhatsApp" class="w-8 h-8" />
  </a>
</template>

<script>
export default {
  name: "WhatsAppButton"
};
</script>

<style scoped>
/* Animación de flotación hacia arriba y abajo */
.float-effect {
  animation: float 3s ease-in-out infinite;
}

/* Keyframes para el movimiento flotante */
@keyframes float {
  0%, 100% {
    transform: translateY(0); /* posición inicial y final */
  }
  50% {
    transform: translateY(-10px); /* mueve el botón hacia arriba */
  }
}
</style>
