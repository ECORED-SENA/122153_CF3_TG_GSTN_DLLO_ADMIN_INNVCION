<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
        
    p.mb-5 A continuación, encontrará una síntesis de la temática estudiada en el componente formativo.

    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/template/sintesis/s-1.svg", alt="Mapa conceptual titulado “Sistemas y paquetes ofimáticos”, ubicado en el centro, del cual se desprenden múltiples ramas que relacionan temas de ofimática y tecnologías de la información. Incluye conceptos como procesadores de texto, hojas de cálculo, presentaciones, navegación web, seguridad de la información, SG-SST, sistemas de información, teoría de sistemas y redes de información. También muestra clasificaciones, características, tipos de conectividad, conectividad a internet, redes sociales, intranet/extranet, hardware, software y herramientas, conectados mediante flechas que indican relaciones entre los conceptos.")
      .col-auto
        a.anexo.mb-5(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
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
