// NexxisDetails.vue

<template>
  <div class="nexxis-details">
    <div class="feature-section">
      <h3>Always up to date</h3>
      <p>
        Built on a non-proprietary IP technology platform, Nexxis is ready for any new technology (such as 4K) as soon as you are. Scalable and flexible, Nexxis allows you to adapt as you need to and expand as you grow.
      </p>
      <ul>
        <li>Always up to date with the latest networking and visualization technologies</li>
        <li>Easy to adopt new integration requirements in the OR</li>
        <li>Easy to connect new ORs to the network architecture</li>
        <li>Expansion results in lower TCO</li>
      </ul>
    </div>
    
    <div class="certification-section">
      <div class="certification-info">
        <i class="certification-icon">✓</i>
        <p>
          Certified as a medical device (CE/FDA), Nexxis is fit for use in the interventional OR. Every part of the solution has been designed and approved for use in a surgical environment.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NexxisDetails'
}
</script>

<style scoped>
.nexxis-details {
  margin: 40px 0;
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

.certification-section {
  background-color: #f5f8fa;
  padding: 25px;
  border-radius: 8px;
  border-left: 4px solid #00b050;
}

.certification-info {
  display: flex;
  align-items: center;
  gap: 15px;
}

.certification-icon {
  font-size: 24px;
  color: #00b050;
  background-color: rgba(0, 176, 80, 0.1);
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  flex-shrink: 0;
}

.certification-info p {
  font-size: 16px;
  line-height: 1.5;
  color: #444;
  margin: 0;
}
</style>