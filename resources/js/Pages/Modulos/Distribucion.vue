<template>
  <WebLayout>
    <Head title="ERP PRISMA | Módulo de Distribución — Gestión eficiente de ventas y cobranza" />

    <!-- HERO / VALUE PROP -->
    <section class="hero">
      <a-row :gutter="[24,24]" align="middle">
        <a-col :xs="24" :md="14">
          <h1 class="hero-title">Módulo de Distribución PRISMA</h1>
          <p class="hero-subtitle">
            Optimiza tus operaciones comerciales con ventas por distribución masiva, desde la pre-venta hasta la auto venta, con total trazabilidad y control.
          </p>

          <ul class="hero-bullets">
            <li>📦 Ingreso masivo de pedidos y control de documentos vencidos</li>
            <li>⚙️ Autorización de pedidos observados y políticas de ventas personalizables</li>
            <li>🚚 Planificación de despachos y traspaso de pedidos a documentos de venta</li>
            <li>📊 Reportes multidimensionales de ventas y cobranzas</li>
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
            <img class="hero-image" src="/img_modulos/11.jpg" alt="Dashboard de Distribución PRISMA" />
            <div class="ribbon">Gestión de distribución eficiente</div>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- DESCRIPCIÓN DEL MÓDULO -->
    <section class="description">
      <h2 class="section-title">Descripción del Módulo de Distribución</h2>
      <p>El Módulo de Distribución de ERP Prisma está diseñado para empresas dedicadas a la distribución masiva de productos, con funcionalidades de pre-venta, auto-venta y control total de operaciones comerciales.</p>
    </section>

    <!-- BENEFICIOS PRINCIPALES -->
    <section class="features">
      <h2 class="section-title">Beneficios Principales</h2>
      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Ingreso Masivo de Pedidos</template>
            <ul class="feature-list">
              <li>Permite digitar y observar pedidos con documentos vencidos, límite de crédito excedido y aplicar políticas de ventas.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Autorización de Pedidos Observados</template>
            <ul class="feature-list">
              <li>Le permite visualizar el motivo de un pedido observado y tomar decisiones de aprobación o modificación.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Traspaso a Documentos de Venta</template>
            <ul class="feature-list">
              <li>Los pedidos aprobados se convierten en facturas o boletas y se fraccionan según el formato de documentos físicos.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Impresión Masiva de Documentos</template>
            <ul class="feature-list">
              <li>Impresión masiva de facturas, boletas, notas de crédito y guías de remisión por lote o individualmente.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Planificación de Despachos</template>
            <ul class="feature-list">
              <li>Creación de planillas de reparto, control de capacidad de vehículos y consolidado de documentos para el reparto.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Reportes de Cuentas por Cobrar</template>
            <ul class="feature-list">
              <li>Obtiene reportes de documentos pendientes por cobrar, filtrados por vendedor, zona y fecha de emisión.</li>
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
            <template #title>Ventas con Códigos de Barra</template>
            <ul class="feature-list">
              <li>Venta y compra con códigos de barras para agilizar el proceso de pedidos y ventas.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Liquidación de Cobranzas</template>
            <ul class="feature-list">
              <li>Liquidación de documentos rechazados y devoluciones parciales, con registro de cobranzas realizadas por planilla.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>

      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Planificación de Ventas y Coberturas</template>
            <ul class="feature-list">
              <li>Medición de la cobertura de ventas y efectividad de la planificación comercial, con estadísticas de avance.</li>
            </ul>
          </a-card>
        </a-col>
        <a-col :xs="24" :md="12">
          <a-card class="list-card" :hoverable="true">
            <template #title>Ranking de Ventas y Clientes</template>
            <ul class="feature-list">
              <li>Consulta de ventas agrupadas por clientes, con clasificación de ventas por vendedor y estadísticas de rendimiento.</li>
            </ul>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- REPORTES DEL MÓDULO -->
    <section class="reports">
      <h2 class="section-title">Reportes de Distribución</h2>
      <ul>
        <li>Hoja de Ruta y listado de clientes por día de visita</li>
        <li>Cuadro de Visitas de Vendedores por semanas</li>
        <li>Acumulado de mercadería devuelta según planillas de reparto</li>
        <li>Consulta multidimensional de cobranzas y cuentas por cobrar</li>
        <li>Ranking de ventas por cliente y estadísticas de venta vs stock</li>
      </ul>
    </section>

    <!-- IMÁGENES ADICIONALES -->
    <section class="images">
      <h2 class="section-title">Visualiza el Módulo en Acción</h2>
      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="8">
          <img class="module-image" src="/img_modulos/12.jpg" alt="Pantalla de Traspaso de Pedidos" />
        </a-col>
        <a-col :xs="24" :md="8">
          <img class="module-image" src="/img_modulos/13.jpg" alt="Pantalla de Reportes y Cobranzas" />
        </a-col>
      </a-row>
    </section>

    <!-- CTA FINAL -->
    <section class="cta-final">
      <a-card class="cta-card" :hoverable="true">
        <h3>¿Listo para optimizar tu distribución?</h3>
        <p>Solicita una demo personalizada y descubre cómo PRISMA puede mejorar la eficiencia de tus operaciones de distribución.</p>
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
  window.location.href = '/contacto?modulo=distribucion'
}

const hablarVentas = () => {
  window.location.href = 'tel:+51010000000' // placeholder; cámbialo por tu número
}

const descargarBrochure = () => {
  window.location.href = '/brochure-distribucion.pdf' // placeholder; súbelo a tu storage público
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
