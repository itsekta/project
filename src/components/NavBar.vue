<template>
    <div class="navbar-wrapper">
      <nav class="navbar">
        <div class="navbar-logo">
          <img src="vue-logo.png" alt="Logo" />
        </div>
        <div class="navbar-links">
          <a href="https://github.com/itsekta" target="_blank" rel="noopener noreferrer" >
            <i class="fab fa-github"></i>
          </a>
          <a href="https://www.instagram.com/_itsekta_/" target="_blank" rel="noopener noreferrer">
            <i class="fab fa-instagram"></i>
          </a>
          <a href="https://www.linkedin.com/in/ekta-chaudhary-07/" target="_blank" rel="noopener noreferrer">
            <i class="fab fa-linkedin"></i>
          </a>
        </div>
      </nav>
      
    </div>
  </template>
  
  <script>
  export default {
  }
  </script>
  
  <style scoped>
  @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css');
.navbar-wrapper{
    position: fixed;
  top: 0;
  left: 0;
  width: 100%;
}
  .navbar {
    
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: #333;
  padding: 10px;
  color: white;
  }
  
  .navbar-logo img {
    width: 40px;
    height: 40px;
  }
  .navbar-links{
    display: flex;
    gap: 8px;
    align-items: center;
  }
  .navbar-links a {
    color: white;
    text-decoration: none;
    margin-left: 10px;
    font-size: 24px;
    
    
  }
  
  .container {
    /* Add your container styles here */
  }
  </style>
  