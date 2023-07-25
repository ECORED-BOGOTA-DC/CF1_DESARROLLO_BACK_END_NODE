<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 2
      h1 MongoDB
    .row.align-items-center.mb-5
      .col-lg-4.mb-4.mb-lg-0
        figure
          img(src='@/assets/curso/tema2/img1.png', style="width: 370px" ,alt='Texto que describa la imagen').m-auto
      .col-lg-8
        p MongoDB es uno de los sistemas gestores de bases de datos NoSQL de tipo documental más famosos del mercado; su nombre viene del término en inglés humongous, que significa gigantesco. Ofrece un conjunto de soluciones, entre las que se incluye la posibilidad de trabajar con servidores que se pueden descargar y configurar en el equipo físico o servicios alojados en la nube por medio del gestor Atlas.
        p Este gestor de bases de datos NoSQL fue escrito en lenguaje C ++, pero todas las consultas usadas para la gestión de la información utilizan el formato BSON, que es similar al formato JSON, ampliamente utilizado por los desarrolladores web y móviles, para los procesos de transferencia de información a través de Internet.
        p.mb-0 Se presenta, entonces, la forma de hacer su instalación; luego, su configuración; y finalmente, su administración:
    .row.align-items-center.mb-4
      .col-auto.d-none.d-md-block.pe-0(style="z-index:2")
        figure
          img(src='@/assets/curso/tema1/img3.svg', style="width: 80px" ,alt='Texto que describa la imagen')
      .col-auto.bg-c3(style="z-index:1")
        .py-3.px-4
          h3.mb-0.ms-0.ms-md-4.text-white Instalación de MongoD
    .row.bg-c1.mb-5
      .col-12
        .px-5.pt-5
          .row.align-items-center.mb-5
            .col-12
              p.mb-0 A continuación, en el video, se muestra la forma en la que se realiza una instalación exitosa de una instancia gratuita de MongoDB y el servicio de gestión Cloud Atlas, accediendo a la dirección 
                |
                a(href="https://www.mongodb.com/es" target="_blank") www.mongodb.com
          figure
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    .row.align-items-center.mb-4
      .col-auto.d-none.d-md-block.pe-0(style="z-index:2")
        figure
          img(src='@/assets/curso/tema1/img3.svg', style="width: 80px" ,alt='Texto que describa la imagen')
      .col-auto.bg-c3(style="z-index:1")
        .py-3.px-4
          h3.mb-0.ms-0.ms-md-4.text-white Instalación de MongoD
    .row.bg-c1.mb-5
      .col-12
        .px-5.pt-5
          .row.align-items-center.mb-5
            .col-12
              p.mb-0 Posteriormente, el sistema ingresará al dashboard de configuración general de MongoDB, Atlas, en el que se recomienda realizar las configuraciones iniciales de seguridad. En este espacio, se establecen las credenciales de acceso necesarias para la gestión de la base de datos. Para conocer cómo se realiza este proceso, le invitamos a ver el siguiente video:
          figure
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    .row.align-items-center.mb-4
      .col-auto.d-none.d-md-block.pe-0(style="z-index:2")
        figure
          img(src='@/assets/curso/tema1/img3.svg', style="width: 80px" ,alt='Texto que describa la imagen')
      .col-auto.bg-c3(style="z-index:1")
        .py-3.px-4
          h3.mb-0.ms-0.ms-md-4.text-white Administración de MongoDB
    p.mb-5 Una vez terminada la configuración básica de seguridad, podrá acceder al dashboard para la administración general de la base de datos NoSQL. Tenga en cuenta que este servicio de base de datos se encuentra administrado por el proveedor Cloud seleccionado y que la base de datos se alberga en un clúster. Para conocer cómo se realizan los pasos de administración, vea lo siguiente:
    .row.align-items-center
      .col-lg-4.mb-4.mb-lg-0
        figure
          img(src='@/assets/curso/tema2/img1.svg', style="width: 370px" ,alt='Texto que describa la imagen').m-auto
      .col-lg-8
    Separador
    #t_2_1
    .titulo-segundo.color-acento-contenido
      h2 2.1. Documentos
    p.mb-5 Como ya se ha mencionado, MongoDB es un gestor de base de datos NoSQL, con una estructura basada en documentos. Por ello, es importante aclarar la jerarquía completa de esta estructuración de la información, la cual se muestra a través de la siguiente información:

</template>

<script>
export default {
  name: 'Tema2',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
