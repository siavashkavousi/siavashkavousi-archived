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

    <div class="layout-padding column items-center portfolio mb-5">
      <h3 class="header__item__title mb-4">PORTFOLIO</h3>
      <div style="width: 500px;">
        <gallery :src="gallery" horizontal-quick-view/>
      </div>
    </div>

    <q-parallax class="layout-padding" src="statics/experience.jpg">
      <div class="row justify-center items-center experience mb-5 fit">
        <h3 class="header__item__title text-orange-5">EXPERIENCE</h3>
        <time-line :points="points"></time-line>
      </div>
    </q-parallax>

    <router-view/>
  </q-layout>
</template>

<script>
  import {
    QLayout,
    QToolbar,
    QAjaxBar,
    QParallax,
    QList,
    QItem
  } from 'quasar'
  import Gallery from '@/gallery'
  import TimeLine from '@/time-line'

  export default {
    components: {
      QLayout,
      QToolbar,
      QAjaxBar,
      QParallax,
      Gallery,
      QList,
      QItem,
      TimeLine,
    },
    data () {
      return {
        gallery: [
          {link: 'https://support.aut.ac.ir', img: 'statics/projects/support.png'},
          {link: 'http://portal2.cloud.aut.ac.ir', img: 'statics/projects/portal.png'},
        ],
        points: [
          {
            pointColor: 'red', // important! the color of every time point and you can use red yellow or green *关键点颜色 可选red yellow green
            img: 'http://www.jikexueyuan.com/event/static/images/bootstrap/bootstrap-logo.png', // img url for every time point 图片地址 可留空
            title: 'hello world', // important! title *时间点标题
            text: 'first post', // important! the content you want show *时间点内容
            linkUrl: 'https://www.google.com', // url for read more 链接url 留空则不显示按钮
            linkText: 'Read detail', // show what in read for more button 按钮显示内容 默认为Read more
            date: '2017-1-1' // time of the point 时间点
          },
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

  .header__item__title
    font-weight bold
</style>
