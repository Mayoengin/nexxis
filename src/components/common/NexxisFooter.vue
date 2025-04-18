// NexxisFooter.vue

<template>
  <footer class="footer">
    <div class="footer-top">
      <div class="footer-column">
        <h4>Products</h4>
        <ul>
          <li><a href="#">Nexxis</a></li>
          <li><a href="#">Surgical Displays</a></li>
          <li><a href="#">OR-over-IP</a></li>
          <li><a href="#">Video Management</a></li>
        </ul>
      </div>
      
      <div class="footer-column">
        <h4>Solutions</h4>
        <ul>
          <li><a href="#">Integrated OR</a></li>
          <li><a href="#">Hybrid OR</a></li>
          <li><a href="#">Minimally Invasive Surgery</a></li>
          <li><a href="#">Surgical Training</a></li>
        </ul>
      </div>
      
      <div class="footer-column">
        <h4>Services</h4>
        <ul>
          <li><a href="#">Professional Services</a></li>
          <li><a href="#">Support Contracts</a></li>
          <li><a href="#">Training & Education</a></li>
          <li><a href="#">Remote Management</a></li>
        </ul>
      </div>
      
      <div class="footer-column">
        <h4>Contact</h4>
        <ul>
          <li><a href="#">Find a Distributor</a></li>
          <li><a href="#">Request a Demo</a></li>
          <li><a href="#">Get a Quote</a></li>
          <li><a href="#">Support Center</a></li>
        </ul>
      </div>
    </div>
    
    <div class="footer-bottom">
      <div class="copyright">
        © 2025 Barco NV. All rights reserved.
      </div>
      
      <div class="legal-links">
        <a href="#">Privacy Policy</a>
        <a href="#">Terms of Use</a>
        <a href="#">Cookie Policy</a>
        <a href="#">Accessibility</a>
      </div>
      
      <div class="social-links">
        <a href="#" class="social-icon">📱</a>
        <a href="#" class="social-icon">📘</a>
        <a href="#" class="social-icon">📷</a>
        <a href="#" class="social-icon">📺</a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'NexxisFooter'
}
</script>

<style scoped>
.footer {
  margin-top: 60px;
  padding: 40px 0 20px;
  background-color: #f5f8fa;
  border-top: 1px solid #eaeaea;
}

.footer-top {
  display: flex;
  flex-wrap: wrap;
  gap: 40px;
  margin-bottom: 40px;
}

.footer-column {
  flex: 1;
  min-width: 200px;
}

.footer-column h4 {
  color: #003366;
  font-size: 18px;
  margin-bottom: 15px;
}

.footer-column ul {
  list-style-type: none;
}

.footer-column li {
  margin-bottom: 8px;
}

.footer-column a {
  text-decoration: none;
  color: #555;
  font-size: 14px;
  transition: color 0.2s;
}

.footer-column a:hover {
  color: #003366;
}

.footer-bottom {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
  padding-top: 20px;
  border-top: 1px solid #eaeaea;
}

.copyright {
  font-size: 14px;
  color: #777;
}

.legal-links {
  display: flex;
  gap: 20px;
}

.legal-links a {
  font-size: 14px;
  color: #777;
  text-decoration: none;
}

.social-links {
  display: flex;
  gap: 15px;
}

.social-icon {
  width: 36px;
  height: 36px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #003366;
  color: white;
  border-radius: 50%;
  text-decoration: none;
  transition: background-color 0.2s;
}

.social-icon:hover {
  background-color: #00264d;
}

@media (max-width: 768px) {
  .footer-top {
    flex-direction: column;
    gap: 30px;
  }
  
  .footer-bottom {
    flex-direction: column;
    gap: 20px;
    text-align: center;
  }
  
  .legal-links {
    flex-wrap: wrap;
    justify-content: center;
  }
}
</style>