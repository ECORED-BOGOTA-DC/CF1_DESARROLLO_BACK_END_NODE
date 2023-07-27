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
          h3.mb-0.ms-0.ms-md-4.text-white Configuración de MongoDB
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
        .tarjeta.tarjeta--gris.p-4
          PasosB.color-acento-contenido
            .row(titulo="")
              .col-12
                .p-4
                  p #[b Paso 1]
                  p Si es la primera vez que intenta manipular bases de datos NoSQL documentales, se recomienda seguir las sugerencias de Atlas y crear una base de datos de prueba para realizar operaciones y consultas de prueba sobre la misma, a manera de entrenamiento. Esto puede tardar un par de minutos adicionales.
                  .row
                    .col-auto
                      a.boton.color-acento-botones.indicador__container(@click="modal1 = true")
                        span #[b #[i(style="color: #12263F") Data base]]
                        .indicador--click(v-if="mostrarIndicador")
                    .col-auto
                      a.boton.color-acento-botones.indicador__container(@click="modal2 = true")
                        span #[b #[i(style="color: #12263F") Load Sample]]
                        .indicador--click(v-if="mostrarIndicador")
            .row(titulo="")
              .col-12
                .p-4
                  p #[b Paso 2]
                  p Dentro de la misma información de la base de datos, podrá acceder a las opciones de conexión al clúster. Recuerde que los sistemas de bases de datos NoSQL están concebidos para ser administrados por APIS externas construidas por los desarrolladores; por esta razón, el sistema le preguntará el medio de conexión preferido.
                  .row
                    .col-auto
                      a.boton.color-acento-botones.indicador__container(@click="modal3 = true")
                        span #[b #[i(style="color: #12263F") Connect]]
                        .indicador--click(v-if="mostrarIndicador")
            .row(titulo="")
              .col-12
                .p-4
                  p #[b Paso 3]
                  p Si desea conectarse por medio de una terminal de comandos (MongoDB Shell), le serán recomendados, de acuerdo al sistema operativo, los comandos o instalaciones previas a realizar, junto con la cadena de conexión que deberá ejecutar en su terminal para establecer una conexión exitosa con la base de datos.
                  .row
                    .col-auto
                      a.boton.color-acento-botones.indicador__container(@click="modal4 = true")
                        span #[b #[i(style="color: #12263F") Connect]]
                        .indicador--click(v-if="mostrarIndicador")
                    .col-auto
                      a.boton.color-acento-botones.indicador__container(@click="modal5 = true")
                        span #[b #[i(style="color: #12263F") Connect]]
                        .indicador--click(v-if="mostrarIndicador")
            .row(titulo="")
              .col-12
                .p-4
                  p #[b Paso 4]
                  p Una vez finalizada la instalación del #[i shell] de Mongo, pruebe utilizar el comando de conexión provisto por Atlas; tenga en cuenta que esta cadena de conexión utilizará el usuario creado anteriormente en la configuración de seguridad.
                  .row
                    .col-auto
                      a.boton.color-acento-botones.indicador__container(@click="modal6 = true")
                        span #[b #[i(style="color: #12263F") Connect]]
                        .indicador--click(v-if="mostrarIndicador")
            .row(titulo="")
              .col-12
                .p-4
                  p #[b Paso 5]
                  p Si lo desea, también puede explorar y gestionar las estructuras creadas en la base de datos directamente desde el portal de MongoDB Atlas, por medio de la opción Browse Collections.
                  .row
                    .col-auto
                      a.boton.color-acento-botones.indicador__container(@click="modal7 = true")
                        span #[b #[i(style="color: #12263F") Connect]]
                        .indicador--click(v-if="mostrarIndicador")
            .row(titulo="")
              .col-12
                .p-4
                  p #[b Paso 6]
                  p El sistema desplegará todas las bases de datos en un panel del lado izquierdo, en el que podrá seleccionar alguna de estas y consultar las colecciones existentes. En el panel central, tendrá un espacio de ejecución de comandos sobre la base de datos seleccionada, y en la parte inferior, se desplegará el resultado de la ejecución de los comandos. Por defecto, desplegará todos los documentos existentes si es que tiene seleccionada una colección de la base de datos.
                  .row
                    .col-auto
                      a.boton.color-acento-botones.indicador__container(@click="modal8 = true")
                        span #[b #[i(style="color: #12263F") Connect]]
                        .indicador--click(v-if="mostrarIndicador")
    ModalA(:abrir-modal.sync="modal1")
      .row
        .col-12
          figure
            img(src='@/assets/curso/tema2/img1.jpg', style="width: 1200px" ,alt='Texto que describa la imagen').m-auto
    ModalA(:abrir-modal.sync="modal2")
      .row
        .col-12
          figure
            img(src='@/assets/curso/tema2/img2.jpg', style="width: 600px" ,alt='Texto que describa la imagen').m-auto
    ModalA(:abrir-modal.sync="modal3")
      .row
        .col-12
          figure
            img(src='@/assets/curso/tema2/img3.jpg', style="width: 900px" ,alt='Texto que describa la imagen').m-auto
    ModalA(:abrir-modal.sync="modal4")
      .row
        .col-12
          figure
            img(src='@/assets/curso/tema2/img4.jpg', style="width: 550px" ,alt='Texto que describa la imagen').m-auto
    ModalA(:abrir-modal.sync="modal5")
      .row
        .col-12
          figure
            img(src='@/assets/curso/tema2/img5.jpg', style="width: 550px" ,alt='Texto que describa la imagen').m-auto
    ModalA(:abrir-modal.sync="modal6")
      .row
        .col-12
          figure
            img(src='@/assets/curso/tema2/img6.jpg', style="width: 1200px" ,alt='Texto que describa la imagen').m-auto
    ModalA(:abrir-modal.sync="modal7")
      .row
        .col-12
          figure
            img(src='@/assets/curso/tema2/img7.jpg', style="width: 1100px" ,alt='Texto que describa la imagen').m-auto
    ModalA(:abrir-modal.sync="modal8")
      .row
        .col-12
          figure
            img(src='@/assets/curso/tema2/img8.jpg', style="width: 950px" ,alt='Texto que describa la imagen').m-auto
    Separador
    #t_2_1
    .titulo-segundo.color-acento-contenido
      h2 2.1. Documentos
    p.mb-5 Como ya se ha mencionado, MongoDB es un gestor de base de datos NoSQL, con una estructura basada en documentos. Por ello, es importante aclarar la jerarquía completa de esta estructuración de la información, la cual se muestra a través de la siguiente información:
    AcordionA.mb-5(tipo="a" clase-tarjeta="tarjeta tarjeta--verde")
      .row.align-items-center.justify-content-center(titulo="Clúster")
        .col-lg-6.mb-4.mb-lg-0
          p.mb-0 En primer lugar, se encuentra el clúster, que es una agrupación de equipos de cómputo llamados nodos, que trabajan en forma conjunta para la gestión de la información presente en la base de datos, es decir, este primer nivel corresponde primordialmente a  infraestructura tecnológica.
        .col-lg-4
          figure
            img(src='@/assets/curso/tema2/img2.png', style="width: 350px" ,alt='Texto que describa la imagen').m-auto
      .row.align-items-center.justify-content-center(titulo="Conjunto de elementos")
        .col-lg-6.mb-4.mb-lg-0
          p.mb-0 Las bases de datos se almacenan en los clústeres y representan el conjunto de elementos que sirven para la gestión de información correspondiente a una solución de software particular y toda la información asociada a estos elementos, incluyendo los mismos datos. En un clúster, pueden existir varias bases de datos, cada una de las cuales responderá a soluciones de software diferentes.
        .col-lg-4
          figure
            img(src='@/assets/curso/tema2/img3.png', style="width: 350px" ,alt='Texto que describa la imagen').m-auto
      .row.align-items-center.justify-content-center(titulo="Colecciones")
        .col-lg-6.mb-4.mb-lg-0
          p.mb-0 Dentro de las bases de datos, se registran las colecciones que agrupan a un conjunto de documentos que representan una misma unidad de información. Si se compara con una base de datos relacional, es un documento que corresponde a una tabla.
        .col-lg-4
          figure
            img(src='@/assets/curso/tema2/img4.png', style="width: 350px" ,alt='Texto que describa la imagen').m-auto
      .row.align-items-center.justify-content-center(titulo="Estructura documental")
        .col-lg-6.mb-4.mb-lg-0
          p Los documentos representan el núcleo de una estructura documental con información que corresponde a un objeto u entidad del mundo real perteneciente al contexto de la aplicación. En un documento, se estructuran, de forma dinámica, los atributos (campos) que caracterizan dichos objetos descritos estructuralmente como pares clave-valor.
          p.mb-0 Nuevamente, si se realiza una comparación con el modelo relacional, un documento equivale a una tupla o fila en una tabla.
        .col-lg-4
          figure
            img(src='@/assets/curso/tema2/img5.png', style="width: 350px" ,alt='Texto que describa la imagen').m-auto
    p.mb-5 Para un mejor entendimiento de esta jerarquía, la siguiente figura presenta gráficamente la relación de los elementos ya descritos:
    .titulo-sexto.color-acento-contenido.mb-4
      p.mb-0 #[b Figura 4]. Jerarquías de almacenamiento en MongoDB
    figure.mb-5
      img(src='@/assets/curso/tema2/img2.svg', style="width: 400px" ,alt='Texto que describa la imagen').m-auto
    p Los documentos son abstracciones de una entidad u objeto del mundo real que expresa sus características por un conjunto de pares clave-valor. La clave o nombre del campo siempre son cadenas de texto y los valores pueden ser de cualquier tipo de dato primitivo o tipos de datos complejos.
    p.mb-5 A continuación, se presentan algunos ejemplos de documentos caracterizados por diferentes tipos de datos:
    .row.justify-content-center
      .col-10.col-md-8.col-lg.m-2
        figure.mb-4
          img(src='@/assets/curso/tema2/img3.svg', style="width: 400px" ,alt='Texto que describa la imagen').m-auto
        .row
          .col-12.bg-c12
            .px-4.py-5
              p.text-center Este documento representa a una persona con los atributos de nombre, apellido, id y edad. Note que cada atributo (campo) se expresa con la estructura clave-valor, donde la clave es una cadena de texto y el valor es representado por un tipo de dato primitivo (#[i String] y #[i Int]).
      .col-10.col-md-8.col-lg.m-2
        figure.mb-4
          img(src='@/assets/curso/tema2/img4.svg', style="width: 400px" ,alt='Texto que describa la imagen').m-auto
        .row
          .col-12.bg-c13
            .px-4.py-5
              p.text-center Este documento representa los datos básicos de una persona y los tipos de carros que le gustan. Note que en este ejemplo, la clave “cars” tiene asociado un tipo de dato compuesto, una colección de Strings. Las colecciones dentro de un documento se agrupan por medio de corchetes [ , ].
      .col-10.col-md-8.col-lg.m-2
        figure.mb-4
          img(src='@/assets/curso/tema2/img5.svg', style="width: 400px" ,alt='Texto que describa la imagen').m-auto
        .row
          .col-12.bg-c14
            .px-4.py-5
              p.text-center Este documento, a diferencia de los anteriores, asocia como valor a la clave cars otro nuevo documento que está representado, a la vez, por los pares clave valor name y models que es una colección de Strings.
              p.text-center Note que, a diferencia de las colecciones, los tipos documentos se agrupan por los caracteres llaves { , }.
    Separador
    #t_2_2
    .titulo-segundo.color-acento-contenido
      h2 2.2. Comandos básicos
    .row.align-items-center.mb-5
      .col-lg-4.mb-4.mb-lg-0
        figure
          img(src='@/assets/curso/tema2/img6.png', style="width: 370px" ,alt='Texto que describa la imagen').m-auto
      .col-lg-8
        p Los comandos básicos que se pueden utilizar para la manipulación y gestión de las bases de datos en MongoDB pueden ser ejecutados una vez se establece la conexión con el servidor, ya sea desde su cliente web o desde una aplicación externa.
        p A diferencia de las bases de datos relacionales, en MongoDB no existe una separación de comandos para la creación de estructuras como en el caso de las sentencias DDL de SQL y comandos para la manipulación de las estructuras creadas como las sentencias DML en SQL. Este tipo de base de datos busca tener mayor flexibilidad y adaptabilidad, por lo que una consulta sobre una estructura inexistente puede hacer que el motor de base de datos cree dicha estructura de forma automática.
        p.mb-0 Los comandos en MongoDB se pueden escribir tanto en una sola línea como ordenados por medio de espacios, saltos de línea o indentación, para hacer más legible su estructura, lo que no afecta la interpretación del motor de base de datos de MongoDB.
    .tarjeta.color-secundario.p-4.p-md-5.mb-5
      .row.justify-content-around.align-items-center
        .col-8.col-sm-6.col-md-4.mb-4.mb-md-0
          img(src="@/assets/curso/tema2/img6.svg")
        .col-md.col-lg-6
          h3(style="color: #12263F") Llamado a la acción comandos básicos más utilizados en MongoDB
          p.mb-4(style="color: #12263F") Le invitamos a conocer los comandos básicos más utilizados junto con su descripción:
          a.boton.color-acento-botones.texto-blanco(:href="obtenerLink('/downloads/prueba.pdf')" target="_blank" type="application/pdf")
            span(style="color: #12263F !important") Descargar
            i.fas.fa-file-download(style="color: #12263F !important")

</template>

<script>
export default {
  name: 'Tema2',
  data: () => ({
    mostrarIndicador: true,
    modal1: false,
    modal2: false,
    modal3: false,
    modal4: false,
    modal5: false,
    modal6: false,
    modal7: false,
    modal8: false,
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
