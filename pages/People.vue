<template>
    <div>
        <Navbar />
        <div class="mt-14  ">
            <div class=" container font-extrabold px-72 content-center text-center">
                <p class="text-5xl">Coordinator</p>
                <div class="mt-16 flex justify-center space-x-5 ">
                    <p>
                        Faculty
                    </p>
                    <p>
                        Student
                    </p>
                </div>
                <div class="mb-28 mt-20 justify-items-center grid grid-cols-3 grid-flow-3 mx-14 gap-y-24 gap-x-20">
                    <CoCard />
                    <CoCard />
                    <CoCard />
                    <div></div>
                    <CoCard />
                </div>

            </div>
        </div>
        <Footer />
    </div>
</template>
<script>
// Initialization for ES Users

</script>