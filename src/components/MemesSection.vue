<template>
    <section class="memes-section">
      <h2 class="section-title">Favorite Memes</h2>
      <div class="memes-container">
        <img v-for="(meme, index) in memes" :key="index" :src="meme" alt="Meme Image" class="meme-img">
      </div>
      <a href="https://t.me/+twjxg3br6spkZWNi" target="_blank" class="join-button">Join the Movement</a>
    </section>
  </template>
  
  <script>
  export default {
    name: 'MemesSection',
    data() {
      return {
        // Using require to dynamically load images
        memes: [
          require('@/assets/meme.webp'),
          require('@/assets/meme.jpg'),
          require('@/assets/mem3.jpg'),
        ]
      };
    }
  }
  </script>
  
  
  <style scoped>
.memes-section {
  text-align: center;
  padding: 2rem;
  background-color: #121212;
  color: #FFFFFF;
}

.section-title {
  color: #FFD700;
  margin-bottom: 1.5rem;
}

.memes-container {
  display: flex;
  justify-content: center;
  align-items: center;
  /* Prevent wrapping to ensure images stay in one row */
  flex-wrap: nowrap;
  overflow-x: auto; /* Allows horizontal scrolling if images exceed screen width */
}

.meme-img {
  /* Adjust width to ensure images fit in a row on wider screens */
  width: 30%; /* Example width, adjust based on your needs and number of images */
  height: auto;
  margin: 10px;
  border-radius: 8px;
  flex-shrink: 0; /* Prevents the images from shrinking if container width is smaller than the combined image widths */
}

.join-button {
  display: inline-block;
  background-color: #FFD700; /* Golden background */
  color: #121212; /* Dark text for contrast */
  padding: 15px 30px; /* Larger padding for a bigger button */
  border-radius: 5px; /* Rounded corners */
  text-decoration: none; /* Removes underline from link */
  font-weight: bold; /* Makes text bold */
  font-size: 1.2em; /* Larger font size */
  margin-top: 20px; /* Spacing from the images above */
  transition: background-color 0.3s, color 0.3s; /* Smooth transition for hover effect */
}

.join-button:hover {
  background-color: #121212; /* Dark background on hover */
  color: #FFD700; /* Golden text on hover */
}
</style>
