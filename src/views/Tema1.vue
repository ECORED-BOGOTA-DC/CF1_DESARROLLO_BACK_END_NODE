<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 1
      h1 Bases de datos NoSQL
    .row.align-items-center.mb-5
      .col-lg-4.mb-4.mb-lg-0
        figure
          img(src='@/assets/curso/tema1/img1.png', style="width: 370px" ,alt='Texto que describa la imagen').m-auto
      .col-lg-8
        p El concepto de bases de datos NoSQL está ampliamente divulgado en el entorno del desarrollo de software para identificar aquellos sistemas de bases de datos que no son gestionados bajo el estándar de SQL y/o no se pueden clasificar dentro de las bases de datos relacionales.
        p Estas bases de datos NoSQL son una forma de solucionar los problemas de diseño de bases de datos que no podían ser resueltos mediante los sistemas de bases de datos relacionales o que, en caso de ser implementados (los sistemas de bases de datos relacionales), representaban un manejo de estructuras demasiado complejas que sacrificaban el rendimiento de las aplicaciones que hacían uso de estas. En este sentido, las bases de datos NoSQL permiten resolver problemas en contextos específicos.
        p.mb-0 Entonces, analice las características de los sistemas de datos relacionales (SQL) frente a los no relacionales (NoSQL):
    .row.mb-5
      .col-12.bg-c2.p-4
        .row
          .col-lg-4.mb-4.mb-lg-0
            p #[b SQL]
            ul.lista-ul.mb-0
              li.d-flex
                i.fas.fa-check(style="color: #FFC202")
                |
                p.mb-0 Conjunto de reglas preestablecidas para la estandarización o normalización de los conceptos y relaciones existentes.
              li.d-flex
                i.fas.fa-check(style="color: #FFC202")
                |
                p.mb-0 Potencia las consultas y reportes de datos que se pueden obtener bajo el estándar de SQL.
              li.d-flex
                i.fas.fa-check(style="color: #FFC202")
                |
                p.mb-0 Información relacionada con un problema particular.
          .col-lg-4.mb-4.mb-lg-0
            figure.fig-p1
              img(src='@/assets/curso/tema1/img2.svg', style="width: 370px" ,alt='Texto que describa la imagen').m-auto
          .col-lg-4
            p #[b NoSQL]
            ul.lista-ul.mb-0
              li.d-flex
                i.fas.fa-check(style="color: #FFC202")
                |
                p.mb-0 Base de datos flexible, que ofrece estructuras de almacenamiento que no requieren ser normalizadas.
              li.d-flex
                i.fas.fa-check(style="color: #FFC202")
                |
                p.mb-0 No tiene un conjunto de reglas que preestablezcan los tipos de relaciones que definirán su comportamiento.
              li.d-flex
                i.fas.fa-check(style="color: #FFC202")
                |
                p.mb-0 Alto nivel de escalamiento y evolución superior.
    .row.align-items-center.mb-5
      .col-lg-8.mb-4.mb-lg-0
        p Es importante tener en cuenta que, con la globalización de las aplicaciones, el uso masivo del Internet y las telecomunicaciones, la forma de procesar los datos se encuentra en constante evolución, lo que requiere de esquemas menos rígidos que permitan cambios de sus estructuras de una manera natural y que sean más fáciles de manejar y escalar a grandes volúmenes de datos; en estas nuevas circunstancias, muchos de los sistemas actuales necesitan tener un alto nivel de rendimiento y una alta escalabilidad, con necesidades de despliegue inmediato, por lo que se acoplan mejor a los sistemas de almacenamiento NoSQL.
        p El concepto NoSQL agrupa dentro de sí diferentes tipos de bases de datos, cada una de ellas con características muy diferentes y particulares, lo que brinda un abanico adicional de opciones que pueden adaptarse mejor a soluciones requeridas en diferentes entornos.
        p.mb-0 Según AWS (2021), las bases de datos NoSQL más representativas son las siguientes:
      .col-lg-4
        figure
          img(src='@/assets/curso/tema1/img2.png', style="width: 370px" ,alt='Texto que describa la imagen').m-auto
    .row.align-items-center.mb-4
      .col-auto.d-none.d-md-block.pe-0(style="z-index:2")
        figure
          img(src='@/assets/curso/tema1/img3.svg', style="width: 80px" ,alt='Texto que describa la imagen')
      .col-auto.bg-c3(style="z-index:1")
        .py-3.px-4
          h3.mb-0.ms-0.ms-md-4.text-white Bases de datos clave-valor
    p.mb-5 Este tipo es una de las bases de datos NoSQL más simples que existen. Su estructura, generalmente, se representa como una tabla de dos columnas:
    .row.justify-content-center.mb-5
      .col-md-9.col-lg-5
        .tarjeta-avatar-b.mb-4.mb-lg-0
          .tarjeta-avatar-b__img
            img(src='@/assets/curso/tema1/img3.png' alt='AvatarTop')
          .tarjeta.tarjeta--azul
            .p-4
              p.mb-0 #[b Clave]
              p.mb-0 En esta columna se realiza un único registro.
      .col-md-9.col-lg-5
        .tarjeta-avatar-b
          .tarjeta-avatar-b__img
            img(src='@/assets/curso/tema1/img4.png' alt='AvatarTop')
          .tarjeta.tarjeta--azul
            .p-4
              p.mb-0 #[b Valor]
              p.mb-0 Almacena los valores, que pueden ser de tipos de datos primitivos o complejos.
    p.mb-5 A continuación, se presenta un ejemplo de la estructura de este tipo de base de datos:
    .titulo-sexto.color-acento-contenido.mb-4
      p.mb-0 #[b Figura 1]. Representación de una base de datos Clave-Valor
    figure.mb-5
      img(src='@/assets/curso/tema1/img4.svg', style="width: 800px" ,alt='Texto que describa la imagen').m-auto
    .row.justify-content-center.mb-5
      .col-lg-10
        .bloque-texto-a.color-secundario.p-4.p-md-5 
          .row.m-0.align-items-center.justify-content-between
            .col-lg-4.mb-4.mb-lg-0
              figure
                img(src='@/assets/curso/tema1/img5.svg', style="width: 360px" ,alt='Texto que describa la imagen').m-auto
            .col-lg-8
              .bloque-texto-a__texto.p-4
                p Como hemos indicado, son altamente flexibles, divisibles y permiten el escalado horizontal a niveles que otros tipos de bases de datos no pueden alcanzar. Algunos ejemplos de aplicaciones que usan este tipo de base de datos:
                ul.lista-ul.mb-0
                  li.d-flex
                    i.fas.fa-circle(style="color: #0097F1")
                    |
                    p.mb-0 Aplicaciones para juegos.
                  li.d-flex
                    i.fas.fa-circle(style="color: #0097F1")
                    |
                    p.mb-0 Aplicaciones para tecnología publicitaria.
                  li.d-flex
                    i.fas.fa-circle(style="color: #0097F1")
                    |
                    p.mb-0 Aplicaciones de IoT.
    p.mb-5 En la siguiente tabla, se muestran algunos de los sistemas gestores de bases de datos NoSQL más famosos en el mercado, que permiten el uso de la estructura de almacenamiento clave-valor:
    .titulo-sexto.color-acento-contenido.mb-4
      p.mb-0 #[b Tabla 1]. Ejemplos de gestores de bases de datos tipo clave-valor
    .row.justify-content-center.mb-5
      .col-lg-9
        .tabla-a.color-acento-contenido
          table
            thead(style="background-color: #0097F1")
              tr
                th(width="30%") Nombre y logo
                th URL sitio oficial
            tbody
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img5.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://redis.io" target="_blank") https://redis.io
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img6.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://couchdb.apache.org" target="_blank") https://couchdb.apache.org
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img7.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://www.project-voldemort.com/voldemort/" target="_blank") https://www.project-voldemort.com/voldemort/
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img8.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://aws.amazon.com/es/dynamodb/" target="_blank") https://aws.amazon.com/es/dynamodb/
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img9.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://riak.com" target="_blank") https://riak.com
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img10.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://www.oracle.com/co/database/technologies/related/berkeleydb.html" target="_blank") https://www.oracle.com/co/database/technologies/related/berkeleydb.html
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img11.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://aerospike.com" target="_blank") https://aerospike.com
    .row.align-items-center.mb-4
      .col-auto.d-none.d-md-block.pe-0(style="z-index:2")
        figure
          img(src='@/assets/curso/tema1/img3.svg', style="width: 80px" ,alt='Texto que describa la imagen')
      .col-auto.bg-c3(style="z-index:1")
        .py-3.px-4
          h3.mb-0.ms-0.ms-md-4.text-white Bases de datos documentales
    p.mb-5 El nombre documental hace referencia al tipo de estructura principal usada para representar la información, el cual se denomina documento.
    .row.justify-content-center.mb-5
      .col-lg-10
        .bloque-texto-a.color-secundario.p-4.p-md-5 
          .row.m-0.align-items-center.justify-content-between
            .col-lg-4.mb-4.mb-lg-0
              figure
                img(src='@/assets/curso/tema1/img6.svg', style="width: 360px" ,alt='Texto que describa la imagen').m-auto
            .col-lg-8
              .bloque-texto-a__texto.p-4
                p.mb-0 En este tipo de base de datos, la información no está contenida en tablas, sino que se compone de una estructura de datos semiestructurada, agrupada por colecciones de objetos o documentos de tipo JSON, XML, YAML o archivos de texto, los cuales, a su vez, pueden estar estructurados por diferentes tipos de datos primitivos o compuestos. Este es un modelo eficiente e intuitivo para los desarrolladores de software.
    p Estas bases de datos semiestructuradas facilitan la versatilidad, por lo que pueden evolucionar según las necesidades de las aplicaciones, y, entre sus ventajas, ofrece la posibilidad de gestión de información semiestructurada, que puede albergar gran cantidad de información con diversos tipos de datos; ya que no tiene un esquema formal o rígido, simplifican las tareas de inserción y actualización de datos.
    p Las aplicaciones web y móviles actuales están sometidas a gran cantidad de cambios en las estructuras de información que gestionan, por lo cual este tipo de bases de datos NoSQL se adecúan muy bien a este tipo de contextos.
    p.mb-5 A continuación, se observa un ejemplo de una posible estructura para una base de datos tipo documental.
    .titulo-sexto.color-acento-contenido.mb-4
      p.mb-0 #[b Figura 2]. Representación gráfica de bases de datos tipo documental
    .row.mb-5
      .col-12.bg-c4
        .p-4
          figure
            img(src='@/assets/curso/tema1/img7.svg', style="width: 1000px" ,alt='Texto que describa la imagen').m-auto
    p.mb-5 De acuerdo con la información ya proporcionada,
    .row.align-items-center.mb-5
      .col-lg-4.bg-c5.mb-4.mb-lg-0
        .p-4
          p.fs-4 #[b ¿dónde es posible encontrar este tipo de base de datos?]
      .col-lg-8
        .cajon.color-primario.p-4
          p.mb-0 Las aplicaciones que comúnmente utilizan estas representaciones son los catálogos, perfiles de usuario y los sistemas de administración de contenido.
    p.mb-5 En la siguiente tabla 2, se muestran algunos de los sistemas gestores de bases de datos NoSQL más famosos en el mercado, que permiten el uso de la estructura de almacenamiento documental. Recuerde que los vistos en la anterior tabla fueros los de clave-valor:
    .titulo-sexto.color-acento-contenido.mb-4
      p.mb-0 #[b Tabla 2]. Ejemplos de gestores de bases de datos tipo documental
    .row.justify-content-center.mb-5
      .col-lg-9
        .tabla-a.color-acento-contenido
          table
            thead(style="background-color: #0097F1")
              tr
                th(width="30%") Nombre y logo
                th URL sitio oficial
            tbody
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img12.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://www.mongodb.com" target="_blank") https://www.mongodb.com
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img13.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://ravendb.net" target="_blank") https://ravendb.net
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img14.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://www.marklogic.com" target="_blank") https://www.marklogic.com
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img15.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://azure.microsoft.com/es-es/services/cosmos-db/" target="_blank") https://azure.microsoft.com/es-es/services/cosmos-db/
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img16.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://orientdb.org" target="_blank") https://orientdb.org
    .row.align-items-center.mb-4
      .col-auto.d-none.d-md-block.pe-0(style="z-index:2")
        figure
          img(src='@/assets/curso/tema1/img3.svg', style="width: 80px" ,alt='Texto que describa la imagen')
      .col-auto.bg-c3(style="z-index:1")
        .py-3.px-4
          h3.mb-0.ms-0.ms-md-4.text-white Bases de datos de tipo grafo
    p Esta base de datos se caracteriza por representar la información por medio de vértices y aristas, lo que la asocia directamente con la teoría de grafos, ampliamente estudiada en la matemática y las ciencias de la computación.
    p.mb-5 Entonces,
    .row.align-items-center.mb-5
      .col-lg-4.bg-c6.mb-4.mb-lg-0
        .p-4
          p.fs-4 #[b ¿qué se entiende por nodo o vértice?]
      .col-lg-8
        .tarjeta-avatar-b.mb-4.mb-lg-0
          .tarjeta-avatar-b__img
            img(src='@/assets/curso/tema1/img17.png' alt='AvatarTop')
          .tarjeta.tarjeta--azul1
            .p-4
              p.mb-0 #[b Nodo o vértice]
              p.mb-0 En esencia, un vértice o nodo representa una entidad donde se almacena un conjunto de atributos que, normalmente, van representados con la estructura de clave – valor, y las aristas representan las relaciones que permiten representar la conexión y asociación entre los diferentes nodos.
    p.mb-5 Este tipo de base de datos carece de un esquema fijo y los nodos, a su vez, pueden tener diferentes tipos y cantidades de atributos, por lo que se dice que son multidimensionales.
    .row.justify-content-center.mb-5
      .col-lg-8
        .tarjeta-avatar-b.mb-4.mb-lg-0
          .tarjeta-avatar-b__img
            img(src='@/assets/curso/tema1/img10.svg' alt='AvatarTop')
          .tarjeta.tarjeta--azul2
            .p-4
              p.mb-0 Otra característica clave es que las relaciones pueden almacenar información adicional y no existen restricciones sobre la forma en la que se establecen dichas relaciones, es decir, pueden ser sin dirección, unidireccionales o bidireccionales. Esta característica le permite tener un altísimo rendimiento en la búsqueda de resultados y el descubrimiento de nueva información.
    p.mb-5 A continuación, un ejemplo gráfico de la representación de una base de datos de tipo grafo:
    .titulo-sexto.color-acento-contenido.mb-4
      p.mb-0 #[b Figura 3]. Representación gráfica de bases de datos tipo grafo
    figure.mb-5
      img(src='@/assets/curso/tema1/img12.svg', style="width: 1300px" ,alt='Texto que describa la imagen').m-auto
      figcaption.mt-3 Nota. Tomado de Almagro (2017).
    .row.align-items-center.mb-5
      .col-lg-4.mb-4.mb-lg-0
        figure
          img(src='@/assets/curso/tema1/img18.png', style="width: 410px" ,alt='Texto que describa la imagen').m-auto
      .col-lg-8
        p Este tipo de base de datos facilita la creación y la ejecución de aplicaciones que funcionan con conjuntos de datos altamente conectados. Los casos de uso típicos son los que incluyen redes sociales, motores de recomendaciones, detección de fraude y gráficos de conocimiento.
        p.mb-0 Ya vimos algunos de los sistemas gestores de bases de datos NoSQL más famosos en el mercado, que permiten el uso de la estructura tipo clave-valor y de almacenamiento documental; ahora, es momento de ver los de tipo grafo:
    .titulo-sexto.color-acento-contenido.mb-4
      p.mb-0 #[b Tabla 3]. Ejemplos de gestores de bases de datos tipo grafo
    .row.justify-content-center.mb-5
      .col-lg-9
        .tabla-a.color-acento-contenido
          table
            thead(style="background-color: #0097F1")
              tr
                th(width="30%") Nombre y logo
                th URL sitio oficial
            tbody
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img19.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://neo4j.com/" target="_blank") https://neo4j.com/
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img20.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://www.tigergraph.com/" target="_blank") https://www.tigergraph.com/
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img21.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://www.graphengine.io/" target="_blank") https://www.graphengine.io/
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img22.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://www.arangodb.com/" target="_blank") https://www.arangodb.com/
              tr
                td
                  figure
                    img(src='@/assets/curso/tema1/img23.png', style="width: 160px" ,alt='Texto que describa la imagen').m-auto
                td
                  a(href="https://titan.thinkaurelius.com/" target="_blank") https://titan.thinkaurelius.com/
    .row.align-items-center.mb-4
      .col-auto.d-none.d-md-block.pe-0(style="z-index:2")
        figure
          img(src='@/assets/curso/tema1/img3.svg', style="width: 80px" ,alt='Texto que describa la imagen')
      .col-auto.bg-c3(style="z-index:1")
        .py-3.px-4
          h3.mb-0.ms-0.ms-md-4.text-white Paralelo entre SQL y NoSQL
    p Las bases de datos SQL y NoSQL cumplen con la labor de gestionar información y existe gran cantidad de sistemas gestores de bases de datos en el mercado, que facilitan este proceso con altos estándares de calidad. Sencillamente, estos dos modelos utilizan estructuras de almacenamiento y estándares de acceso a la información que son transversalmente diferentes. El uso o no de un modelo SQL o NoSQL dependerá del contexto de la solución que se busca resolver y de las necesidades de infraestructura requeridas por el cliente.
    p.mb-5 A continuación, se hace un paralelo de algunas de las características más importantes que diferencian un sistema SQL de un sistema NoSQL (AWS, 2021).
    .row
      .col-12.bg-c7
        .p-4
          SlyderF(columnas="col-12")
            .tarjeta.color-acento-contenido.p-4
              p.text-center.mb-4 #[b Modelos de datos]
              .row
                .col-lg.m-2
                  .row.justify-content-center
                    .col-auto.bg-c8
                      .px-5.py-2
                        p.mb-0 #[b SQL]
                    .col-12.bg-c10
                      .p-4
                        figure.mb-4
                          img(src='@/assets/curso/tema1/img24.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
                        p Presenta un esquema rígido conformado por un conjunto de tablas y relaciones; estas tablas se descomponen en columnas y filas, en las que se utilizan índices para agilizar los procesos de recuperación de información. 
                        p.mb-0 Se siguen procesos preestablecidos de normalización que permiten imponer restricciones de integridad referencial de forma muy exitosa.
                .col-lg.m-2
                  .row.justify-content-center
                    .col-auto.bg-c9
                      .px-5.py-2
                        p.mb-0 #[b NoSQL]
                    .col-12.bg-c10
                      .p-4
                        figure.mb-4
                          img(src='@/assets/curso/tema1/img25.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
                        p p Existe gran variedad de sistemas de representación, entre los que se destacan los clave-valor, documentales y grafos, que no se ciñen a un esquema rígido, por lo cual se garantiza la integridad referencial (esta labor recae sobre los desarrolladores).
                        p.mb-0 Permiten la optimización para el rendimiento y el crecimiento a gran escala.
            .tarjeta.color-acento-contenido.p-4
              p.text-center.mb-4 #[b Propiedades ACID (Atomicidad, Coherencia, Aislamiento y Durabilidad)]
              .row
                .col-lg.m-2
                  .row.justify-content-center
                    .col-auto.bg-c8
                      .px-5.py-2
                        p.mb-0 #[b SQL]
                    .col-12.bg-c10
                      .p-4 
                        p Garantizan completamente estas cuatro propiedades:
                        ol.lista-ol--cuadro
                          li.d-flex
                            .lista-ol--cuadro__vineta
                              span 1
                            | La atomicidad de las transacciones tiene garantía de ejecución al 100% o no se ejecutan en absoluto.
                          li.d-flex
                            .lista-ol--cuadro__vineta
                              span 2
                            | La coherencia se garantiza a través de sus esquemas preestablecidos, por ello, los datos deben cumplir las reglas definidas, de lo contrario, no serán aceptados.
                          li.d-flex
                            .lista-ol--cuadro__vineta
                              span 3
                            | El aislamiento se mantiene, ya que tiene sistemas que permiten la ejecución simultánea de transacciones de forma aislada.
                          li.d-flex
                            .lista-ol--cuadro__vineta
                              span 4
                            | La durabilidad se genera con sistemas complementarios que permiten recuperarse frente a casos inesperados de errores.
                .col-lg.m-2
                  .row.justify-content-center
                    .col-auto.bg-c9
                      .px-5.py-2
                        p.mb-0 #[b NoSQL]
                    .col-12.bg-c10
                      .p-4
                        p.mb-0 Las características de atomicidad, coherencia, aislamiento y durabilidad se flexibilizan para ofrecer el escalamiento horizontal, lo cual hace que estos sistemas sean la mejor opción para casos de baja latencia y alto rendimiento.
            .tarjeta.color-acento-contenido.p-4
              p.text-center.mb-4 #[b Cargas óptimas de trabajo]
              .row
                .col-lg.m-2
                  .row.justify-content-center
                    .col-auto.bg-c8
                      .px-5.py-2
                        p.mb-0 #[b SQL]
                    .col-12.bg-c10
                      .p-4
                        figure.mb-4
                          img(src='@/assets/curso/tema1/img26.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
                        p.mb-0 Presentan un alto procesamiento de transacción online (OLTP) y de procesamiento analítico online (OLAP).
                .col-lg.m-2
                  .row.justify-content-center
                    .col-auto.bg-c9
                      .px-5.py-2
                        p.mb-0 #[b NoSQL]
                    .col-12.bg-c10
                      .p-4
                        figure.mb-4
                          img(src='@/assets/curso/tema1/img27.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
                        p.mb-0 Este tipo de datos es efectivo para sistemas de baja latencia y para el análisis de datos semiestructurados.
            .tarjeta.color-acento-contenido.p-4
              p.text-center.mb-4 #[b API]
              .row
                .col-lg.m-2
                  .row.justify-content-center
                    .col-auto.bg-c8
                      .px-5.py-2
                        p.mb-0 #[b SQL]
                    .col-12.bg-c10
                      .p-4
                        figure.mb-4
                          img(src='@/assets/curso/tema1/img28.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
                        p.mb-0 Utilizan el lenguaje de consulta SQL, que se ejecuta del lado del servidor de base de datos,  para almacenar y recuperar la información.
                .col-lg.m-2
                  .row.justify-content-center
                    .col-auto.bg-c9
                      .px-5.py-2
                        p.mb-0 #[b NoSQL]
                    .col-12.bg-c10
                      .p-4
                        figure.mb-4
                          img(src='@/assets/curso/tema1/img29.png', style="width: 450px" ,alt='Texto que describa la imagen').m-auto
                        p.mb-0 Son óptimas para ser procesadas por APIS construidas por los desarrolladores.
      
</template>

<script>
export default {
  name: 'Tema1',
  components: {},
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
