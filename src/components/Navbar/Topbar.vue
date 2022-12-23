<template>
    <header>

        <h1>
          <label for="">
            <!-- <span class=""></span> -->
            Dashboard
          </label>
        </h1>
<!-- 
        <div class="search-wrapper">
          <span class="las la-search"></span>
          <input type="search" placeholder="Search here">
        </div> -->

        <div class="user-wrapper">
          <span class="las"><img src="@/assets/user.png" alt=""></span>
          <div>
            <h4>John Doe</h4>
            <small>admin</small>
          </div>
        </div>

      </header>
</template>

<script>


export default {
  name: 'Topbar-',
  data(){
    }
}

</script>

<style>

.main-content label{
  font-size: 2.5rem;
  font-weight: 600;
}

header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0.7rem;
  /* box-shadow: 2px 2px 5px rgba(0,0,0,0.2); */
    box-shadow: 0px 2px 0px rgb(0 0 0 / 9%);
  background: #fff;
  position: fixed;
  left: 280px;
  width: calc(100% - 280px);
  top: 0;
  z-index: 100;
}

header h2{
  color: #222;
}

header h1{
  margin-top: 10px;
  margin-left: 1.7rem;
}

header label span{
  font-size: 1.7rem;
  padding-right: 1rem;
}

.search-wrapper {
  border: 1px solid #ccc;
  border-radius: 30px;
  height: 40px;
  display: flex;
  align-items: center;
  /* width: 260px; */
  overflow-x: hidden;
}

.search-wrapper span{
  display: inline-block;
  padding: .5rem;
  font-size: 1.5rem;
  padding-left: 1.2rem;
}

.search-wrapper input{
  height: 100%;
  padding: .5rem;
  border: none;
  outline: none;
}

.user-wrapper{
  display: flex;
  align-items: center;
}

.user-wrapper div h4{
  margin-bottom: 0;
}

.user-wrapper img{
  border-radius: 50%;
  margin-right: 1rem;
  width: 50px;
}

.user-wrapper small{
  display: inline-block;
  color: var(--text-grey);
  margin-top: -10px !important;
}


@media (max-width: 650px) {
  
  .user-wrapper div h4{
    font-size: 14px;
  }
  header h1{
    margin-top: 4px;
  }

}


</style>