<template>
  <WebLayout>
    <Head title="ERP PRISMA | Módulo de Compras y Logística — Toma de decisiones inteligentes" />

    <!-- HERO / VALUE PROP -->
    <section class="hero">
      <a-row :gutter="[24,24]" align="middle">
        <a-col :xs="24" :md="14">
          <h1 class="hero-title">Módulo de Compras y Logística PRISMA</h1>
          <p class="hero-subtitle">
            Toma decisiones inteligentes sobre compras y abastecimiento, optimiza tus órdenes de compra y controla la logística con total flexibilidad.
          </p>

          <ul class="hero-bullets">
            <li>📊 Optimización de compras basada en promedios de ventas</li>
            <li>⚙️ Generación automática de órdenes de compra</li>
            <li>📦 Abastecimiento eficiente de almacén, local y extranjero</li>
            <li>🔍 OLAP: Consultas multidimensionales para tomar decisiones rápidas</li>
          </ul>

          <!-- <div class="hero-cta">
            <a-button type="primary" size="large" @click="contactar">
              Solicitar demostración
            </a-button>
            <a-button size="large" @click="descargarBrochure" class="cta-secondary">
              Descargar brochure (PDF)
            </a-button>
          </div> -->
        </a-col>

        <a-col :xs="24" :md="10">
          <a-card :hoverable="true" class="hero-card" :bodyStyle="{ padding: '0' }">
            <img class="hero-image" src="/img_modulos/comp1.jpeg" alt="Dashboard de Compras y Logística PRISMA" />
            <div class="ribbon">Gestión de compras eficiente</div>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- DESCRIPCIÓN DEL MÓDULO -->
    <section class="description">
      <h2 class="section-title">Descripción del Módulo de Compras y Logística</h2>
      <p>El Módulo de Compras y Logística en ERP Prisma le ayuda a tomar decisiones inteligentes respecto a qué, cuándo, cuánto y a quién comprar, optimizando tanto el proceso de compras como el abastecimiento de almacén.</p>
    </section>

    <!-- FUNCIONALIDADES PRINCIPALES -->
    <section class="features">
      <h2 class="section-title">Características Principales</h2>
      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Padrón de Proveedores y Configuración de Productos</template>
            <ul class="feature-list">
              <li>Mantiene el padrón de proveedores y configura los productos con sus presentaciones, categorías y combos.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Toma de Decisiones para Abastecimiento</template>
            <ul class="feature-list">
              <li>Proyecta el número de días de abastecimiento tomando en cuenta los promedios de ventas de cada producto.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Generación Automática de Órdenes de Compra</template>
            <ul class="feature-list">
              <li>Genera órdenes de compra de manera automática, basándose en el stock actual, las compras anteriores y el costo del producto.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Ingreso de Documentos de Compra</template>
            <ul class="feature-list">
              <li>Permite ingresar documentos de compra con cálculo de costos y actualización en el Kardex y stock.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Órdenes de Servicio</template>
            <ul class="feature-list">
              <li>Genera órdenes de servicio y documentos de compra de servicios de manera directa, detallando toda la información relevante.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>OLAP: Consulta Multidimensional de Compras</template>
            <ul class="feature-list">
              <li>Accede a consultas multidimensionales de compras para tomar decisiones rápidas y ajustadas a las necesidades del negocio.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- CTA FINAL -->
    <section class="cta-final">
      <a-card class="cta-card" :hoverable="true">
        <h3>¿Listo para mejorar tus compras y logística?</h3>
        <p>Solicita una demo personalizada y descubre cómo PRISMA puede optimizar tus decisiones de compras y abastecimiento.</p>
        <div class="cta-actions">
          <a-button type="primary" size="large" @click="contactar">Contactarse</a-button>
        </div>
      </a-card>
    </section>
  </WebLayout>
</template>

<script setup>
import WebLayout from '@/Layouts/WebLayout.vue'
import { Head } from '@inertiajs/vue3'

const contactar = () => {
  window.location.href = '/contacto?modulo=compras'
}

const hablarVentas = () => {
  window.location.href = 'tel:+51010000000' // placeholder; cámbialo por tu número
}

const descargarBrochure = () => {
  window.location.href = '/brochure-compras.pdf' // placeholder; súbelo a tu storage público
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
