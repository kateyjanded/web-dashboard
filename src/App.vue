<template>
  <div id="app">
    <div class="sidebar">
      <div class="sidebar-header">
        <h3 class="brand">
          <span><img style="width:40px; height:40px" src="./assets/brand logo.png" alt=""></span>
        </h3>
        <span>My Web Dashboard</span>
        <span><img src="./assets/menue.png" alt=""></span>
      </div>
      <div class="side-menu">
        <ul>
          <li>
            <a href="">
              <span><img src="./assets/home.png" alt=""></span>
              <span>Home</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/notification.png" alt=""></span>
              <span>Notifications</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/cart.png" alt=""></span>
              <span>Shopping Cart</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/teams.png" alt=""></span>
              <span>Team</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/tasks.png" alt=""></span>
              <span>Tasks</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/project_w.png" alt=""></span>
              <span>Projects</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/timesheet_w.png" alt=""></span>
              <span>Time Sheet</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/contact_w.png" alt=""></span>
              <span>Contact</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/setting_w.png" alt=""></span>
              <span>My Account</span>
            </a>
          </li>
        </ul>
      </div>
    </div>
    <div class="main-content">
      <header>
        <img src="./assets/search.png" class="searchImage" alt="">
        <input type="search" placeholder="Search">
        <div class="social-icons">
          <img src="./assets/notification.png" alt="">
          <div></div>
        </div>
      </header>
      <main>
        <h2>Overview</h2>
        <div class="dashboard-cards">
          <div class="card-single">
            <div class="card-body">
              <img src="./assets/briefcase.png" alt="">
              <div>
                <h5>Account Balance</h5>
                <h4>$30,560</h4>
              </div>
            </div>
            <div class="card-footer">
              <a href="#">View all</a>
            </div>
          </div>
          <div class="card-single">
            <div class="card-body">
              <img src="./assets/reload.png" alt="">
              <div>
                <h5>Pending</h5>
                <h4>$19,680</h4>
              </div>
            </div>
            <div class="card-footer">
              <a href="#">View all</a>
            </div>
          </div>
          <div class="card-single">
            <div class="card-body">
              <img src="./assets/checkbox.png" alt="">
              <div>
                <h5>Processed</h5>
                <h4>$29,430</h4>
              </div>
            </div>
            <div class="card-footer">
              <a href="#">View all</a>
            </div>
          </div>
        </div>
      </main>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  },
  data(){
    return{
      loading: true
    }
  }
}
</script>

<style>
.skeleton-loader{
  float: right;
  height: 300px;
  width: 220px ;
  background: linear-gradient(
    to right,
    rgba(255, 255, 255, 0),
    rgba(255, 255, 255, 0.5) 50%,
    rgba(255, 255, 255, 0)80%
  ), lightgray;
  background-size: 50px 200px;
  background-repeat: repeat-y;
  background-position: 0 0;
  animation: wave 1s infinite;
}
@keyframes wave{
  to {
    background-position: 100% 0;
  }
}
:root{
  --main-color: #027581;
  --color-dark: #1D2231;
  --text-grey: #8390A2;
}
#app {
  font-family: 'poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
* {
  text-decoration: none;
  padding: 0px;
  margin: 0px;
  list-style-type: none;
  box-sizing: border-box;
}
.sidebar{
  position: fixed;
  z-index: 100;
  left: 0;
  top: 0;
  height: 100%;
  width: 250px;
  margin: 0px;
  background: var(--main-color);
  color: #fff;
  overflow-y: auto;
}
.write{
  z-index: 3;
  height: 500px;
  background: red;
}
.sidebar-header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 60px;
  text-align: center;
  vertical-align: center;
  padding: 0rem 1rem;
}
.side-menu{
  padding: 0;
}
.side-menu li{
  padding: 0px;
  margin-bottom: 1rem;
}
.side-menu a{
  color: white;
  font-size: .9rem;
  text-decoration: none;
}
.side-menu img{
  width: 20px;
  height: 20px;
  margin: 0px;
}
.sidebar a span:first-child{
  padding-right: 1rem;
}
.sidebar ul{
  padding-left: 1rem;
}
.sidebar li{
  margin-bottom: 1.2rem;
}
.main-content{
  position: relative;
  margin-left: 250px;
}
.searchImage{
  width: 25px;
  height: 25px;
}
header{
  position: fixed;
  top: 0;
  left: 250px;
  z-index: 100;
  width: calc(100% - 240px);
  background: #fff;
  height: 60px;
  display: flex;
  padding: 0rem 1rem;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid #ccc;
}
main{
  margin-top: 60px;
  min-height: 90vh;
  background: #f1f5f9;
  padding: 1rem;
}
</style>
