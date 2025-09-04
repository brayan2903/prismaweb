<template>
  <WebLayout>
    <Head title="ERP PRISMA | Módulo de Tesorería — Gestión eficiente de fondos" />

    <!-- HERO / VALUE PROP -->
    <section class="hero">
      <a-row :gutter="[24,24]" align="middle">
        <a-col :xs="24" :md="14">
          <!-- <a-tag color="blue" class="hero-badge">Nuevo 2025</a-tag> -->
          <h1 class="hero-title">Módulo de Tesorería PRISMA</h1>
          <p class="hero-subtitle">
            Realiza la gestión total de los fondos de tu empresa, controla el flujo de caja, emite cheques y documentos, y proyecta saldos con total transparencia.
          </p>

          <ul class="hero-bullets">
            <li>💵 Integración con cuentas por pagar, cuentas por cobrar y contabilidad</li>
            <li>📊 Conciliación bancaria automática y control de transacciones bancarias</li>
            <li>📅 Programación de pagos, manejo de cheques y fondos de garantía</li>
            <li>🔄 Generación automática de asientos contables y aplicación de retenciones y detracciones</li>
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
            <img class="hero-image" src="/img_modulos/tesoreria.png" alt="Dashboard de Tesorería PRISMA" />
            <div class="ribbon">Gestión financiera eficiente</div>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- DESCRIPCIÓN DEL MÓDULO -->
    <section class="description">
      <h2 class="section-title">Descripción del Módulo de Tesorería</h2>
      <p>El Módulo de Tesorería de ERP Prisma le permite gestionar de manera eficiente todos los fondos de su empresa, desde la emisión de cheques hasta la conciliación bancaria, pasando por la programación de pagos y la gestión de retenciones y detracciones.</p>
    </section>

    <!-- BENEFICIOS PRINCIPALES -->
    <section class="features">
      <h2 class="section-title">Beneficios Principales</h2>
      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Integración Completa</template>
            <ul class="feature-list">
              <li>Integración fluida con las cuentas por pagar, cuentas por cobrar y la contabilidad.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Conciliación Bancaria Automática</template>
            <ul class="feature-list">
              <li>Realiza conciliaciones bancarias con un solo clic, facilitando el control del flujo de efectivo.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Gestión de Cheques y Pagos</template>
            <ul class="feature-list">
              <li>Generación automática de numeración de cheques por cuenta bancaria, y manejo de pagos a proveedores y otros gastos.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Proyección de Saldo y Fondos</template>
            <ul class="feature-list">
              <li>Proyecta el saldo de tus cuentas y gestiona los fondos de garantía de manera eficiente.</li>
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
            <template #title>Movimientos de Caja y Bancos</template>
            <ul class="feature-list">
              <li>Control total de los movimientos de caja y bancos, incluyendo ingresos, egresos y transferencias.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Programación de Pagos</template>
            <ul class="feature-list">
              <li>Gestiona la programación de pagos a proveedores y otros gastos de la empresa de forma eficiente.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Aplicación de Retenciones y Detracciones</template>
            <ul class="feature-list">
              <li>Aplica automáticamente retenciones y percepciones a documentos de clientes y proveedores.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Generación de Asientos Contables</template>
            <ul class="feature-list">
              <li>Generación automática de asientos contables de las operaciones de tesorería para una integración fluida con la contabilidad.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- REPORTES DEL MÓDULO -->
    <section class="reports">
      <h2 class="section-title">Reportes de Tesorería</h2>
      <ul>
        <li>Cheques emitidos y listados de pagos</li>
        <li>Balance de cuentas y estado de cuentas</li>
        <li>Transacciones de tesorería y documentos pendientes</li>
        <li>Conciliación Bancaria detallada</li>
      </ul>
    </section>

    <!-- CTA FINAL -->
    <section class="cta-final">
      <a-card class="cta-card" :hoverable="true">
        <h3>¿Listo para optimizar la gestión de tu tesorería?</h3>
        <p>Solicita una demo personalizada y descubre cómo PRISMA puede mejorar la administración de los fondos de tu empresa.</p>
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
  window.location.href = '/contacto?modulo=tesoreria'
}

const hablarVentas = () => {
  window.location.href = 'tel:+51010000000' // placeholder; cámbialo por tu número
}

const descargarBrochure = () => {
  window.location.href = '/brochure-tesoreria.pdf' // placeholder; súbelo a tu storage público
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
