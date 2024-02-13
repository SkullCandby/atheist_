<template>
  <div class="header-title">
    <img :src="imageTitle" alt="Atheism Symbol" class="header-image">
    <h2 style="font-size: 2em; font-weight: bold; color: #FFD700;">Atheism on Solana</h2>
    <p style="font-weight: bold; font-size: 1.5em; color: #FFD700;">Fuck gods.</p>
  </div>
</template>

<script>
export default {
  name: 'HeaderTitleSection',
  computed: {
    imageTitle() {
      // Assuming you have an atheism symbol or related image
      return require('@/assets/ateo.jpg');
    }
  }
}
</script>

<style scoped>
@keyframes rotate360 {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}

.header-title {
  background-color: #121212; /* Dark background for atheism theme */
  color: #FFD700; /* Changing to golden color for consistency with your previous request */
  text-align: center;
  padding: 1rem 0;
}

.header-image {
  max-width: 150px; /* Adjust as necessary */
  margin: 20px;
  border-radius: 50%; /* Optional: for rounded images */
  animation: rotate360 10s linear infinite; /* Apply the rotation animation */
}

/* Adjusting the text styling for better visibility on dark background */
h2, p {
  font-weight: bold;
  color: #FFD700; /* Golden color for text to match atheism theme */
}

h2 {
  font-size: 2em; /* Adjust as needed */
}

p {
  font-size: 1.5em; /* Adjust as needed */
  margin: 0.5rem 0;
}
</style>


