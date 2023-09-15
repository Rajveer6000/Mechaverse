<template>
    <div>
        <Navbar />
        <div class="mt-14  ">
            <div class="container px-72 content-center text-center">
                <p class="text-5xl  font-extrabold">Coordinator</p>
                <div>
                    <div class="mt-16 flex justify-start space-x-5 border-b-2 border-black">
                        <nuxt-link id="" class="text-lg text-[#56A856] font-bold px-5 mb-3 hover:text-[#56A856]"
                            to="/people">
                            Faculty Coordinator
                        </nuxt-link>
                        <nuxt-link class="text-lg  font-bold px-5 mb-3 hover:text-[#56A856] " to="/student">
                            Student Representatives
                        </nuxt-link>
                    </div>
                </div>

            </div>
        </div>
        <div class="container px-72 content-center text-center">
            <div class="mb-28 mt-20 justify-items-center grid grid-cols-3 grid-flow-3 mx-14 gap-y-24 gap-x-20">
                <div class="col-span-3">
                    <div class="inline-block">
                        <div class="border-0 h-96 w-72 text-center">
                            <div class=" h-60 w-64 inline-block overflow-hidden bg-center">
                                <img class="w-full h-full object-center object-contain" src="\images\vivekkr.jpg">
                            </div>
                            <p class="font-extrabold text-2xl">Vivek Kumar Metha</p>
                            <p class="font-bold text-lg">Assistant Professor</p>
                            <p class="font-medium text-lg">Department of Mechanical Engineering<br> Tezpur University</p>
                            <p class="font-medium text-lg">Email-id :- vkmetha@tezu.ac.in</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <Footer />
    </div>
</template>
<script>
// Initialization for ES Users

</script>