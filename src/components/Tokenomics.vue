<template>
  <section class="tokenomics-section">
    <h2 style="font-weight: bold;">Tokenomics</h2>
    <div class="content-flex">
      <ul>
        <li>0% tax</li>
        <li>100% LP burnt</li>
        <li>Ownership is renounced.</li>
        <li>CA:Bo6mhso4GfDoiYW5xvVCcaLDpiJLtE7BXDy6bT8QpkRN </li>
      </ul>
      <!-- Adjust the path to your image or gif -->
    </div>
  </section>
</template>

<script>
export default {
  name: 'TokenomicsSection',
  computed: {
    imagePath2() {
      // Ensure the file name matches the asset in your project's src/assets directory
      return require('@/assets/meme.jpg');
    }
  }
}
</script>

<style scoped>
.tokenomics-section {
  background-color: #121212; /* Dark background for atheism theme */
  color: #FFD700; /* Golden text color for contrast */
  padding: 2rem;
  text-align: center;
}

.content-flex {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 2rem; /* Space between the list and the image */
}

.tokenomics-section ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
  font-weight: bold;
  font-size: 2em; /* Adjusted font size for readability */
  color: #FFD700; /* Golden text color */
}

.tokenomics-image {
  max-width: 30%; /* Adjusted max width for better layout */
  margin: 1rem; /* Uniform margin for spacing */
}

/* Adjust if needed to target specific image alignments or sizes */
</style>
