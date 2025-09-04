<template>
  <WebLayout>
    <Head title="ERP PRISMA | Módulo de Ventas — Optimiza tu proceso comercial" />

    <!-- HERO / VALUE PROP -->
    <section class="hero">
      <a-row :gutter="[24,24]" align="middle">
        <a-col :xs="24" :md="14">
          <h1 class="hero-title">Módulo de Ventas PRISMA</h1>
          <p class="hero-subtitle">
            Realiza operaciones comerciales de manera ágil y flexible, con reportes y consultas de valor que optimizan tu negocio.
          </p>

          <ul class="hero-bullets">
            <li>📦 Agiliza la generación de pedidos y facturaciones parciales</li>
            <li>💳 Flexibilidad en operaciones comerciales</li>
            <li>📊 Reportes de ventas, ranking de clientes y trazabilidad total</li>
            <li>🔄 Facilidad de integración con otros programas</li>
          </ul>

          <div class="hero-cta">
            <!-- <a-button type="primary" size="large" @click="contactar">
              Solicitar demostración
            </a-button>
            <a-button size="large" @click="descargarBrochure" class="cta-secondary">
              Descargar brochure (PDF)
            </a-button> -->
          </div>
        </a-col>

        <a-col :xs="24" :md="10">
          <a-card :hoverable="true" class="hero-card" :bodyStyle="{ padding: '0' }">
            <img class="hero-image" src="/img_modulos/pv1.jpeg" alt="Dashboard de Ventas PRISMA" />
            <div class="ribbon">Gestión comercial eficiente</div>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- DESCRIPCIÓN DEL MÓDULO -->
    <section class="description">
      <h2 class="section-title">Descripción del Módulo de Ventas</h2>
      <p>El Módulo de Ventas de ERP Prisma está diseñado para adaptarse a las necesidades comerciales de tu negocio. Agiliza los procesos de generación de pedidos, facturación, y seguimiento de ventas con total trazabilidad, todo desde una interfaz fácil de usar.</p>
    </section>

    <!-- BENEFICIOS PRINCIPALES -->
    <section class="features">
      <h2 class="section-title">Beneficios Principales</h2>
      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Agiliza el Proceso de Generación de Pedido</template>
            <ul class="feature-list">
              <li>Generación rápida y eficiente de pedidos, mejorando el tiempo de respuesta con el cliente.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Facturación Parcial</template>
            <ul class="feature-list">
              <li>Permite realizar facturaciones parciales para mejorar la flexibilidad de los pagos.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Reportes y Consultas de Ventas</template>
            <ul class="feature-list">
              <li>Genera reportes detallados de ventas, ranking de clientes y trazabilidad total del proceso comercial.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Trazabilidad Total</template>
            <ul class="feature-list">
              <li>Sigue todo el proceso de venta, desde la generación del pedido hasta la facturación, con total trazabilidad.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Flexibilidad en la Operación</template>
            <ul class="feature-list">
              <li>El sistema es flexible, permitiendo diferentes modalidades de ventas y formas de pago.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Integración con Otros Sistemas</template>
            <ul class="feature-list">
              <li>Exporta tus datos de ventas a otros programas comunes de uso, facilitando el análisis y la integración.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- FUNCIONALIDADES DEL MÓDULO -->
    <section class="functionalities">
      <h2 class="section-title">Funcionalidades del Módulo</h2>
      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Venta y Compra con Códigos de Barra</template>
            <ul class="feature-list">
              <li>Compra y venta utilizando códigos de barras para una gestión más rápida y precisa.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Consultas Multidimensionales de Ventas</template>
            <ul class="feature-list">
              <li>Consulta de ventas en diferentes niveles, con filtros detallados y flexibilidad en la visualización de datos.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Gestión de Pagos y Cuotas</template>
            <ul class="feature-list">
              <li>Gestión de pagos a cuenta, extornos de pago, y manejo de cuotas por cobrar y pagar.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Reporte de Ranking de Clientes</template>
            <ul class="feature-list">
              <li>Genera un reporte de ranking de clientes, ayudando a identificar a los más rentables y a enfocar esfuerzos de ventas.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- CTA FINAL -->
    <section class="cta-final">
      <a-card class="cta-card" :hoverable="true">
        <h3>¿Listo para optimizar tus ventas?</h3>
        <p>Solicita una demo personalizada y descubre cómo PRISMA puede transformar tu proceso comercial.</p>
        <div class="cta-actions">
          <a-button type="primary" size="large" @click="contactar">Contactarse</a-button>
          <!-- <a-button size="large" ghost @click="hablarVentas">Hablar con ventas</a-button> -->
        </div>
      </a-card>
    </section>
  </WebLayout>
</template>

<script setup>
import WebLayout from '@/Layouts/WebLayout.vue'
import { Head } from '@inertiajs/vue3'

const contactar = () => {
  window.location.href = '/contacto?modulo=ventas'
}

const hablarVentas = () => {
  window.location.href = 'tel:+51010000000' // placeholder; cámbialo por tu número
}

const descargarBrochure = () => {
  window.location.href = '/brochure-ventas.pdf' // placeholder; súbelo a tu storage público
}
</script>

<style scoped>
/* Paleta */
:root {
  --primary: #00a0c8;
  --text: #1f2d3d;
  --muted: #5c6773;
  --bg-soft: #f7fbfd;
}

/* Layouts de sección */
section { padding: 64px 16px; }
.section-title {
  text-align: center;
  font-size: 28px;
  margin-bottom: 24px;
  color: var(--text);
}

/* HERO */
.hero { background: linear-gradient(180deg, #ffffff, var(--bg-soft)); }
.hero-badge { margin-bottom: 8px; }
.hero-title {
  font-size: 40px;
  line-height: 1.1;
  margin: 8px 0 12px;
  color: var(--primary);
  font-weight: 800;
}
.hero-subtitle {
  font-size: 18px;
  color: var(--muted);
  margin-bottom: 16px;
}
.hero-bullets { list-style: none; padding: 0; margin: 0 0 16px; }
.hero-bullets li { margin: 6px 0; color: var(--text); }
.hero-cta { display: flex; gap: 12px; flex-wrap: wrap; margin: 12px 0 8px; }
.cta-secondary { border-color: var(--primary); color: var(--primary); }

.hero-card { position: relative; border: none; }
.hero-image { width: 100%; height: auto; display: block; }
.ribbon {
  position: absolute;
  top: 12px; left: -8px;
  background: var(--primary); color: #fff; padding: 6px 12px;
  font-size: 12px; font-weight: 700; border-radius: 4px;
}

/* CTA final */
.cta-final { background: linear-gradient(180deg, var(--bg-soft), #ffffff); }
.cta-card { text-align: center; border: 1px solid #eaf4f8; }
.cta-card h3 { font-size: 24px; margin-bottom: 8px; color: var(--text); }
.cta-card p { color: var(--muted); margin-bottom: 16px; }
.cta-actions { display: flex; gap: 12px; justify-content: center; flex-wrap: wrap; }

/* Responsivo */
@media (max-width: 768px) {
  .hero-title { font-size: 32px; }
  .hero-subtitle { font-size: 16px; }
}
</style>
