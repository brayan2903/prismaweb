<template>
  <WebLayout>
    <Head title="ERP PRISMA | Módulo de Almacén — Inventarios en tiempo real" />

    <!-- HERO / VALUE PROP -->
    <section class="hero">
      <a-row :gutter="[24,24]" align="middle">
        <a-col :xs="24" :md="14">
          <h1 class="hero-title">Módulo de Almacén PRISMA</h1>
          <p class="hero-subtitle">
            Gestiona de manera eficiente el control de bienes y productos en almacén, realiza movimientos detallados y controla el stock en tiempo real.
          </p>

          <ul class="hero-bullets">
            <li>📦 Gestión detallada por proveedor, categoría y marca</li>
            <li>⚙️ Control de movimientos internos, ajustes y transferencias</li>
            <li>📊 Kardex con valorización de inventario</li>
            <li>🔍 Reportes detallados de stock y movimientos</li>
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
            <img class="hero-image" src="/img_modulos/alm01.png" alt="Dashboard de almacén PRISMA" />
            <div class="ribbon">Inventario en vivo</div>
          </a-card>
        </a-col>
      </a-row>
    </section>

    <!-- DESCRIPCIÓN DEL MÓDULO -->
    <section class="description">
      <h2 class="section-title">Descripción del Módulo de Almacén</h2>
      <p>Este módulo tiene por finalidad gestionar el control estricto de bienes y productos de Almacén, registrando en detalle los movimientos originados por las operaciones del negocio, y también incluye el mantenimiento de vehículos y chóferes.</p>
    </section>

    <!-- CONTENIDO DEL MÓDULO -->
    <section class="content">
      <h2 class="section-title">Contenido del Módulo</h2>
      <ul>
        <li><strong>Configuración de Productos:</strong> El módulo mantiene la configuración de cada producto con las presentaciones, segmentado por proveedor, categoría, subcategoría, marca, foto, medidas del empaque y código de barra.</li>
        <li><strong>Operaciones:</strong> Transferencias entre almacenes y ajustes internos de inventarios como ingresos, mermas, premios, etc.</li>
        <li><strong>Kardex:</strong> El Kardex registra los movimientos de productos con valorización, cálculo de costos promedio ponderado y ofrece informes detallados por producto y almacén.</li>
        <li><strong>Control de Lotes:</strong> Controla lotes con fecha de vencimiento (opcional para algunos productos).</li>
        <li><strong>Historial de Compras:</strong> Consulta del historial de compras por lotes.</li>
        <li><strong>Reportes:</strong> Consultas y reportes detallados del stock actual, histórico, valorización y otros filtros como proveedor, categoría, etc.</li>
        <li><strong>Bienes Prestados:</strong> Ejemplo de registro de préstamos de envases a clientes, mostrando las operaciones de los bienes prestados.</li>
      </ul>
    </section>

    <!-- IMÁGENES DEL MÓDULO -->
    <section class="module-screenshots">
      <h2 class="section-title">Pantallas del Módulo</h2>
      <a-row :gutter="[24,24]">
        <a-col :xs="24" :md="8">
          <img class="module-image" src="/img_modulos/alm02.png" alt="Pantalla de Kardex" />
        </a-col>
        <a-col :xs="24" :md="8">
          <img class="module-image" src="/img_modulos/alm03.png" alt="Pantalla de Movimientos" />
        </a-col>
        <a-col :xs="24" :md="8">
          <img class="module-image" src="/img_modulos/alm04.png" alt="Pantalla de Transferencias" />
        </a-col>
      </a-row>
    </section>

    <!-- REPORTES DEL ALMACÉN -->
    <section class="reports">
      <h2 class="section-title">Reportes de Almacén</h2>
      <p>Los reportes permiten ver el stock actual o histórico de productos, con la opción de filtrar por almacén, proveedor, categoría y más. Los reportes pueden presentarse en formatos detallados o resumidos, mostrando peso y valorización.</p>
      <ul>
        <li>Reporte de Costo de Ventas, Saldo Valorizado y Transferencia entre Almacenes</li>
        <li>Registro de Inventarios Permanente de Unidades Físicas (PLE 12.1)</li>
        <li>Registro de Inventarios Permanente Valorizado (PLE 13.1)</li>
      </ul>
    </section>

    <!-- FUNCIONALIDADES ADICIONALES -->
    <section class="additional-features">
      <h2 class="section-title">Otras Funcionalidades</h2>
      <p>El módulo también incluye un verificador de stock en móviles, lo que permite hacer auditorías rápidas y asegurarse de que el inventario esté correctamente actualizado, todo desde tu dispositivo móvil.</p>
      <img class="module-image" src="/img_modulos/alm11.png" alt="Verificador de stock en móviles" />
    </section>

    <!-- CTA FINAL -->
    <section class="cta-final">
      <a-card class="cta-card" :hoverable="true">
        <h3>¿Listo para optimizar tu almacén?</h3>
        <p>Solicita una demo personalizada y descubre cómo PRISMA se adapta a tu operación.</p>
        <div class="cta-actions">
          <a-button type="primary" size="large" @click="contactar">Agendar demo</a-button>
          <a-button size="large" ghost @click="hablarVentas">Hablar con ventas</a-button>
        </div>
      </a-card>
    </section>
  </WebLayout>
</template>

<script setup>
import WebLayout from '@/Layouts/WebLayout.vue'
import { Head } from '@inertiajs/vue3'

const contactar = () => {
  window.location.href = '/contacto?modulo=almacen'
}

const hablarVentas = () => {
  window.location.href = 'tel:+51010000000' // placeholder; cámbialo por tu número
}

const descargarBrochure = () => {
  window.location.href = '/brochure-almacen.pdf' // placeholder; súbelo a tu storage público
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

/* Pantallas del Módulo */
.module-screenshots .module-image {
  width: 100%;
  height: auto;
  display: block;
}

/* Beneficios */
.benefits { background: #fff; }

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
