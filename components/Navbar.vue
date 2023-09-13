<template>
    <!-- navbar here -->
    <nav class="w-full h-[90px] shadow-md flex justify-between">

        <div class="flex justify-between">
            <div>
                <img class=" h-[60px] ml-15 my-4 align-bottom" src="Mechaverse logo.jpg" alt="mechaverse logo">

            </div>
            <div class="my-7 font-extrabold text-lg">
                MechaVerse
            </div>
        </div>
        <div class="flex justify-between">
            <div>
                <ul class="flex font-semibold text-lg">
                    <li class="m-6">Announcement</li>
                    <li class="m-6">People</li>
                    <li class="m-6">Activities</li>
                    <!-- <li class="m-6"> <a href="MechaVerse\pages\Contactus.vue">Contact Us</a></li> -->
                   <nuxt-link class="m-6" to="/Contactus" >Contact us</nuxt-link>
                </ul>
            </div>
            <div>
                tu logo
            </div>
        </div>
    </nav>
</template>