
<script setup>
const router = useRouter()
const isUserLoggedIn = computed(()=>{
  if (process.browser) {
    return JSON.parse(localStorage?.getItem('user')) || '';

  }
})

function logOutUser(params) {
    localStorage.setItem('user', null)
    router.push('/')
  }
</script>

<template>

    <div class="bg-white ">
        <div class="text-white bg-gradient-to-r from-[#00095e] to-[#424770] flex justify-around py-1 fixed top-0 left-0 w-full">
          <div><img src="~/public/Logo.png" alt="" class="h-16  ">
          </div>
    
          <div class="flex gap-10 pt-4">
            <NuxtLink to="/" >
            <ul class="flex gap-1 hover:text-blue-400 cursor-pointer ">Home <svg xmlns="http://www.w3.org/2000/svg"
                fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6 h-6 pt-1  ">
                <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
              </svg>
            </ul>
          </NuxtLink>
            <ul class="flex gap-1 hover:text-blue-400 cursor-pointer ">About <svg xmlns="http://www.w3.org/2000/svg"
                fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6 h-6 pt-1">
                <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
              </svg>
            </ul>
            <ul class="flex gap-1 hover:text-blue-400 cursor-pointer ">Services <svg xmlns="http://www.w3.org/2000/svg"
                fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6 h-6 pt-1">
                <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
              </svg>
            </ul>
            <NuxtLink to="/contact" class="flex gap-1 hover:text-blue-400 cursor-pointer">Contact <svg xmlns="http://www.w3.org/2000/svg"
                fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6 h-6 pt-1">
                <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
              </svg>
            </NuxtLink>

            <NuxtLink to="/Administrator" class="flex gap-1 hover:text-blue-400 cursor-pointer">Administrator <svg xmlns="http://www.w3.org/2000/svg"
                fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6 h-6 pt-1">
                <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
              </svg>
            </NuxtLink>
    
          </div>
    
          
    
          <div>
            <NuxtLink to="/login"  v-if="!isUserLoggedIn"
            >
            <button
              class="  bg-blue-600 hover:bg-blue-400 text-white font-bold py-2 px-8 mt-2 border-b-5 border-blue-700 hover:border-blue-500 rounded-lg">
              Log in 
            </button>
          </NuxtLink>

          <NuxtLink to="/" v-else>
            <button
            @click="logOutUser"
              class="  bg-blue-600 hover:bg-blue-400 text-white font-bold py-2 px-8 mt-2 border-b-5 border-blue-700 hover:border-blue-500 rounded-lg">
              Log out
            </button>
          </NuxtLink>
          </div>
        </div>

      </div>
</template>

