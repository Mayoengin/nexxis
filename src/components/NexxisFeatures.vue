// NexxisFeatures.vue

<template>
  <div class="nexxis-features">
    <div class="overview">
      <p>
        Nexxis™ is Barco's AV-over-IP platform for the integrated digital operating room.
        It's the best way to share uncompressed, high-resolution video (and audio) in and between operating rooms.
        This unique technology platform has been specifically designed for integration into the digital OR.
      </p>
      <p>
        Ask your integration partner about it and find out how it enhances operational efficiency, team collaboration and surgical precision.
      </p>
    </div>
    
    <div class="feature-section">
      <h3>The precision you need</h3>
      <p>
        High resolution, uncompressed medical images are presented with pixel-perfect precision and shared more efficiently.
      </p>
      <ul>
        <li>Raw, uncompressed images – eliminating artifacts</li>
        <li>Near-zero latency for perfect hand-eye coordination</li>
        <li>4K end-to-end</li>
      </ul>
    </div>
    
    <div class="feature-section">
      <h3>The flexibility you've always wanted</h3>
      <p>
        Nexxis meets every requirement of any surgical procedure. Plug and play (new) devices, switch sources with ease, and display images where and when you need them for optimal viewing comfort and ergonomics. Without interruptions, as the entire platform can be maintained remotely.
      </p>
      <ul>
        <li>Simple to set up the OR (all you need is a single optical cable)</li>
        <li>Easy plug and play of devices</li>
        <li>Central & remote control</li>
      </ul>
    </div>
    
    <div class="feature-section">
      <h3>Easy to share and collaborate</h3>
      <p>
        Images can be streamed in, between, and outside operating rooms (e.g. auditoriums) in real time. This makes it easy to educate, consult and collaborate with your peers. Recording is also possible for documentation purposes and clinical research.
      </p>
      <ul>
        <li>Bi-directional inter-OR communication</li>
        <li>Physician interaction beyond the OR</li>
        <li>Streaming and recording</li>
        <li>Easy interactive education and training</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NexxisFeatures'
}
</script>

<style scoped>
.nexxis-features {
  margin: 60px 0;
}

.overview {
  background-color: #f5f8fa;
  padding: 30px;
  border-radius: 8px;
  margin-bottom: 40px;
}

.overview p {
  font-size: 18px;
  line-height: 1.6;
  margin-bottom: 20px;
  color: #333;
}

.overview p:last-child {
  margin-bottom: 0;
}

.feature-section {
  margin-bottom: 50px;
}

.feature-section h3 {
  color: #003366;
  font-size: 24px;
  margin-bottom: 15px;
  position: relative;
  padding-bottom: 10px;
}

.feature-section h3::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 60px;
  height: 3px;
  background-color: #003366;
}

.feature-section p {
  font-size: 16px;
  line-height: 1.6;
  margin-bottom: 15px;
  color: #555;
}

.feature-section ul {
  list-style-type: none;
}

.feature-section li {
  position: relative;
  padding-left: 25px;
  margin-bottom: 10px;
  font-size: 16px;
  color: #555;
}

.feature-section li::before {
  content: "✓";
  position: absolute;
  left: 0;
  color: #003366;
  font-weight: bold;
}
</style>