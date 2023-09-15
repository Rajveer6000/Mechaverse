<template>
    <!-- navbar here -->
    <nav class="w-full h-[90px] shadow-md flex justify-between m-auto">

        <div class="flex justify-between">
            <div>
                <nuxt-link to="/"><img class=" h-[60px] ml-[100px] my-4 " src="Mechaverse logo.jpg"
                        alt="mechaverse logo"></nuxt-link>

            </div>
            <div class="my-7 font-extrabold text-2xl ml-4">
                <nuxt-link to="/">Mecha<span class=" text-[#56A856]">Verse</span></nuxt-link>
            </div>
        </div>
        <div class="flex justify-between">
            <div>
                <ul class="flex font-semibold text-lg">
                    <nuxt-link class="mx-6 my-8 font-bold hover:text-[#56A856]" to="/Activities">Activities</nuxt-link>
                    <nuxt-link class="mx-6 my-8 font-bold hover:text-[#56A856]" to="/People">People</nuxt-link>
                    <nuxt-link class="mx-6 my-8 font-bold hover:text-[#56A856]" to="/Gallery">Gallery</nuxt-link>
                    <nuxt-link class="mx-6 my-8 font-bold hover:text-[#56A856]" to="/Contactus">Contact us</nuxt-link>
                </ul>
            </div>
            <div>
                <a href="http://www.tezu.ernet.in/" target="_blank"><img class="h-[65px] mr-[100px] my-3" src="TU LOGO.png"
                        alt="TU logo"> </a>
            </div>
        </div>
    </nav>
</template>