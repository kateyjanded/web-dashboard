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
              <span><img src="./assets/team.png" alt=""></span>
              <span>Team</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/task.png" alt=""></span>
              <span>Tasks</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/project.png" alt=""></span>
              <span>Projects</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/timesheet.png" alt=""></span>
              <span>Time Sheet</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/contact.png" alt=""></span>
              <span>contact</span>
            </a>
          </li>
          <li>
            <a href="">
              <span><img src="./assets/setting.png" alt=""></span>
              <span>My Account</span>
            </a>
          </li>
        </ul>
      </div>
    </div>
    <div class="main-content">
        <header>
            <img src="./assets/search.png" alt="">
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
  }
}
</script>

<style>
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
  width: 300px;
  margin: 0px;
  background: var(--main-color);
  color: #fff;
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
  padding: 1rem;
}
.side-menu li{
  padding: 0px;
  margin-bottom: 1rem;
}
.side-menu a{
  color: white;
}
.side-menu img{
  width: 20px;
  height: 20px;
  margin: 0px;
}
.sidebar a span:first-child{
  padding-right: 1rem;
}
</style>
