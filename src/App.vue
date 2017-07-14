<template>
  <q-layout ref="layout">
    <!-- Header -->
    <q-toolbar slot="header">
      <q-toolbar-title>
        Siavash Kavousi
        <span slot="subtitle">personal website</span>
      </q-toolbar-title>
    </q-toolbar>

    <!--<div slot="left">-->
    <!--<q-list no-border link inset-delimiter>-->
    <!--<q-list-header>Essential Links</q-list-header>-->
    <!--<q-item @click="launch('/cv/')">-->
    <!--<q-item-side icon="school"/>-->
    <!--<q-item-main label="CV"/>-->
    <!--</q-item>-->
    <!--<q-item @click="launch('https://twitter.com/siavash_kavousi')">-->
    <!--<q-item-side icon="chat"/>-->
    <!--<q-item-main label="Twitter" sublabel="@siavash_kavousi"/>-->
    <!--</q-item>-->
    <!--</q-list>-->
    <!--</div>-->

    <div class="layout-padding">
      <router-view/>
    </div>
  </q-layout>
</template>

<script>
  import {
    QLayout,
    QToolbar,
    QToolbarTitle,
    QBtn,
    QIcon,
    QItemSide,
    QItemMain,
    QListHeader,
    QList,
    QItem,
    openURL
  } from 'quasar'

  export default {
    components: {
      QLayout,
      QToolbar,
      QToolbarTitle,
      QBtn,
      QIcon,
      QItemSide,
      QItemMain,
      QListHeader,
      QList,
      QItem
    },

    methods: {
      launch (url) {
        openURL(url)
      }
    }
  }
</script>

<style></style>
