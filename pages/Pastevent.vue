<template>
    <div>
        <Navbar />
        <div class="mt-8 lg:mt-14">
            <div class="container px-8 lg:px-72  content-center text-center">
                <p class="text-xl lg:text-5xl  font-extrabold">Events</p>
                <div>
                    <div class="mt-10 lg:mt-16 flex lg:justify-start justify-between px-5  lg:space-x-5 border-b-2 border-black">
                        <nuxt-link id="" class="text-xs lg:text-lg  font-bold px-5 mb-1 lg:mb-3 hover:text-[#56A856] " to="/Event">
                            Upcoming Event
                        </nuxt-link>
                        <nuxt-link class="text-xs lg:text-lg text-[#56A856] font-bold px-5 mb-1 lg:mb-3 hover:text-[#56A856]" to="/Pastevent">
                            Past Event
                        </nuxt-link>
                    </div>
                </div>
            </div>
        </div>
        <div class="container px-8 lg:px-72  content-center text-center">
            <div class=" lg:mb-28 mt-14 lg:mt-20 justify-items-center grid  grid-cols-1 lg:grid-cols-3 lg:grid-flow-3 mx-14 lg:gap-y-24 gap-x-20">
                <!-- //past Events -->
                <div class="w-[250px] h-[586px]">
                    <div class="inline-block max-w-sm rounded overflow-hidden shadow-lg">
                        <img class="w-full h-[250px]" src="\images\emerging trends.jpeg" alt="Emerging trends in technology">
                        <div class="px-6 py-4">
                            <div class="font-bold text-xl mb-2">Emerging trends in technology</div>
                            <p class="text-gray-700 text-base">
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maioreset perferendiseaque, exercitationem praesentium nihil.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="w-[250px] h-[586px]">
                    <div class="inline-block max-w-sm rounded overflow-hidden shadow-lg">
                        <img class="w-full h-[250px]" src="\images\eng simulation.jpeg" alt="Engineerig simulation">
                        <div class="px-6 py-4">
                            <div class="font-bold text-xl mb-2">Engineerig Simulation</div>
                            <p class="text-gray-700 text-base">
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maioreset perferendiseaque, exercitationem praesentium nihil.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="w-[250px] h-[586px]">
                    <div class="inline-block max-w-sm rounded overflow-hidden shadow-lg">
                        <img class="w-full h-[250px]" src="\images\fem.jpeg" alt="FEm">
                        <div class="px-6 py-4">
                            <div class="font-bold text-xl mb-2">Introduction to FEM</div>
                            <p class="text-gray-700 text-base">
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maioreset perferendiseaque, exercitationem praesentium nihil.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="w-[250px] h-[586px] lg:col-span-3">
                    <div class="inline-block max-w-sm rounded overflow-hidden shadow-lg">
                        <img class="w-full h-[250]" src="\images\cfd.webp" alt="CFD">
                        <div class="px-6 py-4">
                            <div class="font-bold text-xl mb-2">Introduction to Computational Fluid Dynamics</div>
                            <p class="text-gray-700 text-base">
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maioreset perferendiseaque, exercitationem praesentium nihil.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <Footer />
    </div>
</template>