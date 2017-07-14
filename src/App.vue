<template>
  <q-layout ref="layout">
    <!-- Header -->
    <q-toolbar slot="header">
      <q-toolbar-title>
        Siavash Kavousi
        <span slot="subtitle">personal website</span>
      </q-toolbar-title>
    </q-toolbar>

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
