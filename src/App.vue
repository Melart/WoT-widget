<template>
  <div id="app">
    
    <Section msg="Выбор элементов"/>
    <Element msg="Элемент 1"/>
    <Element msg="Элемент 2"/>
    <div>
      <OpenPopup msg="Выбор элементов" id="show-modal" />
      <Popup ></Popup>
    </div>
  </div>
</template>

<script>
import Section from './components/Section.vue';
import Element from './components/Element.vue';
import OpenPopup from './components/OpenPopup.vue';
import Popup from './components/Popup.vue';


export default {
  name: 'app',
  components: {
    Section,
    Element,
    OpenPopup,
    Popup
  }
}
</script>

<style>
body {
  background-color: #e4e4e4;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
  width: 500px;
  margin: 0 auto;
  background-color: #fff;
  border: 2px solid rgba(0, 0, 0, 0.2);
  padding: 30px;
}
</style>
