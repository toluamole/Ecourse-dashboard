<template>
  <nav class="panel" style="border-radius:0">
    <div>
     <img class="panel-logo" src="@/assets/img/logo.png" alt="">
    </div>
    <div class="panel-btn">
      <button>Join a course</button>
    </div>
    <div class="panel-list">
      <ul>
        <li><i class="fas fa-columns"></i>Dashboard</li>
        <li><i class="courses fas fa-th-large"></i>All Courses</li>
        <li><i class="far fa-folder"></i>Resources</li>
        <li><i class="far fa-user"></i>Friends</li>
        <li><i class="far fa-comment-alt"></i>Chats</li>
        <li><i class="fas fa-cog"></i>Settings</li>
      </ul>
    </div>
    <div class="upgrade">
      <img class="upgrade-image" src="@/assets/img/folder.png" alt="">
      <p class="upgrade-text">upgrade for more resources </p>
      <button class="upgrade-btn">upgrade</button>
    </div>
 </nav>
</template>

<script>
export default {

}
</script>

<style lang="scss" >
 @import '../assets/scss/index.scss';
  .panel{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    width: 15%;
    margin-bottom: 0!important;
    background: white;
    box-shadow: none;
   &-logo{
     transform: translateX(-50%, -50%);
      margin-top: 2rem;
      margin-bottom: 2rem;
   }
   &-btn{
     margin-bottom: 2rem;
      button{
        width: 150px;
        height: 40px;
        border-radius: 10px;
        border: none;
        background: $btn;
        color: $white;
        cursor: pointer;
        outline: none;
      }
   }
   &-list{
     margin-bottom: 1rem;
     cursor: pointer;
     li{
       margin-bottom: 3rem;
       color: $menu;
       i{
         margin-right: 1rem;
       }
        &:hover{
        color: blue;
        }
     }
      li:nth-child(2){
      color: black;
      font-weight: bold;
      }
   }
   .upgrade{
     display: flex;
     flex-direction: column;
     justify-content: space-between;
     align-items: center;
     border: 1px solid $primary-color;
     border-radius: 5px;
     background: $primary-color;
     padding: 2px;
     margin-bottom: 5rem;
     &-image{
       width:55px;
       margin-bottom: 1rem;
     }
     &-text{
       font-size: 13px;
       margin-bottom: .5rem;
       padding-left: 3px;
       padding-right: 3px;
       width: 139px;
       text-align: center;
     }
     &-btn{
        width: 80px;
        height: 30px;
        border-radius: 5px;
        border: none;
        background: $btn;
        color: $white;
        margin-bottom: 1rem;
        cursor: pointer;
        outline: none;
     }
   }
  }
  .courses{
    color:blue;
  }
</style>
