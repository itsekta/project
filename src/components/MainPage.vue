<template>
    <div class="container">
      <div class="left-panel">
        <!-- <h3 class="left-panel-header">Menu</h3> -->
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
          <br>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus bibendum eros nec magna aliquet sagittis. Vestibulum condimentum maximus aliquet. Suspendisse euismod metus vel metus cursus, a pulvinar neque lacinia. Quisque congue sem eu nisi sagittis faucibus. Nulla tristique metus sit amet dui condimentum pellentesque. Proin consectetur mauris elit, sit amet posuere nunc volutpat eu. Suspendisse potenti.</p>
          <br>
          <p>Nullam a est leo. Nullam facilisis ipsum sed augue lacinia, eu pharetra odio tempor. Nam bibendum tellus eu eros tristique faucibus. Proin at tortor id enim mattis rutrum. Nullam nec enim non nibh laoreet consectetur non id ligula. Morbi quis malesuada neque, vitae sagittis mi. Nunc viverra dignissim est, nec venenatis turpis aliquet ac. Etiam commodo risus at odio congue convallis. Nam facilisis auctor sapien, et ullamcorper turpis porta eu.</p>
          <br>
          <p>Curabitur in eros eget justo finibus dapibus. Donec ut consequat lectus. Phasellus ut sapien at quam bibendum bibendum eu id mi. Ut efficitur euismod lacinia. Sed volutpat scelerisque odio, non posuere ligula aliquam vitae. Nullam facilisis nisl tortor, at ullamcorper nisl luctus in. Duis vehicula urna id felis sollicitudin bibendum. Fusce et facilisis nunc, sed fringilla nunc. Suspendisse sollicitudin tristique elit, a ullamcorper tellus mollis id. In efficitur pharetra risus, in malesuada felis mollis et. Fusce consequat justo ac arcu dignissim efficitur. Vestibulum congue eros vel tortor pellentesque, id pellentesque nibh tincidunt.</p>
 
        </div>
        <div class="content-block" v-else-if="activeComponent === 'contact'">
          <h1>Contact Information</h1>
          <br>
          <p>Curabitur in eros eget justo finibus dapibus. Donec ut consequat lectus. Phasellus ut sapien at quam bibendum bibendum eu id mi. Ut efficitur euismod lacinia. Sed volutpat scelerisque odio, non posuere ligula aliquam vitae. Nullam facilisis nisl tortor, at ullamcorper nisl luctus in. Duis vehicula urna id felis sollicitudin bibendum. Fusce et facilisis nunc, sed fringilla nunc. Suspendisse sollicitudin tristique elit, a ullamcorper tellus mollis id. In efficitur pharetra risus, in malesuada felis mollis et. Fusce consequat justo ac arcu dignissim efficitur. Vestibulum congue eros vel tortor pellentesque, id pellentesque nibh tincidunt.</p>
          <br>
          <p>Nullam a est leo. Nullam facilisis ipsum sed augue lacinia, eu pharetra odio tempor. Nam bibendum tellus eu eros tristique faucibus. Proin at tortor id enim mattis rutrum. Nullam nec enim non nibh laoreet consectetur non id ligula. Morbi quis malesuada neque, vitae sagittis mi. Nunc viverra dignissim est, nec venenatis turpis aliquet ac. Etiam commodo risus at odio congue convallis. Nam facilisis auctor sapien, et ullamcorper turpis porta eu.</p>
          <br>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus bibendum eros nec magna aliquet sagittis. Vestibulum condimentum maximus aliquet. Suspendisse euismod metus vel metus cursus, a pulvinar neque lacinia. Quisque congue sem eu nisi sagittis faucibus. Nulla tristique metus sit amet dui condimentum pellentesque. Proin consectetur mauris elit, sit amet posuere nunc volutpat eu. Suspendisse potenti.</p>
 
        </div>
        <div class="content-block" v-else-if="activeComponent === 'information'">
          <h1>Information</h1>
          <br>
          <p>Nullam a est leo. Nullam facilisis ipsum sed augue lacinia, eu pharetra odio tempor. Nam bibendum tellus eu eros tristique faucibus. Proin at tortor id enim mattis rutrum. Nullam nec enim non nibh laoreet consectetur non id ligula. Morbi quis malesuada neque, vitae sagittis mi. Nunc viverra dignissim est, nec venenatis turpis aliquet ac. Etiam commodo risus at odio congue convallis. Nam facilisis auctor sapien, et ullamcorper turpis porta eu.</p>
          <br>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus bibendum eros nec magna aliquet sagittis. Vestibulum condimentum maximus aliquet. Suspendisse euismod metus vel metus cursus, a pulvinar neque lacinia. Quisque congue sem eu nisi sagittis faucibus. Nulla tristique metus sit amet dui condimentum pellentesque. Proin consectetur mauris elit, sit amet posuere nunc volutpat eu. Suspendisse potenti.</p>
          <br>
          <p>Curabitur in eros eget justo finibus dapibus. Donec ut consequat lectus. Phasellus ut sapien at quam bibendum bibendum eu id mi. Ut efficitur euismod lacinia. Sed volutpat scelerisque odio, non posuere ligula aliquam vitae. Nullam facilisis nisl tortor, at ullamcorper nisl luctus in. Duis vehicula urna id felis sollicitudin bibendum. Fusce et facilisis nunc, sed fringilla nunc. Suspendisse sollicitudin tristique elit, a ullamcorper tellus mollis id. In efficitur pharetra risus, in malesuada felis mollis et. Fusce consequat justo ac arcu dignissim efficitur. Vestibulum congue eros vel tortor pellentesque, id pellentesque nibh tincidunt.</p>
 
        </div>
        <div class="content-block" v-else-if="activeComponent === 'guide'">
          <h1>Guide</h1>
          <br>
          <p>Curabitur in eros eget justo finibus dapibus. Donec ut consequat lectus. Phasellus ut sapien at quam bibendum bibendum eu id mi. Ut efficitur euismod lacinia. Sed volutpat scelerisque odio, non posuere ligula aliquam vitae. Nullam facilisis nisl tortor, at ullamcorper nisl luctus in. Duis vehicula urna id felis sollicitudin bibendum. Fusce et facilisis nunc, sed fringilla nunc. Suspendisse sollicitudin tristique elit, a ullamcorper tellus mollis id. In efficitur pharetra risus, in malesuada felis mollis et. Fusce consequat justo ac arcu dignissim efficitur. Vestibulum congue eros vel tortor pellentesque, id pellentesque nibh tincidunt.</p>
          <br>
          <p>Nullam a est leo. Nullam facilisis ipsum sed augue lacinia, eu pharetra odio tempor. Nam bibendum tellus eu eros tristique faucibus. Proin at tortor id enim mattis rutrum. Nullam nec enim non nibh laoreet consectetur non id ligula. Morbi quis malesuada neque, vitae sagittis mi. Nunc viverra dignissim est, nec venenatis turpis aliquet ac. Etiam commodo risus at odio congue convallis. Nam facilisis auctor sapien, et ullamcorper turpis porta eu.</p>
          <br>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus bibendum eros nec magna aliquet sagittis. Vestibulum condimentum maximus aliquet. Suspendisse euismod metus vel metus cursus, a pulvinar neque lacinia. Quisque congue sem eu nisi sagittis faucibus. Nulla tristique metus sit amet dui condimentum pellentesque. Proin consectetur mauris elit, sit amet posuere nunc volutpat eu. Suspendisse potenti.</p>
 
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
    padding-top: 64px;
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
    gap: 8px;
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
    background-color: #ffffff;
    border-bottom: 3px solid #143a56;
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
  p{
        text-align: start;
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
  