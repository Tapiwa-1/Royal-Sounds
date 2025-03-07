<script setup lang="ts">
import { Head, Link } from '@inertiajs/vue3';
import AppLogoIcon from '../components/AppLogoIcon.vue';
import { Mail, Phone, MapPin } from 'lucide-vue-next';
const services = [
    {
        id: 'event-sound',
        title: 'Event Sound Systems',
        description: 'High-quality PA systems for corporate events, concerts, and private parties.',
        image: '/pictures/event-sound.jpg'
    },
    {
        id: 'microphone-speaker',
        title: 'Microphone & Speaker Rentals',
        description: 'Reliable microphones, speakers, and mixers for clear and professional sound.',
        image: '/pictures/microphone-speaker.jpg'
    },
    {
        id: 'technical-support',
        title: 'Technical Support & Setup',
        description: 'Our expert technicians ensure a seamless audio experience for your event.',
        image: '/pictures/technical-support.jpg'
    }
];
</script>

<template>
    <Head title="PA System Hire">
        <link rel="preconnect" href="https://rsms.me/" />
        <link rel="stylesheet" href="https://rsms.me/inter/inter.css" />
    </Head>

    <div class="relative px-2 flex min-h-screen flex-col items-center bg-[#FDFDFC]  text-[#1b1b18] dark:bg-[#0a0a0a] lg:justify-center ">
        <video autoplay loop muted class="absolute inset-0 hidden w-screen h-screen object-cover lg:block">
                <source src="/videos/pa-system.mp4" type="video/mp4" />
            </video>


        <header class="relative z-10 mb-6 w-full max-w-5xl text-sm">
                <!-- Background Video for Large Screens (Sticky) -->

            <nav class="flex items-center justify-between">
                <Link href="#home" class="text-lg font-bold text-[#1b1b18] dark:text-[#EDEDEC] flex">
                    <div class="flex aspect-square size-8 items-center justify-center rounded-md bg-sidebar-primary text-sidebar-primary-foreground">
                        <AppLogoIcon class="size-5 fill-current text-white dark:text-black" />
                    </div>
                    <div class="">Royal Sounds</div>
                </Link>
                <div class="flex items-center gap-6">
                    <Link href="#about" class="text-sm hover:underline dark:text-[#EDEDEC]">About</Link>
                    <Link href="#services" class="text-sm hover:underline dark:text-[#EDEDEC]">Services</Link>
                    <Link href="#pricing" class="text-sm hover:underline dark:text-[#EDEDEC]">Pricing</Link>
                    <Link href="#contact" class="text-sm hover:underline dark:text-[#EDEDEC]">Contact Us</Link>
                    <Link href="#quote" class="px-5 py-2 text-sm font-medium text-white bg-[#1b1b18] rounded-sm hover:bg-[#3E3E3A] dark:bg-[#EDEDEC] dark:text-[#1b1b18]">
                        Get a Quote
                    </Link>
                </div>
            </nav>
        </header>

        <div id="home" class="relative z-10 flex w-full max-w-5xl items-center justify-center lg:grow">
            <main class="flex w-full flex-col items-center text-center lg:flex-row lg:text-left">
                <div class="flex flex-col my-10 gap-4 max-w-lg">
                    <h1 class="text-3xl font-bold lg:text-5xl text-gray-300">Professional PA System Hire</h1>
                    <p class="text-lg text-gray-300 dark:text-gray-300">
                        Elevate your events with crystal-clear sound. We provide top-quality PA systems for concerts, conferences, weddings, and more.
                    </p>
                    <Link href="#quote" class="mt-5 px-6 py-3 text-lg font-medium text-white bg-[#1b1b18] rounded-sm hover:bg-[#3E3E3A] dark:bg-[#EDEDEC] dark:text-[#1b1b18]">
                        Get a Quote
                    </Link>
                </div>
            </main>
        </div>

        <div id="about" class="relative z-10  bg-fixed bg-center bg-cover w-full max-w-5xl text-white text-justify" style="background-image: url('');">
            <div class="text-2xl font-bold">ABOUT US</div>
            <p class="my-2">Royal Sounds is a premier provider of professional PA system and audio equipment rentals for a diverse range of events across Harare. We cater to corporate functions, weddings, concerts, conferences, parties, and other gatherings, ensuring crystal-clear sound and reliable equipment to enhance the overall event experience. Our mission is to deliver high-quality audio solutions coupled with exceptional customer service, making every event a resounding success.</p>
            <p class="my-2">We offer a comprehensive selection of modern and well-maintained PA systems, microphones, speakers, mixers, and related accessories to meet the specific needs of each client. Our team of experienced technicians provides expert consultation, setup, and on-site support, ensuring seamless operation and optimal sound quality throughout the event.</p>
            <ul class="list-disc pl-6 my-4">
                <li><strong>Superior Equipment:</strong> We invest in and maintain top-of-the-line audio equipment from leading brands, guaranteeing reliability and exceptional sound performance.</li>
                <li><strong>Competitive Pricing:</strong> We offer flexible rental packages tailored to various budgets, providing cost-effective solutions without compromising quality.</li>
                <li><strong>Exceptional Customer Service:</strong> Our dedicated team is committed to providing personalized attention and support, from initial consultation to on-site assistance.</li>
                <li><strong>Local Expertise:</strong> We possess a deep understanding of the Zimbabwean events landscape and can offer valuable insights and recommendations.</li>
            </ul>
            <p class="my-2">Royal Sounds is poised to capitalize on the growing demand for professional audio services in Harare. We are confident that our commitment to quality, service, and affordability will establish us as the preferred choice for PA system rentals, making every event sound exceptional.</p>
        </div>

        <div id="services" class="relative z-10 bg-fixed bg-center text-white bg-cover py-4" style="background-image: url('/pictures/header.jpg');">
            <div class=" max-w-5xl mx-auto px-6">
                <h2 class="text-3xl font-bold text-center mb-6">Our Services</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">


                    <div class="w-full max-w-5xl  bg-white border border-gray-200 rounded-lg shadow-sm">
                        <a href="#">
                            <img class="rounded-t-lg" src="/pictures/service1.jpg" alt="product image" />
                        </a>
                        <div class="px-5 pb-5 pt-2">
                            <a href="#">
                                <h5 class="text-xl font-semibold tracking-tight text-gray-900 ">Event Sound Systems</h5>
                            </a>
                            <p class="tracking-tight text-gray-900 py-3 ">High-quality PA systems for corporate events, concerts, and private parties.</p>
                        </div>
                    </div>
                    <div class="w-full   max-w-5xl bg-white border border-gray-200 rounded-lg shadow-sm">
                        <a href="#">
                            <img class="rounded-t-lg" src="/pictures/service2.jpg" alt="product image" />
                        </a>
                        <div class="px-5 pb-5 pt-2">
                            <a href="#">
                                <h5 class="text-xl font-semibold tracking-tight text-gray-900 ">Event Sound Systems</h5>
                            </a>
                            <p class="tracking-tight text-gray-900 py-3">Reliable microphones, speakers, and mixers for clear and professional sound</p>
                        </div>
                    </div>
                    <div class="w-full  max-w-5xl bg-white border border-gray-200 rounded-lg shadow-sm">
                        <a href="#">
                            <img class=" rounded-t-lg" src="/pictures/service3.jpg" alt="product image" />
                        </a>
                        <div class="px-5 pb-5 pt-2">
                            <a href="#">
                                <h5 class="text-xl font-semibold tracking-tight text-gray-900 ">Technical Support & Setup</h5>
                            </a>
                            <p class="tracking-tight text-gray-900 py-3">Our expert technicians ensure a seamless audio experience for your event.</p>
                        </div>
                    </div>

                </div>
            </div>
        </div>


        <div id="pricing" class="relative z-10 py-16 bg-gray-100 text-black w-full">
            <div class="max-w-5xl mx-auto px-6">
                <h2 class="text-3xl font-bold text-center mb-6">Pricing</h2>
                <p class="text-center mb-8">Affordable and flexible pricing plans for all event sizes.</p>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <img src="/pictures/config1.jpg" alt="Sound SE" class="w-full h-50 object-cover rounded-md mb-4" />
                        <h3 class="text-xl font-bold">Sound SE</h3>
                        <ul class="mt-2 text-sm">
                            <li>✅ Up to 2 Top Speakers</li>
                            <li>✅ 2 Microphones</li>
                            <li>✅ Mixer</li>
                            <li>✅ Suitable for small events (up to 200 people)</li>
                        </ul>
                        <p class="mt-2 text-lg font-semibold">$100 / day</p>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <img src="/pictures/config2.jpg" alt="Sound SE" class="w-full h-50 object-cover rounded-md mb-4" />
                        <h3 class="text-xl font-bold">Sound Plus</h3>
                        <ul class="mt-2 text-sm">
                            <li>✅ Up to 2 Top Speakers</li>
                            <li>✅ 1 Bass Bin for Enhanced Bass</li>
                            <li>✅ 2 Microphones</li>
                            <li>✅ Mixer & Amplifier</li>
                            <li>✅ Suitable for small to medium events (up to 200 people)</li>
                        </ul>
                        <p class="mt-2 text-lg font-semibold">$150 / day</p>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <img src="/pictures/config3.jpg" alt="Sound SE" class="w-full h-50 object-cover rounded-md mb-4" />
                        <h3 class="text-xl font-bold">Sound Pro</h3>
                        <ul class="mt-2 text-sm">
                            <li>✅ Up to 2 Top Speakers</li>
                            <li>✅ 2 Bass Bins for Enhanced Bass</li>
                            <li>✅ 2 Microphones</li>
                            <li>✅ Mixer & Amplifier</li>
                            <li>✅ Suitable for weddings, parties, and events (200+ people)</li>
                        </ul>
                        <p class="mt-2 text-lg font-semibold">$200 / day</p>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <img src="/pictures/config4.jpg" alt="Sound SE" class="w-full h-50 object-cover rounded-md mb-4" />
                        <h3 class="text-xl font-bold">Sound Max</h3>
                        <ul class="mt-2 text-sm">
                            <li>✅ Up to 4 Top Speakers</li>
                            <li>✅ 2 Bass Bins for Enhanced Bass</li>
                            <li>✅ 2 Microphones</li>
                            <li>✅ Mixer & Amplifier</li>
                            <li>✅ Suitable for large events, church services, and concerts (200+ people)</li>
                        </ul>
                        <p class="mt-2 text-lg font-semibold">$300 / day</p>
                    </div>
                </div>
            </div>
        </div>

        <div id="quote" class="relative z-10 py-16 text-white w-full">
            <div class="max-w-xl mx-auto px-6">
                <h2 class="text-3xl font-bold text-center mb-6">Get a Quote</h2>
                <p class="text-center mb-8">Fill out the form below to receive a personalized quote for your event.</p>
                <form class="bg-white p-6 rounded-lg shadow-md w-full text-black">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700">Name</label>
                            <input type="text" class="mt-1 block w-full border-gray-300 rounded-md shadow-sm focus:ring focus:ring-opacity-50 p-2" />
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700">WhatsApp Number</label>
                            <input type="number" class="mt-1 block w-full border-gray-300 rounded-md shadow-sm focus:ring focus:ring-opacity-50 p-2" />
                        </div>
                    </div>
                    <div class="mt-4">
                        <label class="block text-sm font-medium text-gray-700">Event Type</label>
                        <select class="mt-1 block w-full border-gray-300 rounded-md shadow-sm focus:ring focus:ring-opacity-50 p-2">
                            <option>Wedding</option>
                            <option>Corporate Event</option>
                            <option>Concert</option>
                            <option>Private Party</option>
                            <option>Other</option>
                        </select>
                    </div>
                    <div class="mt-4">
                        <label class="block text-sm font-medium text-gray-700">Event Date</label>
                        <input type="date" class="mt-1 block w-full border-gray-300 rounded-md shadow-sm focus:ring focus:ring-opacity-50 p-2" />
                    </div>
                    <div class="mt-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-700">Location</label>
                            <input type="text" class="mt-1 block w-full border-gray-300 rounded-md shadow-sm focus:ring focus:ring-opacity-50 p-2" />
                        </div>
                    </div>
                    <div class="mt-4">
                        <label class="block text-sm font-medium text-gray-700">Additional Requirements</label>
                        <textarea class="mt-1 block w-full border-gray-300 rounded-md shadow-sm focus:ring focus:ring-opacity-50 p-2" rows="4"></textarea>
                    </div>
                    <div class="mt-6 text-center">
                        <button type="submit" class="px-6 py-3 text-lg font-medium text-white bg-[#1b1b18] rounded-sm hover:bg-[#3E3E3A] dark:bg-[#EDEDEC] dark:text-[#1b1b18]">
                            Request Quote
                        </button>
                    </div>
                </form>
            </div>
        </div>


        <footer id="contact" class="relative z-10 bg-cover bg-center bg-gray-900 text-white py-16 w-full" style="background-image: url('/images/contact-bg.jpg');">
            <div class="max-w-5xl mx-auto px-6 text-center">
                <h2 class="text-3xl font-bold mb-6">Contact Us</h2>
                <p class="mb-8">Reach out to us for inquiries and bookings.</p>
                <div class="flex flex-col md:flex-row justify-center items-center gap-6">
                    <div class="flex items-center gap-3">
                        <Phone class="w-6 h-6 text-yellow-400" />
                        <p class="text-lg font-semibold">+263 77 123 4567</p>
                    </div>
                    <div class="flex items-center gap-3">
                        <mail class="w-6 h-6 text-yellow-400" />
                        <p class="text-lg font-semibold">info@royalsounds.co.zw</p>
                    </div>
                    <div class="flex items-center gap-3">
                        <MapPin class="w-6 h-6 text-yellow-400" />
                        <p class="text-lg font-semibold">Harare, Zimbabwe</p>
                    </div>
                </div>
                <div class="mt-8 text-sm opacity-75">&copy; 2024 Royal Sounds. All Rights Reserved.</div>
            </div>
        </footer>


    </div>
</template>

