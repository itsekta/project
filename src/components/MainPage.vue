<template>
    <div class="container">
      <div class="left-panel">
        <h3 class="left-panel-header">Menu</h3>
        <ul>
          <li @click="showContent('home')" :class="{ active: activeComponent === 'home' }">Home</li>
          <li @click="showContent('contact')" :class="{ active: activeComponent === 'contact' }">Contact</li>
          <li @click="showContent('information')" :class="{ active: activeComponent === 'information' }">Information</li>
          <li @click="showContent('guide')" :class="{ active: activeComponent === 'guide' }">Guide</li>
        </ul>
      </div>
      <div class="content-panel">
        <div class="content-block" v-if="activeComponent === 'home'">
          <h1>Welcome to the Home Page</h1>
          <p>This is the content for the Home page.</p>
        </div>
        <div class="content-block" v-else-if="activeComponent === 'contact'">
          <h1>Contact Information</h1>
          <p>This is the contact information page.</p>
        </div>
        <div class="content-block" v-else-if="activeComponent === 'information'">
          <h1>Information</h1>
          <p>This is the information page.</p>
        </div>
        <div class="content-block" v-else-if="activeComponent === 'guide'">
          <h1>Guide</h1>
          <p>This is the guide page.</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        activeComponent: 'home'
      }
    },
    methods: {
      showContent(component) {
        this.activeComponent = component;
      }
    }
  }
  </script>
  
  <style scoped>
  .container {
    display: flex;
    height: 100vh;
  }
  
  .left-panel {
    background-color: #efefef;
    padding: 20px;
    display: flex;
    flex-direction: column;
    gap: 16px;
    min-width: 200px;
  }
  .left-panel-header{
        border-bottom: 2px solid #143a56;
    padding: 8px 12px;
    background-color: #ffffff;
    border-radius: 4px;
  }
  
  ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
    display: flex;
    flex-direction: column;
    gap: 4px;
  }
  
  li {
    padding: 10px;
    cursor: pointer;
    transition: background-color 0.3s;
    border-radius: 4px;
  }
  
  li:hover {
    background-color: #e0e0e0;
  }
  
  li.active {
    background-color: #c5c5c5;
    border-left: 3px solid #143a56;
  }
  
  .content-panel {
    flex: 1;
    padding: 64px 32px;
  }
  .content-block{
    padding: 20px;
    background-color: #ffffff;
    border-radius: 4px;
  }
  @media (max-width: 560px){
    .container{
        flex-direction: column;
    }
    .left-panel{
        display: flex;
        justify-content: center;
    }
    ul{
       flex-direction: row;
    }
  }
  </style>
  