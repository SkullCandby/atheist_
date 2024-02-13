<template>
  <header class="site-header">
    <nav>
      <ul>
        <li><a href="https://twitter.com/atheist_solana" target="_blank"> 👁Twitter</a></li>
        <li><a href="https://dexscreener.com/solana/Bo6mhso4GfDoiYW5xvVCcaLDpiJLtE7BXDy6bT8QpkRN" target="_blank">👁Chart</a></li>
        <li><a href="https://t.me/+twjxg3br6spkZWNi" target="_blank">👁 Telegram</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderSection',
}
</script>

<style scoped>
.site-header {
  background-color: #121212; /* Dark background to match atheism theme */
  padding: 1rem;
}

.site-header nav ul {
  list-style-type: none;
  display: flex;
  justify-content: space-around;
}

.site-header nav ul li a {
  color: #FFD700; /* Golden color for text */
  text-decoration: none;
  padding: 0 0.5rem;
  font-weight: bold; /* Ensure the text is bold */
}
</style>

