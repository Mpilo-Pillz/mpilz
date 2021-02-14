<template>
<nav class="sidebar">
             <ul class="side-nav">
               <router-link v-for="(navItem) in navItems" v-bind:key="navItem" v-bind:to="navItem.route" active-class="router-link-active">
                 <li class="side-nav__item side-nav__link">
                   <span class="user-nav__icon side-nav__icon">

                         <ion-icon v-bind:name="navItem.icon"></ion-icon>
                   </span>
                         <span>{{navItem.title}}</span>
                 </li>
                 </router-link>
             </ul>
             <div class="legal">
                 &copy; 2017 by Dla-mini. Designed by Jonas Schmedttmann
             </div>
         </nav>
  
</template>
<script lang="ts">
export default {
  name: "appNavigator",
  data() {
    return {
      navItems: [
        {
          title: 'Learning',
          route: '/learning',
          icon: 'book'
        },
        {
          title: 'Projects',
          route: '/projects',
          icon: 'laptop'
        },
        {
          title: 'Career',
          route: '/career',
          icon: 'briefcase'
        },
        {
          title: 'Home',
          route: '/',
          icon: 'home'
        },

      ]
    }
  }
};
</script>



