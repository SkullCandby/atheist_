<template>
  <section class="token-section">
    <h2 style="font-size: 2em;">Atheist Coin info</h2>
    <div class="content-wrapper">
      <div class="text-content">
        <p>
  Atheism is not a philosophy; it is not even a view of the world; it is simply a refusal to deny the obvious. Unfortunately, we live in a world in which the obvious is overlooked as a matter of principle. This perspective emphasizes a reliance on empirical evidence and rational thought, choosing observation over belief without evidence.
</p>
<p>
  Historically, humanity has worshipped thousands of gods. But your god is the right one.
</p>

  


      </div>
      <img :src="imagePath" alt="Forever Alone Meme Image" class="token-image">
    </div>
  </section>
</template>

<script>
export default {
  name: 'TokenSection',
  computed: {
    imagePath() {
      // Ensure the file name matches the asset in your project's src/assets directory
      return require('@/assets/zeus.jpeg');
    }
  }
}
</script>

<style scoped>
.token-section {
  background-color: #121212; /* Dark background for atheism theme */
  color: #FFD700; /* Golden text color for contrast */
  padding: 2rem;
  text-align: center;
  overflow-x: hidden; /* Keep this to prevent any potential horizontal scrollbar */
}

.token-section h2 {
  font-size: 2em; /* Maintaining the size */
  color: #FFD700; /* Ensuring the title is also in golden color */
  /* Removing the animation for a static appearance */
}

.content-wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: left; /* Maintain left align for the text content for readability */
}

.text-content {
  font-size: 1.5em; /* Adjusting for better readability */
  color: #FFD700; /* Golden text color for consistency */
  margin: 1rem 0;
  max-width: 50%; /* Keeping the width adjustment */
}

.token-image {
  max-width: 30%; /* Adjusting image size for better layout */
  margin: 1rem; /* Uniform margin for spacing */
}

@media (max-width: 768px) {
  .content-wrapper {
    flex-direction: column;
  }

  .token-image,
  .text-content {
    max-width: 100%;
    margin-left: 0; /* Ensuring mobile responsiveness */
    text-align: center; /* Center align text when in column layout for better presentation */
  }
}
</style>



