<template>
    <div>
        <Navbar />
        <div class="mt-14  ">
            <div class="container px-72 content-center text-center">
                <p class="text-5xl  font-extrabold">Events</p>
                <div>
                    <div class="mt-16 flex justify-start space-x-5 border-b-2 border-black">
                        <nuxt-link id="" class="text-lg  font-bold px-5 mb-3 hover:text-[#56A856]" to="/Event">
                            Upcoming Event
                        </nuxt-link>
                        <nuxt-link class="text-lg text-[#56A856] font-bold px-5 mb-3 hover:text-[#56A856] " to="/Pastevent">
                            Past Event
                        </nuxt-link>
                    </div>
                </div>
            </div>
        </div>
        <div class="container px-72 content-center text-center">
            <div class=" mb-28 mt-20 justify-items-center grid grid-cols-3 grid-flow-3 mx-14 gap-y-24 gap-x-20">
                hello 2
            </div>
        </div>
        <Footer />
    </div>
</template>