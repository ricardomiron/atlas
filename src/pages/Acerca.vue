<template>
  <Layout>
    <section id="about">
      <div class="container">
        <!-- Agregar comunidad -->
        <div class="row flex-center">
          <div
            class="col-md-12 col-lg-4 mb-4 mt-4 d-flex align-items-center justify-content-center order-lg-0 order-md-0"
          >
            <g-image
              src="~/assets/images/collab.png"
              alt="Construyamos juntos"
              class="img-fluid"
            />
          </div>
          <div
            class="col-md-12 col-lg-8 text-md-start order-lg-1 order-md-1"
            style="max-width: 460px;"
          >
            <h1 id="nueva-comunidad" class="fw-bold display-4 mb-4 mt-4">
              ¿Cómo agrego una comunidad?
            </h1>
            <p class="text-dark">
              Agregar una comunidad al Atlas es muy sencillo, por ahora existen
              2 formas 👇
            </p>
            <ul class="text-dark">
              <li>
                💻 Clona el
                <a href="https://github.com/devspacemx/atlas" target="_blank"
                  >repositorio de GitHub</a
                >
                del Atlas de comunidades y agrega un registro en forma de
                archivo markdown al registro de comunidades, sigue las
                instrucciones en el archivo <b>README.md</b> en la raíz del
                repositorio.<br />Una vez que termines de hacer los cambios,
                crea un Pull Request y un mantainer del repositorio aprobará los
                cambios.
              </li>
              <li>
                📄 Llena este
                <a href="https://forms.gle/o4CeeMgSaJbXE7896" target="_blank"
                  >formulario de Google Docs</a
                >
                con los datos que se te solicitan, una vez hayamos agregado tu
                comunidad al registro te notificaremos por correo electrónico.
              </li>
            </ul>
          </div>
        </div>
        <!-- El Atlas -->
        <div class="row flex-center">
          <div
            class="col-md-12 col-lg-4 mb-4 d-flex align-items-center justify-content-center order-lg-1 order-md-0"
          >
            <g-image
              src="~/assets/images/latam.png"
              alt="Comunidades LATAM"
              class="img-fluid mb-1"
            />
          </div>
          <div
            class="col-md-12 col-lg-8 text-md-start order-lg-0 order-md-1"
            style="max-width: 460px;"
          >
            <h1 class="fw-bold display-4 mb-4 mt-2">
              El Atlas<br />de comunidades 🌎
            </h1>
            <p class="text-dark">
              La razón de esta plataforma es el reconocimiento a todas las
              comunidades de tecnología y el crecimiento fenomenal que han
              tenido desde hace unos años.
            </p>
            <p class="text-dark">
              En toda Latinoamérica podemos encontrar distintas comunidades, ya
              sean de tecnologías en general o muy específicas, todas nacen
              gracias a las necesidades y oportunidades que hay en cada país.
            </p>
            <p class="mt-2 text-dark">
              Las de software, las de hardware, las de emprendimiento y
              <b>más...</b>
              Todas participando activamente en generar conocimiento y
              experiencias para sus miembros.
            </p>
          </div>
        </div>
        <!-- Por qué -->
        <div class="row flex-center">
          <div
            class="col-md-12 col-lg-4 mb-4 d-flex align-items-center justify-content-center order-lg-1 order-md-0"
          >
            <g-image
              src="~/assets/images/people.png"
              alt="Personas"
              class="img-fluid"
            />
          </div>
          <div
            class="col-md-12 col-lg-8 text-md-start order-lg-0 order-md-1"
            style="max-width: 460px;"
          >
            <h2 class="fw-bold display-5 mb-4 mt-4">¿Por qué?</h2>
            <p class="text-dark">
              Para que las personas puedan encontrar comunidades de su interés y
              hacer nuevas amistades.
            </p>
            <p class="text-dark">
              Para que las comunidades puedan encontrar otros grupos con causas
              en común y hacer sinergia.
            </p>
            <p class="text-dark">
              Para que todos podamos aprender de todos, cuando las comunidades
              crecen ¡Todos nos fortalecemos!
            </p>
            <a
              class="btn btn-info me-1 text-truncate"
              :href="'https://twitter.com/intent/tweet?text=' + shareText"
              target="_blank"
              rel="noreferrer"
              role="button"
              >Comparte con tu red</a
            >
          </div>
        </div>
      </div>
    </section>
  </Layout>
</template>

<script>
import { metaInfo } from "../data";

export default {
  metaInfo() {
    return metaInfo(this.$seo, "¿Qué es?", true);
  },
  data() {
    return {
      shareText:
        "🔎 ¿Ya conoces Atlas?%0aDescubre esta plataforma dónde se reunen las comunidades tecnológicas en Latinoamérica 🌎 %0aConoce más sobre el proyecto en 👉 https://comunidades.lat/",
    };
  },
};
</script>

<style lang="scss"></style>
