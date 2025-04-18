// NavBar.vue

<template>
  <nav class="navbar">
    <div class="logo">
      <img src="./assets/barco-logo.png" alt="Barco Logo" />
    </div>
    
    <div class="nav-links">
      <a href="#" class="nav-link">Products</a>
      <a href="#" class="nav-link">Solutions</a>
      <a href="#" class="nav-link">Services</a>
      <a href="#" class="nav-link">Support</a>
      <a href="#" class="nav-link">Resources</a>
      <a href="#" class="nav-link">About</a>
    </div>
    
    <div class="nav-actions">
      <div class="search">
        <input type="text" placeholder="Search..." />
        <button><i>🔍</i></button>
      </div>
      <button class="menu-toggle">☰</button>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 0;
  border-bottom: 1px solid #eaeaea;
}

.logo img {
  height: 30px;
}

.nav-links {
  display: flex;
  gap: 25px;
}

.nav-link {
  text-decoration: none;
  color: #333;
  font-weight: 500;
  transition: color 0.2s;
}

.nav-link:hover {
  color: #003366;
}

.nav-actions {
  display: flex;
  align-items: center;
  gap: 15px;
}

.search {
  display: flex;
  border: 1px solid #ddd;
  border-radius: 4px;
  overflow: hidden;
}

.search input {
  border: none;
  padding: 8px 12px;
  outline: none;
}

.search button {
  background-color: #f5f5f5;
  border: none;
  padding: 8px 12px;
  cursor: pointer;
}

.menu-toggle {
  display: none;
  background: none;
  border: none;
  font-size: 24px;
  cursor: pointer;
}

@media (max-width: 768px) {
  .nav-links {
    display: none;
  }
  
  .search {
    display: none;
  }
  
  .menu-toggle {
    display: block;
  }
}
</style>