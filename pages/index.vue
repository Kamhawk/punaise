<template>
  <div class="main-page">
    <Header></Header>
    <About></About>
    <Project></Project>
    <Contact></Contact></div
></template>

<script>
import Header from './Header'
import About from './About'
import Project from './Project'
import Contact from './Contact'
export default {
  components: { Header, About, Project, Contact }
}
</script>
