<template>
  <WebLayout>
    <!-- Hero Section -->
    <section class="hero">
      <div class="hero-content">
        <h1>Bienvenido a Globaltech Innovaciones</h1>
        <p>Transformamos ideas en tecnología. Soluciones innovadoras para tu negocio.</p>
        <Link :href="route('login')">
          <a-button type="primary" size="large">Acceder</a-button>
        </Link>
      </div>
    </section>

    <!-- Sección de Servicios -->
    <section class="services">
      <h2>Nuestros Servicios</h2>
      <div class="services-container">
        <div class="service-card">
          <img src="/logo.png" alt="Desarrollo de Software" loading="lazy" />
          <h3>Desarrollo de Software</h3>
          <p>Desarrollamos soluciones a medida que ayudan a optimizar y automatizar procesos.</p>
        </div>
        <!-- <div class="service-card">
          <img src="/logo.png" alt="Aplicaciones Móviles" loading="lazy" />
          <h3>Aplicaciones Móviles</h3>
          <p>Aplicaciones móviles para facilitar la interacción con tus clientes y mejorar la productividad.</p>
        </div>
        <div class="service-card">
          <img src="/logo.png" alt="Diseño Web" loading="lazy" />
          <h3>Diseño Web</h3>
          <p>Diseños web atractivos y funcionales para mejorar la experiencia de tus usuarios.</p>
        </div> -->
      </div>
    </section>

    <!-- Sección de Nosotros -->
    <section class="about">
      <h2>¿Quiénes Somos?</h2>
      <p>
        En Globaltech Innovaciones nos especializamos en soluciones tecnológicas para empresas. Nuestro equipo multidisciplinario tiene experiencia en desarrollo de software, aplicaciones móviles, diseño web y consultoría empresarial.
      </p>
    </section>
  </WebLayout>
</template>

<script setup>
import WebLayout from '@/Layouts/WebLayout.vue';
import { Link } from '@inertiajs/vue3';
</script>

<style scoped>
/* Hero Section */
.hero {
  height: 100vh;
  background: url('/ERPDigital.png') no-repeat center center/cover;
  color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 2rem;
}

.hero-content {
  max-width: 900px;
}

.hero h1 {
  font-size: 3rem;
  font-weight: 700;
}

.hero p {
  font-size: 1.5rem;
  margin-top: 1rem;
}

.services {
  padding: 3rem 2rem;
  background-color: #f9f9f9;
  text-align: center;
}

.services h2 {
  font-size: 2.5rem;
  margin-bottom: 2rem;
}

.services-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.service-card {
  background: #fff;
  padding: 1.5rem;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  text-align: center;
}

.service-card img {
  width: 100%;
  height: auto;
  border-radius: 8px;
  margin-bottom: 1.5rem;
}

.service-card h3 {
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.service-card p {
  font-size: 1rem;
  color: #666;
}

.about {
  padding: 3rem 2rem;
  text-align: center;
}

.about h2 {
  font-size: 2.5rem;
  margin-bottom: 1.5rem;
}

.about p {
  font-size: 1.2rem;
  color: #555;
  line-height: 1.6;
  max-width: 800px;
  margin: 0 auto;
}

/* Mobile Responsiveness */
@media (max-width: 768px) {
  .hero h1 {
    font-size: 2.5rem;
  }

  .hero p {
    font-size: 1.2rem;
  }

  .services-container {
    grid-template-columns: 1fr 1fr;
  }

  .service-card {
    padding: 1rem;
  }

  .about h2 {
    font-size: 2rem;
  }
}
</style>
