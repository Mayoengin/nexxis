// NexxisHeader.vue

<template>
  <div class="nexxis-header">
    <div class="slideshow-container">
      <transition-group name="slide" tag="div">
        <div v-if="currentMedia === 0" key="image" class="slide">
          <img src="./assets/3d-monitor.JPG" alt="Nexxis Operating Room Solution" />
        </div>
        <div v-for="(video, index) in videos" v-if="currentMedia === index + 1" :key="`video-${index}`" class="slide">
          <video controls>
            <source :src="video.src" :type="video.type">
            Your browser does not support the video tag.
          </video>
        </div>
      </transition-group>
      <div class="slideshow-controls">
        <button 
          v-for="index in totalMedia" 
          :key="index" 
          :class="{ active: currentMedia === index - 1 }"
          @click="currentMedia = index - 1"
        ></button>
      </div>
    </div>
    
    <div class="product-info">
      <div class="product-header">
        <h1>Nexxis</h1>
        <div class="action-buttons">
          <button class="subscribe-btn">
            Subscribe to this product
          </button>
          <button class="notification-btn">
            <i class="bell-icon">🔔</i>
          </button>
        </div>
      </div>
      
      <h2>Uncompressed AV-over-IP platform</h2>
      
      <ul class="features-list">
        <li>Share video/audio in and outside the OR</li>
        <li>With near-zero latency & no compression</li>
        <li>Flexible to meet the needs of any procedure</li>
        <li>4K ready</li>
      </ul>
      
      <div class="cta-buttons">
        <button class="quote-btn">Get your quote</button>
        <button class="buy-btn">Where to buy</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NexxisHeader',
  data() {
    return {
      currentMedia: 0,
      videos: [
        { src: '@/assets/test.mp4', type: 'video/mp4' },
        { src: '@/assets/test.mp4', type: 'video/mp4' },
        { src: '@/assets/test.mp4', type: 'video/mp4' }
      ]
    }
  },
  computed: {
    totalMedia() {
      return this.videos.length + 1; // 1 image + 3 videos
    }
  },
  mounted() {
    // Optional: Auto-rotate slideshow
    setInterval(() => {
      this.currentMedia = (this.currentMedia + 1) % this.totalMedia;
    }, 5000);
  }
}
</script>

<style scoped>
.nexxis-header {
  display: flex;
  gap: 40px;
  margin: 40px 0;
}

.slideshow-container {
  flex: 1;
  position: relative;
  height: 400px;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.slide {
  position: absolute;
  width: 100%;
  height: 100%;
}

.slide img, .slide video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.slideshow-controls {
  position: absolute;
  bottom: 20px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  gap: 10px;
}

.slideshow-controls button {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  border: none;
  background-color: rgba(255, 255, 255, 0.5);
  cursor: pointer;
}

.slideshow-controls button.active {
  background-color: white;
}

.product-info {
  flex: 1;
  display: flex;
  flex-direction: column;
}

.product-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}

.product-header h1 {
  font-size: 36px;
  color: #003366;
}

.action-buttons {
  display: flex;
  gap: 10px;
}

.subscribe-btn {
  background-color: #003366;
  color: white;
  border: none;
  padding: 8px 16px;
  border-radius: 4px;
  cursor: pointer;
}

.notification-btn {
  background: none;
  border: 1px solid #003366;
  border-radius: 4px;
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

h2 {
  font-size: 24px;
  color: #333;
  margin-bottom: 20px;
}

.features-list {
  list-style-type: none;
  margin-bottom: 30px;
}

.features-list li {
  position: relative;
  padding-left: 30px;
  margin-bottom: 12px;
  font-size: 18px;
}

.features-list li::before {
  content: "•";
  position: absolute;
  left: 10px;
  color: #003366;
  font-weight: bold;
}

.cta-buttons {
  display: flex;
  gap: 15px;
  margin-top: auto;
}

.quote-btn, .buy-btn {
  padding: 12px 24px;
  border-radius: 4px;
  font-size: 16px;
  font-weight: bold;
  cursor: pointer;
  transition: all 0.2s;
}

.quote-btn {
  background-color: #003366;
  color: white;
  border: none;
}

.buy-btn {
  background-color: white;
  color: #003366;
  border: 1px solid #003366;
}

.quote-btn:hover, .buy-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

/* Transition effects */
.slide-enter-active, .slide-leave-active {
  transition: opacity 0.5s;
}

.slide-enter-from, .slide-leave-to {
  opacity: 0;
}
</style>