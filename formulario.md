---
layout: default
title: Formulario
permalink: /formulario/
lang: es
lang_alt_url: /intake/
---

<article class="post intake-page">
  <header class="intake-hero">
    <p class="eyebrow">INTAKE MESLO</p>
    <h1 class="pageTitle">Cuentanos en que punto esta tu negocio hoy.</h1>
    <p class="intro">
      Completa el formulario a continuacion para entender tu proceso actual de
      estimacion, las limitaciones de tu operacion y el tipo de apoyo que
      tiene mas sentido para ti.
    </p>
  </header>

  <form
    name="meslo-intake-es"
    method="POST"
    action="{{ '/formulario/gracias/' | relative_url }}"
    data-netlify="true"
    netlify-honeypot="bot-field"
    class="intake-form"
  >
    <input type="hidden" name="form-name" value="meslo-intake-es">
    <p class="hidden-field">
      <label>No llenes este campo si eres humano: <input name="bot-field"></label>
    </p>

    <section class="intake-section">
      <h2>1. Informacion Basica</h2>
      <div class="intake-grid intake-grid-2">
        <div class="field">
          <label for="nombre-completo">Nombre Completo</label>
          <input id="nombre-completo" name="Nombre Completo" type="text" required>
        </div>
        <div class="field">
          <label for="correo-electronico">Correo Electronico</label>
          <input id="correo-electronico" name="Correo Electronico" type="email" required>
        </div>
        <div class="field">
          <label for="numero-telefono">Numero de Telefono</label>
          <input id="numero-telefono" name="Numero de Telefono" type="text" required>
        </div>
        <div class="field">
          <label for="nombre-empresa">Nombre de la Empresa</label>
          <input id="nombre-empresa" name="Nombre de la Empresa" type="text" required>
        </div>
      </div>
    </section>

    <section class="intake-section">
      <h2>2. Panorama del Negocio</h2>
      <div class="field">
        <fieldset>
          <legend>A que tipo de trabajo te dedicas principalmente?</legend>
          <label><input type="radio" name="Tipo Principal de Trabajo" value="Contratista General" required> Contratista General</label>
          <label><input type="radio" name="Tipo Principal de Trabajo" value="Subcontratista"> Subcontratista (HVAC, Electrico, Plomeria, etc.)</label>
          <label><input type="radio" name="Tipo Principal de Trabajo" value="Negocio de Servicios"> Negocio de Servicios</label>
          <label><input type="radio" name="Tipo Principal de Trabajo" value="Negocio de Productos"> Negocio de Productos</label>
          <label><input type="radio" name="Tipo Principal de Trabajo" value="Otro"> Otro</label>
          <input name="Tipo Principal de Trabajo Otro" type="text" placeholder="Si es otro, especifica">
        </fieldset>
      </div>

      <div class="field">
        <fieldset>
          <legend>Cual es el tamano promedio de tus trabajos?</legend>
          <label><input type="radio" name="Tamano Promedio de Trabajo" value="Menos de $10K" required> Menos de $10K</label>
          <label><input type="radio" name="Tamano Promedio de Trabajo" value="$10K - $50K"> $10K - $50K</label>
          <label><input type="radio" name="Tamano Promedio de Trabajo" value="$50K - $250K"> $50K - $250K</label>
          <label><input type="radio" name="Tamano Promedio de Trabajo" value="Mas de $250K"> Mas de $250K</label>
        </fieldset>
      </div>

      <div class="field">
        <fieldset>
          <legend>Cual es tu ingreso mensual actual?</legend>
          <label><input type="radio" name="Ingreso Mensual Actual" value="Menos de $50K" required> Menos de $50K</label>
          <label><input type="radio" name="Ingreso Mensual Actual" value="$50K - $150K"> $50K - $150K</label>
          <label><input type="radio" name="Ingreso Mensual Actual" value="$150K - $500K"> $150K - $500K</label>
          <label><input type="radio" name="Ingreso Mensual Actual" value="Mas de $500K"> Mas de $500K</label>
        </fieldset>
      </div>
    </section>

    <section class="intake-section">
      <h2>3. Situacion Actual</h2>
      <div class="field">
        <fieldset>
          <legend>Como estas estimando tus trabajos actualmente?</legend>
          <label><input type="radio" name="Metodo Actual de Estimacion" value="Hoja de calculo (Excel)" required> Hoja de calculo (Excel)</label>
          <label><input type="radio" name="Metodo Actual de Estimacion" value="Papel y pluma"> Papel y pluma</label>
          <label><input type="radio" name="Metodo Actual de Estimacion" value="Software"> Software (especifica)</label>
          <label><input type="radio" name="Metodo Actual de Estimacion" value="No tengo un sistema consistente"> No tengo un sistema consistente</label>
          <input name="Software de Estimacion" type="text" placeholder="Si usas software, especifica">
        </fieldset>
      </div>

      <div class="field">
        <fieldset>
          <legend>Conoces tus gastos reales (overhead) y metas de ganancia?</legend>
          <label><input type="radio" name="Claridad de Overhead y Ganancia" value="Si, claramente" required> Si, claramente</label>
          <label><input type="radio" name="Claridad de Overhead y Ganancia" value="Mas o menos"> Mas o menos</label>
          <label><input type="radio" name="Claridad de Overhead y Ganancia" value="No"> No</label>
        </fieldset>
      </div>
    </section>

    <section class="intake-section">
      <h2>4. Identificacion del Problema</h2>
      <div class="field">
        <fieldset>
          <legend>Cual es tu mayor problema en este momento? (Selecciona todos los que apliquen)</legend>
          <label><input type="checkbox" name="Problemas Principales" value="Cotizar por debajo (perder dinero)"> Cotizar por debajo (perder dinero)</label>
          <label><input type="checkbox" name="Problemas Principales" value="No conocer los costos reales"> No conocer los costos reales</label>
          <label><input type="checkbox" name="Problemas Principales" value="Estimaciones inconsistentes"> Estimaciones inconsistentes</label>
          <label><input type="checkbox" name="Problemas Principales" value="Problemas de flujo de efectivo"> Problemas de flujo de efectivo</label>
          <label><input type="checkbox" name="Problemas Principales" value="Demasiado trabajo manual"> Demasiado trabajo manual</label>
          <label><input type="checkbox" name="Problemas Principales" value="Falta de sistemas claros"> Falta de sistemas claros</label>
          <label><input type="checkbox" name="Problemas Principales" value="Dificultad para crecer"> Dificultad para crecer</label>
        </fieldset>
      </div>

      <div class="field">
        <label for="problema-principal">En una sola oracion, cual es el principal problema que quieres resolver?</label>
        <textarea id="problema-principal" name="Principal Problema a Resolver" required></textarea>
      </div>
    </section>

    <section class="intake-section">
      <h2>5. Resultado Deseado</h2>
      <div class="field">
        <label for="exito-90-dias">Como se veria el exito en los proximos 90 dias?</label>
        <textarea id="exito-90-dias" name="Definicion de Exito en 90 Dias" required></textarea>
      </div>
    </section>

    <section class="intake-section">
      <h2>6. Nivel de Preparacion</h2>
      <div class="field">
        <fieldset>
          <legend>Que estas buscando?</legend>
          <label><input type="radio" name="Lo Que Esta Buscando" value="Un sistema que pueda implementar yo mismo" required> Un sistema que pueda implementar yo mismo</label>
          <label><input type="radio" name="Lo Que Esta Buscando" value="Guia sobre trabajos reales"> Guia sobre trabajos reales</label>
          <label><input type="radio" name="Lo Que Esta Buscando" value="Alguien que me ayude a construir sistemas"> Alguien que me ayude a construir sistemas</label>
          <label><input type="radio" name="Lo Que Esta Buscando" value="Apoyo operativo completo"> Apoyo operativo completo</label>
        </fieldset>
      </div>

      <div class="field">
        <fieldset>
          <legend>Estas preparado para invertir en mejorar tus sistemas de estimacion y operacion?</legend>
          <label><input type="radio" name="Disposicion de Inversion" value="Si" required> Si</label>
          <label><input type="radio" name="Disposicion de Inversion" value="Tal vez"> Tal vez</label>
          <label><input type="radio" name="Disposicion de Inversion" value="No"> No</label>
        </fieldset>
      </div>
    </section>

    <section class="intake-section">
      <h2>7. Pregunta Clave</h2>
      <div class="field">
        <label for="impacto-negocio">Si logramos mejorar tu estimacion y precios, que impacto tendria en tu negocio?</label>
        <textarea id="impacto-negocio" name="Impacto en el Negocio al Mejorar Estimacion y Precios" required></textarea>
      </div>
    </section>

    <div class="intake-actions">
      <button class="button" type="submit">Enviar Formulario</button>
    </div>
  </form>
</article>
