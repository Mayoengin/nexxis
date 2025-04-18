// Nexxis3DSection.vue

<template>
  <div class="nexxis-3d-section">
    <div class="section-content">
      <div class="section-text">
        <h3>3D imaging with MDSC-8232 M3D</h3>
        <p>
          The MDSC-8232 M3D is a 31-inch, 2D and 3D 4K surgical monitor that can be seamlessly integrated into Nexxis architectures. With this display integrated into your Nexxis system, 3D sources become part of the full integration, including support for inter-OR sharing, remote management, streaming and recording. 3D source images are also automatically translated into 2D or 3D for maximum visibility.
        </p>
      </div>
      <div class="section-image">
        <img src="./assets/3d-monitor.JPG" alt="MDSC-8232 M3D Surgical Monitor" />
      </div>
    </div>
    
    <div class="components-notice">
      <p>
        Scroll down for our current offering of Nexxis components. For Nexxis accessories and network switches, your Barco sales representative will be happy to help you.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Nexxis3DSection'
}
</script>

<style scoped>
.nexxis-3d-section {
  margin: 60px 0;
}

.section-content {
  display: flex;
  gap: 40px;
  align-items: center;
  margin-bottom: 30px;
}

.section-text {
  flex: 1;
}

.section-text h3 {
  color: #003366;
  font-size: 24px;
  margin-bottom: 15px;
  position: relative;
  padding-bottom: 10px;
}

.section-text h3::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 60px;
  height: 3px;
  background-color: #003366;
}

.section-text p {
  font-size: 16px;
  line-height: 1.6;
  color: #555;
}

.section-image {
  flex: 1;
}

.section-image img {
  width: 100%;
  border-radius: 8px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}

.components-notice {
  background-color: #f5f8fa;
  padding: 20px;
  border-radius: 8px;
  text-align: center;
  margin-top: 40px;
}

.components-notice p {
  font-size: 16px;
  color: #666;
  font-style: italic;
}
</style>