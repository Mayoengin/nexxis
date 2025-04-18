<template>
  <div class="app">
    <NavBar />
    <NexxisHeader />
    <NexxisFeatures />
    <NexxisDetails />
    <Nexxis3DSection />
    <NexxisFooter />
  </div>
</template>

<script>
import NavBar from './components/common/NavBar.vue';
import NexxisHeader from './components/NexxisHeader.vue';
import NexxisFeatures from './components/NexxisFeatures.vue';
import NexxisDetails from './components/NexxisDetails.vue';
import Nexxis3DSection from './components/Nexxis3DSection.vue';
import NexxisFooter from './components/common/NexxisFooter.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    NexxisHeader,
    NexxisFeatures,
    NexxisDetails,
    Nexxis3DSection,
    NexxisFooter
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, sans-serif;
}

.app {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}
</style>