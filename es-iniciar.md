---
layout: default
title: Ingreso MESLO
permalink: /es/iniciar/
lang: es
---

<article class="post intake-page">
  <header class="intake-hero">
    <p class="eyebrow">INGRESO MESLO</p>
    <h1 class="pageTitle">Cuéntanos dónde está tu negocio hoy.</h1>
    <p class="intro">
      Completa el siguiente formulario para entender cómo estás estimando, qué limitaciones operativas tienes y qué tipo de apoyo tiene más sentido para tu situación.
    </p>
  </header>

  <form
    name="meslo-intake-es"
    method="POST"
    action="{{ '/start-intake/thanks/' | relative_url }}"
    data-netlify="true"
    netlify-honeypot="bot-field"
    class="intake-form"
  >
    <input type="hidden" name="form-name" value="meslo-intake-es">
    <p class="hidden-field">
      <label class="no-asterisk">Don't fill this out if you're human: <input name="bot-field"></label>
    </p>

    <section class="intake-section">
      <h2>1. Información básica</h2>
      <div class="intake-grid intake-grid-2">
        <div class="field">
          <label for="full-name-es">Nombre completo</label>
          <input id="full-name-es" name="Nombre completo" type="text" required>
        </div>
        <div class="field">
          <label for="email-es">Correo electrónico</label>
          <input id="email-es" name="Correo electrónico" type="email" required>
        </div>
        <div class="field">
          <label for="phone-es">Número de teléfono</label>
          <input id="phone-es" name="Número de teléfono" type="tel" required>
        </div>
        <div class="field">
          <label for="company-es">Nombre de la empresa</label>
          <input id="company-es" name="Nombre de la empresa" type="text" required>
        </div>
      </div>
    </section>

    <section class="intake-section">
      <h2>2. Panorama del negocio</h2>
      <div class="field">
        <label>¿A qué tipo de trabajo te dedicas principalmente?</label>
        <div class="options">
          <label><input type="radio" name="Tipo de trabajo" value="Contratista general" required> Contratista general</label>
          <label><input type="radio" name="Tipo de trabajo" value="Subcontratista"> Subcontratista (HVAC, eléctrico, plomería, etc.)</label>
          <label><input type="radio" name="Tipo de trabajo" value="Empresa de servicios"> Empresa de servicios</label>
          <label><input type="radio" name="Tipo de trabajo" value="Negocio de productos"> Negocio de productos</label>
          <label><input type="radio" name="Tipo de trabajo" value="Otro"> Otro</label>
        </div>
      </div>

      <div class="field">
        <label>¿Cuál es el tamaño promedio de tus proyectos?</label>
        <div class="options">
          <label><input type="radio" name="Tamaño de proyectos" value="Menos de $10K" required> Menos de $10K</label>
          <label><input type="radio" name="Tamaño de proyectos" value="$10K - $50K"> $10K - $50K</label>
          <label><input type="radio" name="Tamaño de proyectos" value="$50K - $250K"> $50K - $250K</label>
          <label><input type="radio" name="Tamaño de proyectos" value="$250K+"> $250K+</label>
        </div>
      </div>

      <div class="field">
        <label>¿Cuál es tu ingreso mensual actual?</label>
        <div class="options">
          <label><input type="radio" name="Ingreso mensual" value="Menos de $50K" required> Menos de $50K</label>
          <label><input type="radio" name="Ingreso mensual" value="$50K - $150K"> $50K - $150K</label>
          <label><input type="radio" name="Ingreso mensual" value="$150K - $500K"> $150K - $500K</label>
          <label><input type="radio" name="Ingreso mensual" value="$500K+"> $500K+</label>
        </div>
      </div>
    </section>

    <section class="intake-section">
      <h2>3. Estado actual</h2>
      <div class="field">
        <label>¿Cómo estás estimando actualmente tus proyectos?</label>
        <div class="options">
          <label><input type="radio" name="Método de estimación" value="Hoja de cálculo" required> Hoja de cálculo (Excel, Google Sheets)</label>
          <label><input type="radio" name="Método de estimación" value="Papel y pluma"> Papel y pluma</label>
          <label><input type="radio" name="Método de estimación" value="Software"> Software (especificar)</label>
          <label><input type="radio" name="Método de estimación" value="Sin sistema"> No tengo un sistema consistente</label>
        </div>
      </div>

      <div class="field">
        <label>¿Conoces tus gastos generales y objetivos de utilidad reales?</label>
        <div class="options">
          <label><input type="radio" name="Conoce overhead/utilidad" value="Sí" required> Sí, claramente</label>
          <label><input type="radio" name="Conoce overhead/utilidad" value="Parcial"> Más o menos</label>
          <label><input type="radio" name="Conoce overhead/utilidad" value="No"> No</label>
        </div>
      </div>
    </section>

    <section class="intake-section">
      <h2>4. Identificación del problema</h2>
      <div class="field">
        <label>¿Cuál es tu mayor problema hoy? (Selecciona todos los que apliquen)</label>
        <div class="options checkbox-group">
          <label><input type="checkbox" name="Problema hoy" value="Cotizando por debajo del costo"> Estoy cotizando por debajo del costo</label>
          <label><input type="checkbox" name="Problema hoy" value="No conozco mis costos reales"> No conozco mis costos reales</label>
          <label><input type="checkbox" name="Problema hoy" value="Estimaciones inconsistentes"> Estimaciones inconsistentes</label>
          <label><input type="checkbox" name="Problema hoy" value="Problemas de flujo de efectivo"> Problemas de flujo de efectivo</label>
          <label><input type="checkbox" name="Problema hoy" value="Demasiado trabajo manual"> Demasiado trabajo manual</label>
          <label><input type="checkbox" name="Problema hoy" value="Sin sistemas claros"> No tengo sistemas claros</label>
          <label><input type="checkbox" name="Problema hoy" value="Problemas para escalar"> Problemas para escalar</label>
        </div>
      </div>
      <div class="field">
        <label for="problema-es">En una oración, ¿qué problema quieres resolver?</label>
        <textarea id="problema-es" name="Problema a resolver" rows="3" required></textarea>
      </div>
    </section>

    <section class="intake-section">
      <h2>5. Resultado deseado</h2>
      <div class="field">
        <label for="resultado-es">¿Cómo se vería el éxito en los próximos 90 días?</label>
        <textarea id="resultado-es" name="Resultado deseado" rows="3" required></textarea>
      </div>
    </section>

    <section class="intake-section">
      <h2>6. Nivel de preparación</h2>
      <div class="field">
        <label>¿Qué estás buscando?</label>
        <div class="options">
          <label><input type="radio" name="Nivel de preparación" value="DIY" required> Un sistema que pueda implementar yo mismo</label>
          <label><input type="radio" name="Nivel de preparación" value="Guía aplicada"> Guía aplicada a proyectos reales</label>
          <label><input type="radio" name="Nivel de preparación" value="Construir conmigo"> Alguien que construya sistemas conmigo</label>
          <label><input type="radio" name="Nivel de preparación" value="Soporte completo"> Soporte operativo completo</label>
        </div>
      </div>

      <div class="field">
        <label>¿Estás dispuesto a invertir en mejorar tus sistemas de estimación y operación?</label>
        <div class="options">
          <label><input type="radio" name="Disposición a invertir" value="Sí" required> Sí</label>
          <label><input type="radio" name="Disposición a invertir" value="Tal vez"> Tal vez</label>
          <label><input type="radio" name="Disposición a invertir" value="No"> No</label>
        </div>
      </div>
    </section>

    <section class="intake-section">
      <h2>7. Pregunta clave</h2>
      <div class="field">
        <label for="impacto-es">Si pudiéramos mejorar tu estimación y precios, ¿qué impacto tendría en tu negocio?</label>
        <textarea id="impacto-es" name="Impacto esperado" rows="3" required></textarea>
      </div>
    </section>

    <div class="form-actions">
      <button type="submit" class="button button-primary">Enviar información</button>
    </div>
  </form>
</article>
