<script setup>  
    import doctor from '../assets/doctor.jpg'
    import one from '../assets/Picture1.png'
    import two from '../assets/Picture2.png'
    import { ref } from 'vue';
    import { Icon } from '@iconify/vue';

    // Importing teams
    import tone from '../assets/who.png'
    import ttwo from '../assets/fasil.png'
    import ad1 from '../assets/amare.png'
    import won from '../assets/won.png'
    import hen from '../assets/hen.png'




    const change = ref(false)

    const toggle =()=>{
        change.value = !change.value
    }

</script>

<template>
    <main class="w-screen">
        <section class="h-[60vh] overflow-y-hidden">
            <img :src="doctor"  alt="">
        </section>
        <div class="w-11/12 sm:w-10/12 mx-auto mt-1 sm:mt-7" id="product">
            <p class="text-3xl text-[#1f438c] font-bold">
                 Introducing the ESMAD: A Low-Cost, Customizable, and High-Quality 3D Printed Stethoscope
            </p>

            <div class="card flex flex-col sm:flex-row shadow-md rounded-md p-3 my-7 space-x-20 items-center justify-center border border-[#1f438c]">
                <div class="flex flex-col items-center justify-center">
                    <img v-if="change" class="w-[80vw] sm:w-[90vw]"  :src="one" alt="">
                    <img v-else class="w-[80vw] h-[50vh]"  :src="two" alt="">

                    <img v-if="change" @click="toggle" class="w-[15vw] sm:w-[5vw]"  :src="two" alt="">
                    <img v-else @click="toggle" class="w-[15vw] sm:w-[5vw]"  :src="one" alt="">

                </div>
                
                <div class="">
                    <p class="font-light">
                        The ESMAD is an exceptional 3D printed stethoscope made in Ethiopia. It offers remarkable sound quality, customization options, and affordability, making it easily accessible to healthcare professionals and enthusiasts. Features include an advanced acoustic chamber for accurate diagnoses, customizable components, low-cost manufacturing, reliability, sustainable production, and the convenience of online ordering. The ESMAD is set to revolutionize the healthcare landscape in Ethiopia and beyond with its game-changing attributes.
                    </p>
                    <div class="flex space-x-2 my-2 items-center">
                        <p class="text-2xl font-bold text-[#1f438c]">1500 Birr </p>
                        <p class="font-light text-sm">Only</p>
                    </div>
                    <div>
                        <button class="bg-[#1f438c] text-white px-5 py-2 rounded-md mt-5 flex items-center justify-center space-x-3">
                            <Icon icon="material-symbols:shopping-cart-outline" color="white" />
                            Order Now
                        </button>
                    </div>
                </div>
            </div>
        </div>


        <!-- Features Section -->
        <div class="w-11/12 sm:w-10/12 mx-auto my-4" id="team">
             <p class="text-3xl text-[#1f438c] font-bold my-4">
                    About Us
            </p>
            <p>
                Meet the team behind the ESMAD. We are a group of passionate and dedicated individuals who are committed to improving the healthcare landscape in Ethiopia and beyond. We are driven by our desire to make a difference in the world and our love for innovation. We are proud to present the ESMAD, a revolutionary 3D printed stethoscope that is set to transform the healthcare industry.
            </p>


            <!-- Team members -->
            <div class="grid sm:grid-cols-2 grid-cols-1">
                <div class="p-3 rounded-md shadow-md flex items-center space-x-7">
                    <img class="w-[20vw]" :src="ttwo" alt="">
                   <div>
                         <p class="font-bold text-lg">Fasil T. BSc Mechanical Engineer, MSc BME(pr.)</p>
                         <span class="text-md font-bold">Founder & CEO of ESMAD</span>
                        <p class="my-2 text-justifyfont-light">CNC Machine developer Developed Portable Medical Oxygen Concentrator, Fetoscope & d/f Mechatronic Projects</p>
                   </div>
                </div>

                 <div class="p-3 rounded-md shadow-md flex items-center justify-between space-x-7">
                        <img class="w-[20vw]" :src="tone" alt="">
                       <div>
                            <p class="font-bold text-lg">Mahider A. BSc Management</p>
                             <span class="text-md font-bold">Founder & CEO of ESMAD</span>
                            <p class="my-2 text-justifyfont-light">Project Lead at OVSI Medical supply chain analysis</p>
                       </div>
                    </div>

                
            </div>



            <p class="text-xl font-bold my-3 text-[#1f438c]">Advisory team</p>

            <div class="grid-cols-1 grid sm:grid-cols-3 gap-5  my-4">
                <div class="p-3 rounded-md shadow-md">
                    <img :src="ad1" alt="">
                    <p class="font-bold text-lg">Amare Kassew (Ph.D..)- Entrepreneur, Project Lead & Software developer</p>
                             
                            <p class="my-2 text-justifyfont-light">BSc, MSc, & Ph.D Electrical Engineer Director at BiTec (Business Incubation)</p>
                            <span class="text-md font-bold">Business Advisor</span>
                </div>

                <div class="p-3 rounded-md shadow-md">
                        <img :src="won" alt="">
                         <p class="font-bold text-lg">Dr. Wondwossen A.</p>
                             
                                <p class="my-2 text-justifyfont-light">Medical Surgeon at Han clinic </p>
                                <span class="text-md font-bold">10 years of work experience</span>
                    </div>

                <div class="p-3 rounded-md shadow-md">
                        <img :src="hen" alt="">
                        <p class="font-bold text-lg">Henok Mebratie</p>
                         <p class="text-md font-bold">Founder & CEO of Lik3D CNC machine Manufacturing</p>
                             
                                <p class="my-2 text-justifyfont-light">Mechanical , Chemical Engineer</p>
                                <!-- <span class="text-md font-bold">Business Advisor</span> -->
                    </div>
            </div>
            
        </div>
    </main>

    <footer class="py-3 w-screen bg-black text-white flex justify-center">
        <p>&copy; all right reserved</p>
    </footer>
</template>



<style  scoped>
   
</style>