<template>
  <div class="course">
    <section class="course_header">
      <input type="text" name="search" class="course_header-search " placeholder="search">
      <img src="@/assets/img/notification.png" alt="" class="course_header-image">
    </section>
    <section class="course_nav">
      <h2 class="course_nav-text" > All courses</h2>
      <ul class="course_nav-list">
        <li class="first">Ongoing</li>
        <li>Favorite</li>
        <li>Completed</li>
      </ul>
    </section>
    <section class="course_items">
      <div class="course_items-ui">
        <div class="course_items-ui--top">
          <div class="course_items-ui--top-items">
            <h3 class="course_items-ui--top-items-title">UI/UX Design</h3>
            <p class="course_items-ui--top-items-lessons">20 lessons</p>
          </div>
          <p class="course_items-ui--top-duration">2h 20min</p>
        </div>
        <div class=" course_items-ui--bottom">
         <img src="@/assets/img/Play.png" alt="Play button" class="">
         <img src="@/assets/img/Mask Group.png" alt="profile picture of a man" class="">
        </div>
      </div>
      <img class="course_items-image" src="@/assets/img/image 20.png" alt="">
      <section class="course_items-second">
        <div class="course_items-second--1">
          <div class="course_items-second--1-top">
            <div class="course_items-second--1-top-items">
              <h3 class="course_items-second--1-top-items-title">Photography</h3>
              <p class="course_items-second--1-top-items-lessons">12 lessons</p>
            </div>
           <p class="course_items-second--1-top-duration">1h 30min</p>
          </div>
          <div class=" course_items-second--1-bottom">
            <img src="@/assets/img/Play.png" alt="Play button" class="">
            <img src="@/assets/img/Group 110.png" alt="profile picture of a man" class="">
          </div>
          <img src="@/assets/img/image 23.png" alt="">
        </div>
        <div class="course_items-second--2">
          <div class="course_items-second--1-top">
            <div class="course_items-second--1-top-items">
              <h3 class="course_items-second--1-top-items-title">Animation</h3>
              <p class="course_items-second--1-top-items-lessons">12 lessons</p>
            </div>
           <p class="course_items-second--1-top-duration">2h 30min</p>
          </div>
          <div class=" course_items-second--1-bottom">
            <img src="@/assets/img/Play.png" alt="Play button" class="">
            <img src="@/assets/img/Group 112.png" alt="profile picture of a man" class="">
          </div>
          <img src="@/assets/img/image 24.png" alt="">
        </div>
      </section>
    </section>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/scss/index.scss';
 .course{
   width: 70%;
   height: 100%;
   display: flex;
   flex-direction: column;

   &_header{
     display: flex;
     flex-direction:row;
     justify-content: space-between;
     align-items: flex-start;
     &-search{
       margin: 2rem;
       width: 45%;
       height: 2.5rem;
       border-radius: 5px;
       border: none;
       text-align: left;
       padding-left: 1rem;
       cursor: pointer;
       outline: none;
       background-color: $white;
       color: rgba(118, 132, 146, 0.8);
     }
     &-image{
       margin: 2rem;
       width: 20px;
     }
   }
   &_nav{
     display: flex;
     justify-content: space-between;
     align-items: center;
     &-text{
       margin: 2rem;
       font-weight: bold;
       font-family: inherit;
       font-size: 20px;
       color:#011F3B;
     }
     &-list{
      display: flex;
      margin: 2rem;
      font-size: .8rem;
      cursor: pointer;
      .first{
       color: blue;
      }
      .first::before{
        position: absolute;
        content: " ";
        border-bottom: 2px solid #5E81F4;
        background: #5E81F4;
        width: 20px;
        height: 2px;
        left: 61%;
        bottom: 884px;
        top: 17%;
      }    
    }
    li{
      padding-right: .7rem;
      font-family: inherit;
      font-weight: 400;
      color: rgba(118, 132, 146, 0.8);
    }
   }
   &_items{
     display: flex;
     flex-direction: column;
     &-image{
       position: relative;
       width:93%;
       height: 300px;
       margin-left: 2rem;
       border-radius: 10px;
     }
     &-ui{
       width: 55%;
       height: 25%;
        position: absolute;
        z-index: 9999;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        margin: 2rem;
        margin-left:3rem;
        &--top{
          display: flex;
          justify-content: space-between;
          align-items: center;
          &-items{
            &-title{
              margin-bottom: 5px;
              color: #ffff;
              font-family: 'Inter', sans-serif;
              font-size: 1.2rem;
            }
            &-lessons{
              color: rgba(255, 255, 255, 0.8);
              font-family: 'Inter', sans-serif;
              font-size: 1rem;
            }
          }
          &-duration{
            color: rgba(255, 255, 255, 0.8);
            font-family: 'Inter', sans-serif;
            font-size: 1rem;
          }
        }
        &--bottom{
          display: flex;
          justify-content: space-between;
          align-items: center;
        }
      }
     &-second{
       display: flex;
       justify-content: space-between;
       margin-top: 2rem;
       &--1{
         width: 45%;
         height: auto;
         margin-left: 2rem;
         display: flex;
         flex-direction: column;
         justify-content: space-between;
         &-top{
           width: 25%;
            position: absolute;
            z-index: 9999;
            display: flex;
            justify-content: space-between;
            margin: 1.5rem;
             &-items{
            &-title{
              margin-bottom: 5px;
              color: #ffff;
              font-family: 'Inter', sans-serif;
              font-size: 1.2rem;
            }
            &-lessons{
              color: rgba(255, 255, 255, 0.8);
              font-family: 'Inter', sans-serif;
              font-size: 1rem;
            }
          }
          &-duration{
            color: rgba(255, 255, 255, 0.8);
            font-family: 'Inter', sans-serif;
            font-size: 1rem;
          }
         }
         &-bottom{
            width: 25%;
            height: 50%;
            position: absolute;
            z-index: 9999;
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: .7rem;
          }
         img{
           position: relative;
           border-radius: 10px;
         }
       }
       &--2{
         width: 45%;
         height: auto;
         margin-right: 1.5rem;
         img{
           position: relative;
           border-radius: 10px;
         }
       }
     }
   }
 }
</style>
