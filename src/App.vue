<template>
<div>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>

  <!-- 
    <Home2 />
    <Home /> 
    <TwoWayBindings />
    <GetInputValues />
  <GetCheckBoxAndRadioValues />
  <ConditionalRendaring />
  <ForLoop />
  <PassDataToChildComponent />
  -->
  <ReuseComponent />
</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
/* import Home2 from './components/Part-1-Basic.vue.vue'
  import Home from './components/Part-2-Events.vue' 
 import TwoWayBindings from './components/Part-3-TwoWayBindings.vue'
import GetInputValues from './components/Part-4-GetInputValues.vue'
import GetCheckBoxAndRadioValues from './components/Part-5-GetCheckBoxAndRadioValues.vue',
import ConditionalRendaring from './components/Part-6-ConditionalRendaring.vue'
import ForLoop from './components/Part-7-ForLoop.vue'
import PassDataToChildComponent from './components/Part-8-PassDataToChildComponent.vue'
 */
import ReuseComponent from './components/Part-9-ReuseComponent.vue'



export default {
  name: 'App',
  components: {
    HelloWorld,
  /*   Home2,
    Home, 
    TwoWayBindings,
    GetInputValues,
    GetCheckBoxAndRadioValues,
    ConditionalRendaring,
    ForLoop, 
    PassDataToChildComponent,
  */
    ReuseComponent
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
