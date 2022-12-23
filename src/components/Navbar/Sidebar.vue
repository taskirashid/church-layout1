<template>
    <div class="sidebar">
      <div class="sidebar-brand">
        <h1><span class="">Revive Haven Church</span></h1>
      </div>

      <div class="sidebar-menu">
        <ul>
          <li class="router-link-blk">
            <router-link to="/overview">
              <i class="fas fa-archive"></i>
              <span>Overview</span>
            </router-link>
          </li>
          <li>
            <router-link to="/aachensMsg">
              <i class="fas fa-comment-alt"></i>     
              <span>Aachen's Messages</span>  
            </router-link>
          </li>
          <li>
            <router-link to="/parish">
              <i class="fas fa-place-of-worship"></i> 
              <span>Parish</span>  
            </router-link>
          </li>
          <li>
            <router-link to="/members">
              <i class="fas fa-users"></i>
              <span>Members</span> 
            </router-link>
          </li>
          <li>
            <router-link to="/committee">
              <i class="fas fa-users-cog"></i> 
              <span>Committee</span>  
            </router-link>
          </li>
          <li>
            <router-link to="/announcementPage">
              <i class="fas fa-bullhorn"></i>
              <span>Announcement</span>
            </router-link>
          </li>
          <li>
            <router-link to="/obituary">
              <i class="fas fa-book-dead"></i>
              <span>Obituary</span>  
            </router-link>
          </li>
          <li>
            <router-link to="/events">
              <i class="fas fa-list-alt"></i>
              <span>Events</span>  
            </router-link>
          </li>
          <li>
            <router-link to="/flashNews">
              <i class="fas fa-newspaper"></i>   
              <span>Flash News</span>  
            </router-link>
          </li>
          <li>
            <router-link to="/worshipTime">
              <i class="fas fa-clock"></i> 
              <span>Worship Time</span>  
            </router-link>
          </li>
          <li>
            <router-link to="/settings">
              <i class="fas fa-cogs"></i>
              <span>Settings</span>  
            </router-link>
          </li>
        </ul>
      </div>

    </div>
</template>


<script>

export default {
  name: 'Sidebar-',
  data(){
    }
}

</script>

<style>


.sidebar{
  width: 280px;
  position: fixed;
  left: 0;
  top: 0;
  height: 100%;
  background: var(--main-color);
  box-shadow: 2px 0px 0px rgb(0 0 0 / 9%);
  z-index: 101;
}

.sidebar-brand {
  /* height: 90px; */
  padding: 0.9rem 0rem 0.9rem 2rem;
  color: var(--font-white);
}

.sidebar-brand h1{
  margin-top: 10px;
}

.sidebar-brand span {
  display: inline-block;
  color: var(--font-white);
  font-size: 2rem;
  font-weight: 600;
  font-variant-caps: small-caps;

}

.sidebar-menu li{
  width: 100%;
  /* margin-bottom: 1.3rem; */
  /* margin-left: 2rem; */
}

.sidebar-menu span {
    margin-left: 13px;
}

.sidebar-menu a{
  display: block;
  color: #363635;
  font-size: 1.4rem;
  font-weight: 400;
  padding-left: 4rem;
  padding-top: 1rem;
  padding-bottom: 1rem;
}

.sidebar-menu ul{
  padding-left: 0px;
}

.sidebar-menu a{
    text-decoration: none;
}

.sidebar-menu a:hover{
    text-decoration: none;
}

/* .sidebar-menu a.active{ */
.sidebar-menu a.router-link-exact-active{
  background: #ebeced;
  color: #34363a;
  text-decoration: none;
  box-shadow: 0px 0px 2px 0px #ffffff;
  padding-left: 5rem;
  transition: .5s cubic-bezier(0.22, 0.61, 0.36, 1);
}

.sidebar-menu a span:first-child{
  font-size: 1.5rem;
  padding-right: 1rem;
}

</style>