<template>
  <WebLayout>
    <Head title="ERP PRISMA | Módulo de Producción — Gestión eficiente de la producción" />

    <!-- HERO / VALUE PROP -->
    <section class="hero">
      <a-row :gutter="[24,24]" align="middle">
        <a-col :xs="24" :md="14">
          <a-tag color="blue" class="hero-badge">Nuevo 2025</a-tag>
          <h1 class="hero-title">Módulo de Producción PRISMA</h1>
          <p class="hero-subtitle">
            Gestiona todos los procesos de producción con una potente herramienta de planificación, controlando recursos y materiales de forma eficiente.
          </p>

          <ul class="hero-bullets">
            <li>⚙️ Planificación automática de órdenes de producción</li>
            <li>💼 Gestión de operarios, máquinas, y costos por hora</li>
            <li>📊 Reportes detallados de costos y eficiencia</li>
            <li>🔄 Integración completa con compras, ventas e inventarios</li>
          </ul>

          <div class="hero-cta">

          </div>
        </a-col>

        <a-col :xs="24" :md="10">
          <a-card :hoverable="true" class="hero-card" :bodyStyle="{ padding: '0' }">
            <img class="hero-image" src="/img_modulos/pro1.jpeg" alt="Dashboard de Producción PRISMA" />
            <div class="ribbon">Gestión de producción eficiente</div>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- DESCRIPCIÓN DEL MÓDULO -->
    <section class="description">
      <h2 class="section-title">Descripción del Módulo de Producción</h2>
      <p>El Módulo de Producción de ERP Prisma le permite gestionar todos los procesos que intervienen en la fabricación de un producto, con una potente herramienta de planificación que le permitirá controlar la carga de los recursos y gestionar las necesidades de los materiales.</p>
    </section>

    <!-- BENEFICIOS PRINCIPALES -->
    <section class="features">
      <h2 class="section-title">Beneficios Principales</h2>
      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Generación Automática de Órdenes de Producción</template>
            <ul class="feature-list">
              <li>Generación automática de órdenes de producción para productos terminados, semi-elaborados o intermedios.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Control de Producción Intermedia</template>
            <ul class="feature-list">
              <li>Registro de avances de producción mediante la carga de vales de producción intermedia.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Gestión de Operarios y Costos</template>
            <ul class="feature-list">
              <li>Indicación de operarios, costos por hora, control de máquinas y procesos de producción.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Costeo y Control de Órdenes de Producción</template>
            <ul class="feature-list">
              <li>Permite costear y controlar órdenes de producción que abarcan más de un período contable.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Gestión de Recetas</template>
            <ul class="feature-list">
              <li>Permite manejar múltiples alternativas de recetas para la producción de un mismo artículo o ingresar insumos sin receta.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Distribución de Gastos de Fabricación</template>
            <ul class="feature-list">
              <li>Distribuye los gastos de fabricación proporcionalmente a las órdenes de trabajo.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Control de Ingresos y Salidas</template>
            <ul class="feature-list">
              <li>Controla los ingresos y salidas de productos (materiales, insumos, empaques y productos terminados).</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Gestión Integral de Compras, Ventas e Inventarios</template>
            <ul class="feature-list">
              <li>Integración total con las compras, ventas e inventarios para un control eficiente de la producción.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- REPORTES DEL MÓDULO -->
    <section class="reports">
      <h2 class="section-title">Reportes de Producción</h2>
      <ul>
        <li>Costo por Producción</li>
        <li>Costo Acumulado por Producto</li>
        <li>Reporte de Productos Usados o Insumos</li>
        <li>Reporte Costo por Recurso Humano</li>
        <li>Reporte por Maquina</li>
        <li>Reporte por Centro de Producción</li>
        <li>Reporte por Hoja de Costos</li>
        <li>Estado de Costo de Valorizado Anual</li>
      </ul>
    </section>

    <!-- CTA FINAL -->
    <section class="cta-final">
      <a-card class="cta-card" :hoverable="true">
        <h3>¿Listo para optimizar tu proceso de producción?</h3>
        <p>Solicita una demo personalizada y descubre cómo PRISMA puede transformar tu proceso productivo.</p>
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
  window.location.href = '/contacto?modulo=produccion'
}

const hablarVentas = () => {
  window.location.href = 'tel:+51010000000' // placeholder; cámbialo por tu número
}

const descargarBrochure = () => {
  window.location.href = '/brochure-produccion.pdf' // placeholder; súbelo a tu storage público
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
