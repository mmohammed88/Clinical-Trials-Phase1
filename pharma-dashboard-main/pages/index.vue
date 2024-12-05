<script setup>
import { IconBriefcase } from "@tabler/icons-vue";
import { IconChartAreaLine } from "@tabler/icons-vue";
import { IconGraph } from "@tabler/icons-vue";
import card from "~/components/Card/card.vue";
import { IconBrandFacebook } from '@tabler/icons-vue';



definePageMeta({
  layout: "base-layout",
});

const scrollToSection = (id) => {
    const section = document.getElementById(id);
    if (section) {
        console.log(section.offsetTop);
        window.scrollTo({
            top: section.offsetTop -150,
            behavior: 'smooth' // You can change this to 'auto' for instant scroll
        });
    }

}

</script>
<template>
  <!-- Header -->
  <div class="bg-white ">
   


    


    <!-- </header> -->

    <!-- Hero Section -->
    <!--<section class="bg-white py-20 fade-in">-->
    <div class="grid md:grid-cols-2 items-center justify-center pt-5 mb-10  "
      style="background-image: url('/img/hero.jpg') ;background-repeat: no-repeat; background-size: cover; max-height:700px; min-height:600px;">
      <div class="flex flex-col items-start justify-start gap-4 text-black mx-auto  ml-20 py-20">
        <h1 class="text-5xl font-bold mb-4 text-white">
          Streamline Marketing Intelligence with Vasl AI
        </h1>
        <div class="flex gap-4 ">
          <a href="#" class="bg-blue-600 text-white py-3 px-10 rounded hover:bg-blue-700" @click="scrollToSection('vasl-section')">Learn More</a>
          
          <NuxtLink class="bg-blue-600 text-white py-3 px-10   rounded hover:bg-blue-700 " to="/contact">Contact Us</NuxtLink>          
        </div>
      </div>
      <!--<div class="mx-auto">
        <img
          src="~/public/hero.jpg"
          width="100%"
          height="100%"
          class="mx-auto"
          alt="Image"
        />
      </div>
    -->
    </div>

    <!-- Features Section -->
    <section class="py-2">
      <div class="container mx-auto text-center">
        <!-- <div class="grid grid-cols-1 md:grid-cols-1 gap-5"> -->
        <!-- <div class="bg-white p-5 rounded hover-card">
          <h3 class="text-2xl font-semibold mb-4"></h3>
          <p class="text-gray-700">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
            maxime.
          </p>
        </div> -->
        <!-- </div> -->
        <div class="container mx-auto text-center">
          <div class="w-[70%] mx-auto">Vasl AI goes beyond traditional methods by leveraging a powerful combination of
            Machine Learning, Hyper Automation, and Data Analytics on defined ontologies. This unique approach enables
            Vasl AI to:
          </div>
          <div class="grid grid-cols-1 md:grid-cols-4 gap-8 ">
            <div class="bg-white p-6 hover-card flex flex-col items-center gap-4 hover:shadow-lg transition duration-300">
              <div
                class="w-20 h-20 border-4 border-dotted hover:border-blue-500  border-indigo-600 flex justify-center items-center rounded-full hover:scale-150 transition duration-300">
                <IconBriefcase />
              </div>
              <h3 class="text-2xl font-semibold mb-4 pt-4">Deliver logical and accurate results</h3>
            </div>
            <div class="bg-white p-6 hover-card flex flex-col items-center gap-4 hover:shadow-lg transition duration-300">
              <div
                class="w-20 h-20 border-4 border-dotted hover:border-blue-500 border-indigo-600 flex justify-center items-center rounded-full hover:scale-150 transition duration-300">
                <IconChartAreaLine />
              </div>
              <h3 class="text-2xl font-semibold mb-4">Streamline access to information with Machine Learning</h3>
            </div>
            <div class="bg-white p-6 hover-card flex flex-col items-center gap-4 hover:shadow-lg transition duration-300">
              <div
                class="w-20 h-20 border-4 border-dotted hover:border-blue-500 border-indigo-600 flex justify-center items-center rounded-full hover:scale-150 transition duration-300">
                <IconGraph />
              </div>
              <h3 class="text-2xl font-semibold mb-4">Provide customized dashboards for various user groups</h3>
            </div>
            <div class="bg-white p-6 hover-card flex flex-col items-center gap-4 hover:shadow-lg transition duration-300">
              <div
                class="w-20 h-20 border-4 border-dotted hover:border-blue-500 border-indigo-600 flex justify-center items-center rounded-full hover:scale-150 transition duration-300">
                <IconBriefcase />
              </div>
              <h3 class="text-2xl font-semibold mb-4">Offer downloadable charts, graphs, and summaries</h3>
            </div>
            <!-- <div class="bg-white p-6 rounded shadow-md hover-card border">
        <h3 class="text-2xl font-semibold mb-4">Data Science</h3>
        <p class="text-gray-700">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
          maxime.
        </p>
      </div> -->
            <!-- <div class="bg-white p-6 rounded shadow-md hover-card border">
        <h3 class="text-2xl font-semibold mb-4">Data Science</h3>
        <p class="text-gray-700">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
          maxime.
        </p>
      </div> -->
            <!-- <div class="bg-white p-6 rounded shadow-md hover-card border">
        <h3 class="text-2xl font-semibold mb-4">Data Science</h3>
        <p class="text-gray-700">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
          maxime.
        </p>
      </div> -->
          </div>
        </div>
      </div>
    </section>

    <!--left column-->
    <div class="container bg-white mx-auto text-left cursor-pointer">
      <div class="bg-white px-10 pt-10 rounded">
        <h2 class="text-2xl text-blue-600 font-bold mb-2 ">Why Choose Us</h2>
        
      </div>
      <div class="grid grid-cols-1 md:grid-cols-2">
        <div class="p-10 flex flex-col gap-8 pr-5 text-xl">
          
          <div class="flex items-center space-x-4 ">
            <span
              class="inline-block p-5 rounded-full bg-blue-700   text-white text-lg font-semibold w-8 h-8 flex justify-center items-center">1</span>
            <div class="hover:underline">
              <!-- <h3 class="text-lg font-medium text-gray-800">Data Quality</h3> -->
              <p class="text-gray-600 ">
                <span class="font-bold ">Data Overload:</span> Sifting through massive amounts of data is a struggle.
                Vasl AI simplifies access to relevant information
              </p>
            </div>
          </div>
          <div class="flex items-center space-x-4 ">
            <span
              class="inline-block rounded-full p-5 bg-blue-700 text-white text-lg font-semibold w-8 h-8 flex justify-center items-center">2</span>
            <div class="hover:underline">
              <!-- <h3 class="text-lg font-medium text-gray-800">Data Quality</h3> -->
              <p class="text-gray-600">
                <span class="font-bold">Data Quality:</span> Manual data collection can be error-prone. Vasl AI ensures
                high-quality data through automation.
              </p>
            </div>
          </div>
          <div class="flex items-center space-x-4 ">
            <span
              class="inline-block p-5 rounded-full bg-blue-700 text-white text-lg font-semibold w-8 h-8 flex justify-center items-center">3</span>
            <div class="hover:underline">
              <!-- <h3 class="text-lg font-medium text-gray-800">Data Quality</h3> -->
              <p class="text-gray-600">
                <span class="font-bold">Actionable Insights: </span>Clients demand actionable insights. Vasl AI helps
                generate strategic reports that drive informed decision-making.
              </p>
            </div>
          </div>
          <div class="flex items-center space-x-4">
            <span
              class="inline-block p-5 rounded-full bg-blue-700 text-white text-lg font-semibold w-8 h-8 flex justify-center items-center">4</span>
            <div class=" hover:underline">
              <!-- <h3 class="text-lg font-medium text-gray-800">Data Quality</h3> -->
              <p class="text-gray-600">

                <span class="font-bold">Competitive Differentiation: </span> Standing out in a crowded market is
                crucial. Vasl AI empowers researchers with cutting-edge techniques for a competitive edge.

              </p>
            </div>
          </div>
          <div class="flex items-center space-x-4 ">
            <span
              class="inline-block p-5 rounded-full bg-blue-700 text-white text-lg font-semibold w-8 h-8 flex justify-center items-center">5</span>
            <div class="hover:underline">
              <!-- <h3 class="text-lg font-medium text-gray-800">Data Quality</h3> -->
              <p class="text-gray-600">
                <span class="font-bold"> Client Needs:</span> Meeting client demands for speed, budget, and scope is
                essential. Vasl AI delivers up-to-date insights efficiently.
              </p>
            </div>
          </div>
        </div>
        <img src="~/public/Painpoint.jpg" class=" bg-white h-[510px] w-[480px]"
          alt="Image with custom padding and margin" />
      </div>
    </div>
    <!--right margin-->
    <div class="grid grid-cols-1 md:grid-cols-2 gap-2 bg-white">
      <img src="~/public/Aboutus.jpg" class=" mx-auto h-[510px] w-[480px]"
        alt="Image with custom padding and margin" />
      <div class="bg-white">
        <header class="flex flex-col justify-center py-16 px-4 md:px-8">
          <h2 class="text-2xl  text-blue-800">About Us</h2>
          <h1 class="text-3xl font-bold text-gray-800 my-6">
            We Complete Every Project With Extra Care As Customer Need
          </h1>
          <p class="text-xl text-gray-600 mt-4">
            QALB Holdings, a leading Al-powered tech firm based in London, UK,
            is revolutionizing the life sciences sector with Vasl Al. This
            groundbreaking technology empowers market researchers, business
            analysts, and other professionals with cutting-edge Al solutions for
            market research and competitive intelligence.
          </p>
          
        </header>
      </div>
    </div>

    <!--servicess-->
    <div class="container mx-auto text-center p-10 bg-[#F2FEFE]" id="vasl-section">
      <div>
        <h1 class="text-gray-700 font-bold text-3xl">The Vasl AI solutions</h1>
        <p class="mx-auto w-70 my-6">
          QALB Holdings has created Vasl AI, an on-demand Market Intelligence platform that offers a comprehensive
          solution:
        </p>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8   ">
        <div class="bg-white p-6 rounded shadow-md hover-card border cursor-pointer hover:shadow-lg transition duration-300">
          <h3 class="text-2xl font-semibold mb-4">Data Crawling and Storage</h3>
          <p class="text-gray-700">
            Vasl AI gathers data from various sources and stores it in a secure data warehouse.
          </p>
        </div>
        <div class="bg-white p-6 rounded shadow-md hover-card border cursor-pointer hover:shadow-lg transition duration-300">
          <h3 class="text-2xl font-semibold mb-4">Data Processing</h3>
          <p class="text-gray-700">
            Experts develop algorithms for data mining, cleansing, and organization, making it user-friendly.
          </p>
        </div>
        <div class="bg-white p-6 rounded shadow-md hover-card border cursor-pointer hover:shadow-lg transition duration-300">
          <h3 class="text-2xl font-semibold mb-4">Extensive Database</h3>
          <p class="text-gray-700">
            Vasl AI boasts a vast database encompassing millions of pharmaceutical & biotech products, thousands of
            indications, and hundreds of therapy areas.
          </p>
        </div>
        <div class="bg-white p-6 rounded shadow-md hover-card border cursor-pointer hover:shadow-lg transition duration-300">
          <h3 class="text-2xl font-semibold mb-4">AI-Driven Insights</h3>
          <p class="text-gray-700">
            Vasl AI utilizes Machine Learning to provide logical and accurate solutions across various therapeutic areas
            and indications globally.
          </p>
        </div>
        <div class="bg-white p-6 rounded shadow-md hover-card border cursor-pointer hover:shadow-lg transition duration-300">
          <h3 class="text-2xl font-semibold mb-4">Customizable Dashboards</h3>
          <p class="text-gray-700">
            Users can access information and dashboards tailored to their specific needs.
          </p>
        </div>
        <!-- <div class="bg-white p-6 rounded shadow-md hover-card border cursor-pointer hover:shadow-lg transition duration-300">
          <h3 class="text-2xl font-semibold mb-4">Data Science</h3>
          <p class="text-gray-700">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
            maxime.
          </p>
        </div> -->
      </div>
    </div>

    <!-- <div class="text-center pt-6">
      <h1 class="font-sans text-2xl font-medium text-blue-500">Latest News</h1>
  
      <h3>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Velit molestias unde autem aspernatur quod, non
        voluptatum eius praesentium similique rem</h3>



    </div>
    <card></card> -->

    <!--<section class="bg-blue-600 py-20 text-white">
      <div class="container mx-auto text-center">
        <h2 class="text-3xl font-bold mb-4">Ready to get started?</h2>
        <p class="mb-8">
          Contact us today to learn more about our services and how we can help
          your business grow.
        </p>
        <a
          href="#"
          class="bg-white text-blue-600 py-2 px-4 rounded hover:bg-gray-200"
          >Contact Us</a
        >
      </div>
    </section>
  -->

    <!-- <div class="container mx-auto text-center">
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      <div class="bg-white p-6 rounded shadow-md hover-card">
        <h3 class="text-2xl font-semibold mb-4">Data Science</h3>
        <p class="text-gray-700">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
          maxime.
        </p>
      </div>
      <div class="bg-white p-6 rounded shadow-md hover-card">
        <h3 class="text-2xl font-semibold mb-4">Data Engineering</h3>
        <p class="text-gray-700">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
          maxime.
        </p>
      </div>
      <div class="bg-white p-6 rounded shadow-md hover-card">
        <h3 class="text-2xl font-semibold mb-4">Facing AI Challenges</h3>
        <p class="text-gray-700">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
          maxime.
        </p>
      </div>
    </div>
  </div> -->

    <!-- Call to Action Section -->
    <!-- <section class="bg-blue-600 py-20 text-white">
    <div class="container mx-auto text-center">
      <h2 class="text-3xl font-bold mb-4">Ready to get started?</h2>
      <p class="mb-8">
        Contact us today to learn more about our services and how we can help
        your business grow.
      </p>
      <a
        href="#"
        class="bg-white text-blue-600 py-2 px-4 rounded hover:bg-gray-200"
        >Contact Us</a
      >
    </div>
  </section> -->

    <!-- <div class="container mx-auto text-center">
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      <div class="bg-white p-6 rounded shadow-md hover-card">
        <h3 class="text-2xl font-semibold mb-4">Data Science</h3>
        <p class="text-gray-700">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
          maxime.
        </p>
      </div>
      <div class="bg-white p-6 rounded shadow-md hover-card">
        <h3 class="text-2xl font-semibold mb-4">Data Engineering</h3>
        <p class="text-gray-700">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
          maxime.
        </p>
      </div>
      <div class="bg-white p-6 rounded shadow-md hover-card">
        <h3 class="text-2xl font-semibold mb-4">Facing AI Challenges</h3>
        <p class="text-gray-700">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia,
          maxime.
        </p>
      </div>
    </div>
  </div> -->


    <!-- Footer -->
    <div class="bg-gradient-to-r from-[#00042c] to-[#171147]">
      <footer class="text-white pt-10 pb-5">
        <div class=" bg-dark-blue  text-white container mx-auto px-10 pt-5">
          <div class="flex flex-wrap justify-between items-start bg-dark-400 p-4 text-white ">
            <div class="w-full sm:w-1/4  px-4  ">
              <div>
                <img src="~/public/Logo.png" class="h-[60px] w-[120px]  ">
              </div>
              <p class="text-white">Vasl Al is groundbreaking technology empowers market researchers, business analysts, and other professionals with cutting-edge Al solutions for market research and competitive intelligence.
              </p>
              <div class="flex mt-4 gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                  stroke="#fff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"
                  class="icon icon-tabler icons-tabler-outline icon-tabler-brand-facebook">
                  <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                  <path d="M7 10v4h3v7h4v-7h3l1 -4h-4v-2a1 1 0 0 1 1 -1h3v-4h-3a5 5 0 0 0 -5 5v2h-3" />
                </svg>
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                  stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                  class="icon icon-tabler icons-tabler-outline icon-tabler-brand-x">
                  <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                  <path d="M4 4l11.733 16h4.267l-11.733 -16z" />
                  <path d="M4 20l6.768 -6.768m2.46 -2.46l6.772 -6.772" />
                </svg>
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-brand-linkedin " width="30"
                  height="30" viewBox="0 0 24 24" stroke-width="1.5" stroke="#ffffff" fill="none" stroke-linecap="round"
                  stroke-linejoin="round">
                  <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                  <path d="M4 4m0 2a2 2 0 0 1 2 -2h12a2 2 0 0 1 2 2v12a2 2 0 0 1 -2 2h-12a2 2 0 0 1 -2 -2z" />
                  <path d="M8 11l0 5" />
                  <path d="M8 8l0 .01" />
                  <path d="M12 16l0 -5" />
                  <path d="M16 16v-3a2 2 0 0 0 -4 0" />
                </svg>


              </div>
            </div>
            <div class="w-full sm:w-1/6 mb-4 sm:mb-0 ">
              <h3 class="mb-4 font-bold text-2xl border-b-4 pb-3 border-[#060c4a]">Services</h3>
            </div>
            <div class="w-full sm:w-1/6 mb-4 sm:mb-0 ">
              <h3 class="mb-4 font-bold text-2xl border-b-4 pb-3 border-[#060c4a]">Important Links</h3>
              <ul>
                <li><a href="#" class="text-gray-400 hover:text-white flex items-center">
                    <div><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                        stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                        class="icon icon-tabler icons-tabler-outline icon-tabler-chevrons-right">
                        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                        <path d="M7 7l5 5l-5 5" />
                        <path d="M13 7l5 5l-5 5" />
                      </svg>
                    </div>
                    <span>About Us</span>
                  </a></li>
                <li><a href="#" class="text-gray-400 hover:text-white flex items-center">
                    <div><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                        stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                        class="icon icon-tabler icons-tabler-outline icon-tabler-chevrons-right">
                        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                        <path d="M7 7l5 5l-5 5" />
                        <path d="M13 7l5 5l-5 5" />
                      </svg></div><span>Services</span>
                  </a></li>
              </ul>
            </div>
            <div class="w-full sm:w-1/3">
              <h3 class="mb-4 font-bold text-2xl border-b-4 pb-3 border-[#060c4a] ">Information</h3>
              <ul>
                <div class="flex mt-4 gap-2">

                  <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                    stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                    class="icon icon-tabler icons-tabler-outline icon-tabler-phone">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                    <path
                      d="M5 4h4l2 5l-2.5 1.5a11 11 0 0 0 5 5l1.5 -2.5l5 2v4a2 2 0 0 1 -2 2a16 16 0 0 1 -15 -15a2 2 0 0 1 2 -2" />
                  </svg>
                  <div class="flex flex-col gap-1">
                    <div class="text-gray-400 text-1xl  font-bold text-white ">Phone</div>
                    <span class="text-gray-400 text-white ">+44 (0)20 8470 4967</span>
                  </div>
                  
                </div>

                <div class="flex mt-4 gap-2">

                  <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-mail">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                    <path d="M3 7a2 2 0 0 1 2 -2h14a2 2 0 0 1 2 2v10a2 2 0 0 1 -2 2h-14a2 2 0 0 1 -2 -2v-10z" />
                    <path d="M3 7l9 6l9 -6" />
                  </svg>
                  <div class="flex flex-col gap-1">
                    <div class="text-gray-400 text-1xl  font-bold text-white ">Email</div>
                    <span class="text-gray-400 text-white ">Sales@vaslai.com</span>
                  </div>
                  
                </div>
                <div class="flex mt-4 gap-2">

                  <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-map-pin">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                    <path d="M9 11a3 3 0 1 0 6 0a3 3 0 0 0 -6 0" />
                    <path d="M17.657 16.657l-4.243 4.243a2 2 0 0 1 -2.827 0l-4.244 -4.243a8 8 0 1 1 11.314 0z" />
                  </svg>
                  <div class="flex flex-col gap-1">
                    <div class="text-gray-400 text-1xl  font-bold text-white ">Address</div>
                    <span class="text-gray-400 text-white ">Plashet Grove, London,
                      United Kingdom, E6 1AA</span>
                  </div>
                  
                </div>

                
                
                
                
                
              </ul>
            </div>
          </div>

        </div>
      </footer>
    </div>

    <footer class="bg-gray-800 p-4 text-white text-center">
      <p>&copy; 2024 Vasl AI. All Rights Reserved.</p>
    </footer>
  </div>
</template>
