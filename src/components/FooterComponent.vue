<template>
  <footer class="footer">
    <a href="https://t.me/your_telegram" target="_blank">Telegram</a>
    <a href="https://your_chart_link" target="_blank">Chart</a>
    <a href="https://twitter.com/your_twitter" target="_blank">Twitter</a>
  </footer>
</template>

<script>
export default {
  name: 'FooterComponent',
}
</script>

<style scoped>
.footer {
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  background-color: #121212; /* Dark background to match the theme */
  text-align: center;
  padding: 1rem 0;
}

.footer a {
  margin: 0 15px;
  color: #FF0000; /* Red color for links to stand out on the dark background */
  text-decoration: none;
}
</style>

