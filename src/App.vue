<template>
  <div id="app">
    <HeaderSection/>
    <HeaderTitle />
    <TokenSection />
    <TokenomicsSection />
    <MemesSection />
    </div>
</template>

<script>
import HeaderTitle from './components/HeaderTitle.vue';
import TokenSection from './components/TokenSection.vue';
import TokenomicsSection from './components/Tokenomics.vue';
import HeaderSection from './components/HeaderSection.vue';
import MemesSection from './components/MemesSection.vue';

export default {
  name: 'App',
  components: {
    HeaderSection,
    HeaderTitle,
    TokenSection,
    TokenomicsSection,
    MemesSection,
  }
}
</script>

<style>
</style>
