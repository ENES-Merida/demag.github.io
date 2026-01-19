---
layout: page
title: Titúlate con Nosotros
subtitle: DeMAG
hero_image: /img/LaPlancha.webp
hero_height: is-medium
hero_darken: true
show_sidebar: false
---

{% include notification.html message="Sitio bajo construcción, actualizaremos la información muy pronto." %}
<div class="tabs is-centered is-boxed mb-5" id="OfertaTitulacion">
  <ul>
    <li class="is-active" data-target="home-titulacion">
      <a>
        <span class="icon is-small"
          ><i class="fas fa-user-graduate" aria-hidden="true"></i
        ></span>
        <span class="has-text-centered">Titúlate con<br>Nosotros</span>
      </a>
    </li>
    <li data-target="actividad-docencia-divulgacion">
      <a>
        <span class="icon is-small"
          ><i class="fas fa-chalkboard-teacher" aria-hidden="true"></i
        ></span>
        <span class="has-text-centered">Actividad de Apoyo a la<br>Docencia o la Divulgación</span>
      </a>
    </li>
    <li data-target="actividad-investigacion">
      <a>
        <span class="icon is-small"
          ><i class="fas fa-brain" aria-hidden="true"></i
        ></span>
        <span class="has-text-centered">Actividad de<br>Investigacion</span>
      </a>
    </li>
    <li data-target="actividad-profesional">
      <a>
        <span class="icon is-small"
          ><i class="fas fa-user-tie" aria-hidden="true"></i
        ></span>
        <span class="has-text-centered">Actividad<br>Profesional</span>
      </a>
    </li>
    <li data-target="tesis">
      <a>
        <span class="icon is-small"
          ><i class="fas fa-university" aria-hidden="true"></i
        ></span>
        <span class="has-text-centered">Proyecto de<br>Tesis</span>
      </a>
    </li>
  </ul>
</div>

<!--Contenido de cada tab-->
<div id="home-titulacion" class="tab-titu">
    {% include oferta-titulacion/titulate-con-nosotros.html %}
</div>
<div id="actividad-docencia-divulgacion" class="tab-titu is-hidden">
    {% include oferta-titulacion/actividad-docencia-divulgacion.html %}
</div>
<div id="actividad-investigacion" class="tab-titu is-hidden">
    {% include oferta-titulacion/actividad-investigacion.html %}
</div>
<div id="actividad-profesional" class="tab-titu is-hidden">
    {% include oferta-titulacion/actividad-profesional.html %}
</div>
<div id="tesis" class="tab-titu is-hidden">
    {% include oferta-titulacion/tesis.html %}
</div>
<script>
  const tabs = document.querySelectorAll('#OfertaTitulacion li');
  const tabContents = document.querySelectorAll('.tab-titu');
  tabs.forEach(tab => {
    tab.addEventListener('click', function() {
      tabs.forEach(t => t.classList.remove('is-active'));
      this.classList.add('is-active');
      const target = this.getAttribute('data-target');
      tabContents.forEach(content => {
        content.classList.add('is-hidden');
      });
      document.getElementById(target).classList.remove('is-hidden');
    });
  });
</script>
<hr>
<p>A tener en cuenta:</p>
<ul class="has-text-justified">
    <li>Independientemente de los créditos requeridos para cada modalidad de titulación, se requiere tener al menos <strong>75 por ciento</strong> de avance curricular para iniciar a trabajar en tu proceso de titulación.</li>
    <li>La vigencia del registro del anteproyecto de titulación, para todas las opciones, será de un año. En caso de transcurrir dicho periodo sin haber concluido el trabajo, el (la) sustentante podrá solicitar a su Comité Académico una renovación, que deberá ser avalada por el (la) asesor (a).</li>
</ul>
