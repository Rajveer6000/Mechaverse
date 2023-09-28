<template>
    <!-- navbar here -->
    <div>
        <nav class="lg:block w-full h-[60px] lg:h-[90px] shadow-md flex justify-start m-auto lg:px-10" id="top-header">

            <div class="flex justify-between">
                <div class="ml-3  my-auto ">
                    <nuxt-link to="/"><img class="lg:h-16 h-10 w-10 lg:w-16 " src="Mechaverse logo.jpg"
                            alt="mechaverse logo"></nuxt-link>

                </div>
                <div class="my-auto lg:my-7 font-bold lg:font-extrabold  text-lg lg:text-2xl ml-4">
                    <nuxt-link to="/">Mecha<span class=" text-[#56A856]">Verse</span></nuxt-link>
                </div>
            </div>
            <div class="flex justify-start">
                <div>
                    <ul class="flex font-semibold text-lg">
                        <nuxt-link
                            class=" hidden lg:block mx-3 lg:mx-6 my-4 lg:my-8 font-medium text-xs lg:text-lg  lg:font-bold hover:text-[#56A856]"
                            to="/Event">Events</nuxt-link>
                        <nuxt-link
                            class=" hidden lg:block mx-3 lg:mx-6 my-4 lg:my-8 font-medium text-xs lg:text-lg lg:font-bold hover:text-[#56A856]"
                            to="/People">People</nuxt-link>
                        <nuxt-link
                            class=" hidden lg:block mx-3 lg:mx-6 my-4 lg:my-8 font-medium text-xs lg:text-lg lg:font-bold hover:text-[#56A856]"
                            to="/Gallery">Gallery</nuxt-link>
                        <nuxt-link
                            class=" hidden lg:block mx-3 lg:mx-6 my-4 lg:my-8 font-medium text-xs lg:text-lg lg:font-bold hover:text-[#56A856]"
                            to="/Contactus">Contact us</nuxt-link>
                    </ul>
                </div>
                <div class="my-auto hidden lg:block ">
                    <a href="http://www.tezu.ernet.in/" target="_blank"><img class="lg:h-16 lg:w-16" src="TU LOGO.png"
                            alt="TU logo"> </a>
                </div>
            </div>
        </nav>

        <div id="mobile-header" class="fixed left-0 right-0 top-0 z-100 block lg:hidden">
            <div
                class="container max-w-screen-lg px-4 pt-5 pb-5 lg:pb-2 mx-auto space-y-4 lg:space-y-0 lg:flex lg:items-center lg:justify-between lg:space-x-10 bg-white shadow-md">
                <div class="flex justify-between">
                    <NuxtLink to="/" class="nav-link">
                        <img src="Mechaverse logo.jpg" class="w-12 h-12 lg:w-24 lg:h-24">
                    </NuxtLink>
                    <p class="font-semibold text-lg lg:text-2xl tracking-normal text-black mx:16 lg:mx-28">MechaVerse </p>
                    <div class="flex items-center space-x-2 lg:hidden">
                        <svg viewBox="0 0 20 20" fill="currentColor"
                            class="w-6 h-6 text-black p-1  box-content rounded-full" @click="toggleMenuToggle">
                            <path v-if="toggleMenu" fill-rule="evenodd"
                                d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
                                clip-rule="evenodd"></path>
                            <path v-else fill-rule="evenodd"
                                d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
                                clip-rule="evenodd"></path>
                        </svg>
                    </div>
                </div>
                <div class="flex flex-col space-y-4 lg:hidden shadow-md" v-if="toggleMenu">
                    <div
                        class="flex flex-col space-y-3 lg:space-y-0 lg:flex-row lg:space-x-6 xl:space-x-8 lg:items-center pt-5">

                        <NuxtLink to="/Event" class="nav-item">
                            <p class="text-black">Events</p>
                        </NuxtLink>
                        <NuxtLink to="/People" class="nav-item">
                            <p class="text-black">People</p>
                        </NuxtLink>

                        <NuxtLink to="/Gallery" class="nav-item">
                            <p class="text-black">Gallery</p>
                        </NuxtLink>
                        <NuxtLink to="/Contactus" class="nav-item">
                            <p class="text-black">Contact Us</p>
                        </NuxtLink>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            toggleMenu: false,
        }
    },
    mounted() {
        var previousScroll = 0;
        var previousScrollMobile = 0;
        var navbar = document.getElementById('top-header'),
            navClasses = navbar.classList; // classList doesn't work <IE10
        var navbarMobile = document.getElementById('mobile-header'),
            navClassesMobile = navbarMobile.classList; // classList doesn't work <IE10

        window.addEventListener('scroll', function (e) {
            var currentScroll = window.scrollY;
            var isDown = currentScroll > previousScroll;
            var isDownMobile = currentScroll > previousScrollMobile

            if (isDown && !navClasses.contains('scrolled') && currentScroll > 65) {
                // scrolling down, didn't add class yet
                navClasses.add('scrolled'); // we hide the navbar
            } else if (!isDown && currentScroll <= 65) {
                // scrolling up
                navClasses.remove('scrolled'); // won't error if no class found
            }

            console.log(currentScroll)
            if (isDownMobile && !navClassesMobile.contains('scrolled') && currentScroll > 0) {
                // scrolling down, didn't add class yet
                navClassesMobile.add('scrolled'); // we hide the navbar
            } else if (!isDownMobile) {
                // scrolling up
                navClassesMobile.remove('scrolled'); // won't error if no class found
            }

            // always update position
            previousScroll = currentScroll;
            previousScrollMobile = currentScroll;
        });
    },
    watch: {
        $route(to, from) {
            this.toggleMenu = false;
        }
    },
    methods: {
        toggleMenuToggle() {
            this.toggleMenu = !this.toggleMenu;
        },
    }
}
</script>

<style scoped lang="scss">
/*#top-header {
  position: fixed;
  right: 0;
  left: 0;
  top: 0;
  /* your height 
  height: 175px;
  /* .... 
  -webkit-transform: translate3d(0, 0, 0);
  -moz-transform: translate3d(0, 0, 0);
  transform: translate3d(0, 0, 0);
  -webkit-transition: -webkit-transform .4s;
  -moz-transition: -moz-transform .4s;
  -o-transition: transform .4s;
  transition: transform .4s;
} */

#mobile-header {
    position: fixed;
    right: 0;
    left: 0;
    top: 0;
    /* your height */
    height: 77px;
    /* .... */
    -webkit-transition: -webkit-transform .4s;
    -moz-transition: -moz-transform .4s;
    -o-transition: transform .4s;
    transition: transform .4s;
}

.scrolled {
    /* subtract your height */
    -webkit-transform: translate3d(0, -77px, 0);
    -moz-transform: translate3d(0, -77px, 0);
    transform: translate3d(0, -77px, 0);
}

.nav-item {
    @apply text-white border-b-2 border-transparent transition-all py-2
}</style>