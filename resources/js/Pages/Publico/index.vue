```vue
<template>
  <WebLayout>
    <!-- Hero Section with Carousel -->
    <section class="hero">
      <a-carousel autoplay :autoplay-speed="2500" class="carousel">
        <div v-for="(image, index) in carouselImages" :key="index" class="carousel-item">
          <img :src="image" alt="Carousel Image" class="carousel-image" />
        </div>
      </a-carousel>
      <div class="hero-content">
        <h1>Bienvenido a Globaltech Innovaciones</h1>
        <p>Transformamos ideas en tecnología. Descubre nuestro ERP PRISMA: la solución integral para facturación electrónica en Perú, con módulos para contabilidad, compras, ventas y más.</p>
        <div class="hero-buttons">
          <Link :href="route('login')">
            <a-button type="primary" size="large">Acceder</a-button>
          </Link>
          <!-- <a-button type="default" size="large" class="demo-button" @click="scrollToDemo">Ver Demo</a-button> -->
        </div>
      </div>
    </section>

    <!-- Sección de Servicios -->
    <section class="services">
      <h2>Nuestros Servicios</h2>
      <div class="services-container">
        <div class="service-card">
          <img src="/logo.png" alt="ERP PRISMA" loading="lazy" />
          <h3>ERP PRISMA</h3>
          <p>Sistema ERP completo para empresas peruanas. Incluye facturación electrónica, gestión de contabilidad, compras, ventas, almacén, distribución, tesorería y nóminas. Automatiza procesos y asegura cumplimiento normativo.</p>
          <a-button type="link" @click="scrollToFeatures">Ver Módulos</a-button>
        </div>
        <div class="service-card">
          <img src="/logo_prisma.png" alt="Desarrollo de Software" loading="lazy" />
          <h3>Desarrollo de Software</h3>
          <p>Desarrollamos soluciones a medida que ayudan a optimizar y automatizar procesos.</p>
        </div>
      </div>
    </section>

    <!-- Sección de Características / Módulos -->
    <section class="features" id="features">
      <h2>Módulos de ERP PRISMA</h2>
      <a-row :gutter="[16, 16]">
        <a-col :xs="24" :sm="12" :md="8" v-for="(module, index) in modules" :key="index">
          <a-card hoverable class="module-card">
            <template #cover>
              <img alt="module image" :src="module.image" loading="lazy" />
            </template>
            <a-card-meta :title="module.title">
              <template #description>{{ module.description }}</template>
            </a-card-meta>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- Sección de Demo de Módulos -->
    <section class="demo" id="demo">
      <h2>Descubre Nuestros Módulos en Acción</h2>
      <p>Ve una demostración del módulo de contabilidad en ERP PRISMA.</p>
      <div class="video-container">
        <iframe
          width="560"
          height="315"
          src="https://www.youtube.com/embed/hhj-c3Ra7gE"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen
        ></iframe>
      </div>
    </section>

    <!-- Sección de Nosotros -->
    <section class="about">
      <h2>¿Quiénes Somos?</h2>
      <p>
        En Globaltech Innovaciones nos especializamos en soluciones tecnológicas para empresas. Nuestro equipo multidisciplinario tiene experiencia en desarrollo de software, aplicaciones móviles, diseño web y consultoría empresarial. Con ERP PRISMA, ofrecemos una herramienta poderosa para la facturación electrónica y gestión integral en Perú.
      </p>
      <a-button type="primary" size="large" @click="scrollToContact">Contáctanos</a-button>
    </section>

    <!-- Sección de Contacto -->
    <section class="contact" id="contact">
      <h2>Contáctanos</h2>
      <p>¿Listo para transformar tu negocio con ERP PRISMA? Escríbenos y te ayudaremos.</p>
      <a-form layout="vertical" class="contact-form">
        <a-row :gutter="[16, 16]">
          <a-col :xs="24" :sm="12">
            <a-form-item label="Nombre">
              <a-input placeholder="Ingresa tu nombre" />
            </a-form-item>
          </a-col>
          <a-col :xs="24" :sm="12">
            <a-form-item label="Correo Electrónico">
              <a-input placeholder="Ingresa tu correo" />
            </a-form-item>
          </a-col>
          <a-col :span="24">
            <a-form-item label="Mensaje">
              <a-textarea placeholder="Cuéntanos cómo podemos ayudarte" :rows="4" />
            </a-form-item>
          </a-col>
          <a-col :span="24">
            <a-button type="primary" size="large" @click="submitContactForm">Enviar</a-button>
          </a-col>
        </a-row>
      </a-form>
    </section>
  </WebLayout>
</template>

<script setup>
import WebLayout from '@/Layouts/WebLayout.vue';
import { Link } from '@inertiajs/vue3';
import { ref } from 'vue';
import { Carousel as ACarousel, Button as AButton, Row as ARow, Col as ACol, Card as ACard, CardMeta as ACardMeta, Form as AForm, FormItem as AFormItem, Input as AInput, Textarea as ATextarea } from 'ant-design-vue';

const carouselImages = ref([
  'img/img_1.jpg', // Placeholder image
  'img/img_2.jpg', // Placeholder image
  'img/img_3.jpg', // Placeholder image
  'img/img_4.jpg'  // Placeholder image
]);

const modules = ref([
  {
    title: 'Contabilidad',
    description: 'Gestión de asientos contables, plantillas, tipos de cambio y reportes financieros.',
    image: '/img/conta.jpg' // Placeholder, cambia por real
  },
  {
    title: 'Compras',
    description: 'Registro de compras, proveedores y generación automática de asientos.',
    image: '/img/compras.jpg'
  },
  {
    title: 'Ventas',
    description: 'Facturación electrónica, notas de crédito y gestión de clientes.',
    image: '/img/ventas.jpg'
  },
  {
    title: 'Almacén',
    description: 'Control de inventarios, kardex y costos de venta.',
    image: '/img/almacen.jpg'
  },
  {
    title: 'Distribución',
    description: 'Gestión de rutas, entregas y logística.',
    image: '/img/distrubucion.jpg'
  },
  {
    title: 'Tesorería',
    description: 'Gestión de caja, bancos y flujos de efectivo.',
    image: '/img/tesoreria.jpg'
  },
  {
    title: 'Nóminas',
    description: 'Cálculo de sueldos, deducciones y reportes laborales.',
    image: '/img/nomina.jpg'
  }
]);

const scrollToDemo = () => {
  document.getElementById('demo').scrollIntoView({ behavior: 'smooth' });
};

const scrollToFeatures = () => {
  document.getElementById('features').scrollIntoView({ behavior: 'smooth' });
};

const scrollToContact = () => {
  document.getElementById('contact').scrollIntoView({ behavior: 'smooth' });
};

const submitContactForm = () => {
  // Placeholder for form submission logic
  alert('Formulario enviado. ¡Gracias por contactarnos!');
};
</script>

<style scoped>
/* Hero Section */
.hero {
  position: relative;
  height: 100vh;
  color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 2rem;
  overflow: hidden;
}

.carousel {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -1;
}

.carousel-item {
  height: 100vh;
  width: 100%;
}

.carousel-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
}

.hero-content {
  max-width: 900px;
  z-index: 1;
  background: rgba(0, 0, 0, 0.5);
  padding: 2rem;
  border-radius: 8px;
}

.hero h1 {
  font-size: 3.5rem;
  font-weight: 700;
  margin-bottom: 1rem;
  animation: fadeInDown 1s ease-in;
}

.hero p {
  font-size: 1.5rem;
  margin-bottom: 2rem;
  animation: fadeInUp 1s ease-in;
}

.hero-buttons {
  display: flex;
  gap: 1rem;
  justify-content: center;
}

.demo-button {
  animation: fadeInUp 1s ease-in 0.2s;
}

/* Services */
.services {
  padding: 4rem 2rem;
  background-color: #f9f9f9;
  text-align: center;
}

.services h2 {
  font-size: 2.5rem;
  margin-bottom: 2rem;
  animation: fadeIn 1s ease-in;
}

.services-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.service-card {
  background: #fff;
  padding: 1.5rem;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  text-align: center;
  transition: transform 0.3s ease;
}

.service-card:hover {
  transform: translateY(-5px);
}

.service-card img {
  width: 100%;
  height: 150px;
  object-fit: cover;
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

/* Features */
.features {
  padding: 4rem 2rem;
  background-color: #fff;
  text-align: center;
}

.features h2 {
  font-size: 2.5rem;
  margin-bottom: 2rem;
  animation: fadeIn 1s ease-in;
}

.module-card {
  transition: transform 0.3s ease;
}

.module-card:hover {
  transform: translateY(-5px);
}

.module-card img {
  height: 150px;
  object-fit: cover;
}

/* Demo */
.demo {
  padding: 4rem 2rem;
  background-color: #f9f9f9;
  text-align: center;
}

.demo h2 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  animation: fadeIn 1s ease-in;
}

.demo p {
  font-size: 1.2rem;
  margin-bottom: 2rem;
}

.video-container {
  max-width: 800px;
  margin: 0 auto;
}

.video-container iframe {
  width: 100%;
  height: auto;
  aspect-ratio: 16/9;
}

/* About */
.about {
  padding: 4rem 2rem;
  text-align: center;
}

.about h2 {
  font-size: 2.5rem;
  margin-bottom: 1.5rem;
  animation: fadeIn 1s ease-in;
}

.about p {
  font-size: 1.2rem;
  color: #555;
  line-height: 1.6;
  max-width: 800px;
  margin: 0 auto 2rem;
}

/* Contact */
.contact {
  padding: 4rem 2rem;
  background-color: #fff;
  text-align: center;
}

.contact h2 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  animation: fadeIn 1s ease-in;
}

.contact p {
  font-size: 1.2rem;
  margin-bottom: 2rem;
}

.contact-form {
  max-width: 600px;
  margin: 0 auto;
}

/* Animations */
@keyframes fadeInDown {
  from {
    opacity: 0;
    transform: translateY(-20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Mobile Responsiveness */
@media (max-width: 768px) {
  .hero h1 {
    font-size: 2.5rem;
  }

  .hero p {
    font-size: 1.2rem;
  }

  .hero-buttons {
    flex-direction: column;
    gap: 0.5rem;
  }

  .services-container {
    grid-template-columns: 1fr;
  }

  .service-card {
    padding: 1rem;
  }

  .about h2,
  .demo h2,
  .features h2,
  .contact h2 {
    font-size: 2rem;
  }
}

@media (max-width: 576px) {
  .hero h1 {
    font-size: 2rem;
  }

  .hero p {
    font-size: 1rem;
  }

  .video-container {
    max-width: 100%;
  }
}
</style>
```
