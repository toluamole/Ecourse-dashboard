<template>
  <nav class="panel panel-right" style="border-radius:0">
    <div class="profile">
      <img class="profile-image" src="@/assets/img/Rectangle 100.png" alt="">
      <p class="profile-name">Alexa Rogue</p>
      <i class="profile-icon"></i>
    </div>
    <!-- End of profile  -->
    <div class="prog">
      <h3 class="prog-primary">Progress</h3>
      <div class="prog-items">
       <i class="fas fa-pen"></i>
        <div class="prog-text">
          <p class="prog-text-primary">UI/UX Design</p>
          <span class="prog-text-secondary">Advanced</span>
        </div>
        <progress class="progress is-small is-blue" value="75" max="100">60%</progress>
      </div>
       <div class="prog-items">
      <i class="fas fa-camera"></i>
        <div class="prog-text">
          <p class="prog-text-primary">Photography</p>
          <h6 class="prog-text-secondary">Intermediate</h6>
        </div>
        <progress class="progress is-small is-glo" value="50" max="100">60%</progress>
      </div>
       <div class="prog-items">
       <i class="fas fa-pen"></i>
        <div class="prog-text">
          <p class="prog-text-primary">Animation</p>
          <span class="prog-text-secondary">Advanced</span>
        </div>
        <progress class="progress is-small is-orange" value="70" max="100">60%</progress>
      </div>
    </div>
    <!-- End of progress -->
    <div class="task">
      <h3 class="task-primary">Upcoming Task</h3>
      <div class="task-items">
       <i class="far fa-comment-alt"></i>
        <div class="task-text">
          <p class="task-text-primary">UI/UX - Design</p>
          <h6 class="task-text-secondary">27th october 2020, Tuesday</h6>
        </div>
      </div>
       <div class="task-items">
      <i class="fas fa-camera"></i>
        <div class="task-text">
          <p class="task-text-primary">Animation - 3D Animation</p>
          <h6 class="task-text-secondary">27th october 2020, Tuesday</h6>
        </div>
      </div>
    </div>
    <!-- End of task -->
    <div class="footer">
      <div class="footer-image">
        <img class="footer-image-background" src="@/assets/img/download.png" alt="" srcset="">
      </div>
    </div>
 </nav>
 <!-- <p>progress</p> -->
</template>

<script>
export default {

}
</script>

<style lang="scss">
 @import '../assets/scss/index.scss';
 .panel-right{
    width: 25%;
 }
 .profile{
   margin-top: 1.5rem;
   display: flex;
  //  flex-direction: row;
   justify-content: center;
   align-items: center;
   margin-right: 4rem;
   &-image{
    //  margin-right: 2rem;
   }
   &-name{
     margin-left: .5rem;
     font-weight: 600;
     font-family: inherit;
     font-size: 1rem;
     color: black;
   }
   &-icon {
      border: solid $menu;
      border-width: 0 1.5px 1.5px 0;
      display: inline-block;
      padding: 2px;
      transform: rotate(45deg);
      -webkit-transform: rotate(45deg);
      margin-left:1rem;
    }
 }
 .prog{
    display: flex;
    flex-direction: column;
    &-primary{
      margin-right: 12rem;
      margin-top: 2rem;
      margin-bottom: 1.5rem;
      font-weight: 600;
      color: black;
    }
    &-text{
      font-family: inherit;
      &-primary{
        font-size: 14px;
        font-weight: 600;
        color: black;
      }
      &-secondary{
        font-size: 12px;
        margin-top: 2.5px;
        color:#83919E;
      }
    }
    &-items{
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 2rem;
      progress.is-small{
        width: 5.5rem;
        height: 0.4rem;
        border-radius: 12px;
      }
      progress.is-blue::-webkit-progress-value{
        background-color: rgba($color:#5E81F4 , $alpha: 1.0);
      }
      progress.is-blue::-webkit-progress-bar{
        background:  rgba(94, 129, 244, 0.2);
      }
      progress.is-glo::-webkit-progress-value{
        background-color: rgba($color:#0CC3E7 , $alpha: 1.0)
      }
      progress.is-glo::-webkit-progress-bar{
        background:  rgba(12, 195, 231, 0.18);
      }
      progress.is-orange::-webkit-progress-value{
        background-color: rgba($color:#FFAE33 , $alpha: 1.0)
      }
      progress.is-orange::-webkit-progress-bar{
        background:  rgba(255, 128, 139, 0.2);
      }
      .fa-pen{
        color: #5E81F4;
        background-color: rgba(94, 129, 244, 0.2);
        padding: 13px;
        border-radius: 5px;
        font-size: 19px;
      }
      .fa-camera{
        color: #0CC3E7;
        background-color: rgba(12, 195, 231, 0.18);
        padding: 13px;
        border-radius: 5px;
        font-size: 19px;
      }
    }
  }
  .task{
    display: flex;
    flex-direction: column;
    &-primary{
      margin-right: 9rem;
      margin-top: 2rem;
      margin-bottom: 1.5rem;
      font-weight: 600;
      color: black;
    }
    &-text{
      font-family: inherit;
      &-primary{
        font-size: 14px;
        font-weight: 600;
        color: black;
        margin-right: 1.5rem;
      }
      &-secondary{
        font-size: 12px;
        color:#83919E;
        margin-right: 2.5rem;
        margin-top: 3px;
      }
    }
    &-items{
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 2rem;
      .fa-comment-alt{
        color: #5E81F4;
        background-color: rgba(94, 129, 244, 0.2);
        padding: 13px;
        border-radius: 5px;
        font-size: 19px;
      }
      .fa-camera{
        color: #FFAE33;
        background-color: rgba(255, 128, 139, 0.2);
        padding: 13px;
        border-radius: 5px;
        font-size: 19px;
      }
    }
  }
  // .footer-image-background{
  //   position: absolute;
  //   z-index: 1;
  // }
  .footer{
    background-color: $white !important;
  }
  .footer-image{
    // position: absolute;
    // bottom: 9.4%;
    // right: 3%;
    // z-index: 9999;
    // width: 6rem;
    cursor: pointer;
  }
</style>
