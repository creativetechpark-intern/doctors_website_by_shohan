
<template>
<container>
    <!-- start header -->
    <header class="absolute top-0 left-0 w-full z-50 px-4 sm:px-8 lg:px-16 xl:px-40 2xl:px-64">
        <div class="hidden md:flex justify-between items-center py-2 border-b text-sm py-3" style="border-color: rgba(255,255,255,.25)">
            <div class="">
                <ul class="flex text-white">
                    <li>
                        <div class="flex items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 fill-current text-white" viewBox="0 0 24 24">
                                <path d="M12,2C7.589,2,4,5.589,4,9.995C3.971,16.44,11.696,21.784,12,22c0,0,8.029-5.56,8-12C20,5.589,16.411,2,12,2z M12,14 c-2.21,0-4-1.79-4-4s1.79-4,4-4s4,1.79,4,4S14.21,14,12,14z" />
                            </svg>
                            <span class="ml-2">1985 Kerry Way, Whittier, CA, USA</span>
                        </div>
                    </li>
                    <li class="ml-6">
                        <div class="flex items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 fill-current text-white" viewBox="0 0 24 24">
                                <path d="M14.594,13.994l-1.66,1.66c-0.577-0.109-1.734-0.471-2.926-1.66c-1.193-1.193-1.553-2.354-1.661-2.926l1.661-1.66 l.701-.701L5.295,3.293L4.594,3.994l-1,1C3.42,5.168,3.316,5.398,3.303,5.643c-0.015,0.25-0.302,6.172,4.291,10.766 C11.6,20.414,16.618,20.707,18,20.707c0.202,0,0.326-0.006,0.358-0.008c0.245-0.014,0.476-0.117,0.649-0.291l1-1l.697-.697 l-5.414-5.414L14.594,13.994z" />
                            </svg>
                            <span class="ml-2">+1 562-789-1935</span>
                        </div>
                    </li>
                </ul>
            </div>

            <div class="">
                <ul class="flex justify-end text-white">
                    <li><a href="#" target="_blank" title="Facebook"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current"><path d="M20,3H4C3.447,3,3,3.448,3,4v16c0,0.552,0.447,1,1,1h8.615v-6.96h-2.338v-2.725h2.338v-2c0-2.325,1.42-3.592,3.5-3.592 c0.699-0.002,1.399,0.034,2.095,0.107v2.42h-1.435c-1.128,0-1.348,0.538-1.348,1.325v1.735h2.697l-0.35,2.725h-2.348V21H20 c0.553,0,1-0.448,1-1V4C21,3.448,20.553,3,20,3z"></path></svg></a></li>
                    <li class="ml-6"><a href="#" target="_blank" title="Twitter"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current"><path d="M19.633,7.997c0.013,0.175,0.013,0.349,0.013,0.523c0,5.325-4.053,11.461-11.46,11.461c-2.282,0-4.402-0.661-6.186-1.809 c0.324,0.037,0.636,0.05,0.973,0.05c1.883,0,3.616-0.636,5.001-1.721c-1.771-0.037-3.255-1.197-3.767-2.793 c0.249,0.037,0.499,0.062,0.761,0.062c0.361,0,0.724-0.05,1.061-0.137c-1.847-0.374-3.23-1.995-3.23-3.953v-0.05 c0.537,0.299,1.16,0.486,1.82,0.511C3.534,9.419,2.823,8.184,2.823,6.787c0-0.748,0.199-1.434,0.548-2.032 c1.983,2.443,4.964,4.04,8.306,4.215c-0.062-0.3-0.1-0.611-0.1-0.923c0-2.22,1.796-4.028,4.028-4.028 c1.16,0,2.207,0.486,2.943,1.272c0.91-0.175,1.782-0.512,2.556-0.973c-0.299,0.935-0.936,1.721-1.771,2.22 c0.811-0.088,1.597-0.312,2.319-0.624C21.104,6.712,20.419,7.423,19.633,7.997z"></path></svg></a></li>
                </ul>
            </div>
        </div>

        <div class="flex flex-wrap items-center justify-between py-6">
            <div class="w-1/4 md:w-auto">
                <a href="index.html" class="font-extrabold text-3xl text-white">The Doctor</a>
            </div>

            <input type="checkbox" id="menu-toggle" class="hidden" />
            <label for="menu-toggle" class="md:hidden block cursor-pointer">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current text-white">
                    <path d="M3,5h18c0.553,0,1-0.447,1-1s-0.447-1-1-1H3c-0.553,0-1,0.447-1,1S2.447,5,3,5z M3,12h18c0.553,0,1-0.447,1-1 s-0.447-1-1-1H3c-0.553,0-1,0.447-1,1S2.447,12,3,12z M3,19h18c0.553,0,1-0.447,1-1s-0.447-1-1-1H3c-0.553,0-1,0.447-1,1 S2.447,19,3,19z"></path>
                </svg>
            </label>
            <div class="w-full md:w-auto">
                <nav class="md:flex space-x-12 text-black">
                    <a href="#" class="block py-2 px-4">Home</a>
                    <a href="#" class="block py-2 px-4">About</a>
                    <a href="#" class="block py-2 px-4">Services</a>
                    <a href="#" class="block py-2 px-4">Contact</a>
                    <a href="#" class="block py-2 px-4 bg-blue-500 text-white rounded-full">Book Appointment</a>
                </nav>
            </div>
        </div>
    </header>
    <!-- end header -->

</container>


</template>