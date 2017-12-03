<template>
  <q-layout ref="layout">
    <q-ajax-bar color="tertiary"/>
    <!-- Header -->
    <q-toolbar slot="header" class="header">
      <q-parallax class="header__background" src="statics/aut.jpg"/>
      <div class="row justify-center items-end fit">
        <div class="row justify-center items-center mb-3 header__container">
          <img src="./assets/user.svg" width="200px" class="mr-3 header__avatar">
          <div class="column justify-start">
            <strong class="header__title">Siavash Kavousi</strong>
            <div>Amirkabir University of Technology</div>
            <div><strong class="text-orange-5">Devops</strong> Engineer</div>
            <div class="row justify-start header__social mt-1">
              <a href="https://github.com/siavashkavousi">
                <fa-icon :icon="['fab', 'github']" size="3x"></fa-icon>
              </a>
              <a href="https://twitter.com/siavash_kavousi">
                <fa-icon :icon="['fab', 'twitter']" size="3x"></fa-icon>
              </a>
            </div>
          </div>
        </div>
      </div>
    </q-toolbar>

    <div class="column items-center portfolio my-5">
      <h3 class="portfolio__title">PORTFOLIO</h3>

      <div style="width: 500px;">
        <q-gallery-carousel :src="gallery" horizontal-quick-view/>
      </div>
      <!--<q-carousel arrows dots class="text-white">-->
      <!--<div slot="slide" class="bg-primary">-->
      <!--<div class="portfolio__support"></div>-->
      <!--</div>-->
      <!--<div slot="slide" class="bg-secondary">-->
      <!--Slide 2-->
      <!--</div>-->
      <!--</q-carousel>-->
    </div>

    <div class="layout-padding">
      <router-view/>
    </div>
  </q-layout>
</template>

<script>
  import {
    QLayout,
    QToolbar,
    QAjaxBar,
    QParallax,
    QCarousel,
    QGalleryCarousel
  } from 'quasar'

  export default {
    components: {
      QLayout,
      QToolbar,
      QAjaxBar,
      QParallax,
      QCarousel,
      QGalleryCarousel
    },
    data () {
      return {
        gallery: [
          'statics/projects/support.png',
          'statics/projects/portal.png',
        ],
      }
    },
  }
</script>

<style lang="stylus">
  @import './themes/app.variables.styl'

  .header
    height 400px
    position relative

  .header__background
    position absolute
    top 0
    left 0
    background-size cover
    width calc(100% + 10px)
    height calc(100% + 10px)
    z-index 1
    margin -5px
    filter blur(5px)

  .header__container
    z-index 10
    @media (min-width: $breakpoint-md)
      margin-right 200px

  .header__title
    font-size 46px
    font-weight 400

  .header__avatar
    border 3px solid white
    border-radius 50%

  .header__social
    & > a
      color white
      &:hover
        color: darken(white, 20%)
    & > *
      padding-right 10px

  .portfolio
    /*background-color #B8CEF1*/
  .portfolio__title
    font-weight bold

  .portfolio__support
    /*background url("statics/projects/support.png")*/
    width 400px
    height 300px
    background-size cover
</style>
