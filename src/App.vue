<template>
  <q-layout ref="layout" view="hHr LpR lFf" :right-breakpoint="1100">
    <!-- Header -->
    <q-toolbar slot="header">
      <q-btn flat @click="$refs.layout.toggleLeft()">
        <q-icon name="menu"/>
      </q-btn>
      <q-toolbar-title>
        Siavash Kavousi
        <span slot="subtitle">personal website</span>
      </q-toolbar-title>
    </q-toolbar>

    <div slot="left">
      <q-list no-border link inset-separator>
        <q-list-header>Essential Links</q-list-header>
        <q-side-link item to="/cv">
          <q-item-side icon="school"/>
          <q-item-main label="Docs" sublabel="cv"/>
        </q-side-link>
        <q-side-link item to="/twitter">
          <q-item-side icon="rss feed"/>
          <q-item-main label="Twitter" sublabel="@siavash_kavousi"/>
        </q-side-link>
      </q-list>
    </div>
    <router-view/>
    <!-- Footer -->
    <q-toolbar slot="footer">
      <q-toolbar-title>
        Layout Footer
      </q-toolbar-title>
    </q-toolbar>
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
    QSideLink,
    QListHeader,
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
      QSideLink,
      QListHeader
    }
  }
</script>

<style></style>
