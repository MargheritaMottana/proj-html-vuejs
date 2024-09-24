<script >
  export default {
	    data() {
	     return { 
            cta:{
                title: 'Grow Your Online Business Strategically, and Improve Customer Retention.',
            },
            menu:[
                {
                    name: 'Service',
                    links:[
                        {
                            title: 'Marketing Plan',
                            url: '#'
                        },
                        {
                            title: 'Sales Development',
                            url: '#',               
                        },
                        {
                            title: 'Digital Marketing',
                            url: '#',               
                        },
                        {
                            title: 'Pricing',
                            url: '#',               
                        },
                        {
                            title: 'Why Us',
                            url: '#',               
                        },
                        {
                            title: 'Cases Studies',
                            url: '#',               
                        },
                    ]
                },
                {
                    name: 'Resources',
                    links:[
                        {
                            title: 'Learning Center',
                            url: '#',               
                        },
                        {
                            title: 'Video Tutorials',
                            url: '#',               
                        },
                        {
                            title: 'Customers',
                            url: '#',               
                        },
                        {
                            title: 'Blog',
                            url: '#',               
                        },
                    ]
                },
                {
                    name: 'Company',
                    links:[
                        {
                            title: 'Who We Are',
                            url: '#',               
                        },
                        {
                            title: 'Contact Us',
                            url: '#',               
                        },
                        {
                            title: 'Careers',
                            url: '#',               
                        },
                    ]
                },
            ],
            copyright: '© 2020 · Avada Consultant · Powered by WordPress',
            contacts: {
                number: 'Call Us (555)802-1234',
                email: 'info@yourcompany.com'
            },
          }
        },
    }
</script>

<template>
    <footer class="container">
        <div class="my-container">

            <!-- cta e menu -->
            <div class="row justify-content-between mb-5">

                <!-- cta & icone -->
                 <div class="col-5">
                    <!-- titolo -->
                    <h4 class="mb-4">
                      {{ cta.title }}
                    </h4>

                    <!-- icone -->
                    <div class="d-flex">
                        <a class="myLink social-icon me-3" href="#">
                            <i class="fa-brands fa-facebook-f"></i>
                        </a>
                        <a class="myLink social-icon me-3" href="#">
                            <i class="fa-brands fa-x-twitter"></i>
                        </a>
                        <a class="myLink social-icon me-3" href="#">
                            <i class="fa-brands fa-instagram"></i>
                        </a>
                        <a class="myLink social-icon me-3" href="#">
                            <i class="fa-brands fa-youtube"></i>
                        </a>
                        <a class="myLink social-icon me-3" href="#">
                            <i class="fa-brands fa-linkedin-in"></i>
                        </a>
                        <a class="myLink social-icon me-3" href="#">
                            <i class="fa-brands fa-tiktok"></i>
                        </a>
                    </div>

                 </div>
                
                <!-- link -->
                <div class="col-2" v-for="(section, i) in menu" :key="i">

                    <!-- titolo sezione -->
                    <div class="font-small fw-bold mb-3">
                        {{ section.name }}
                    </div>

                    <!-- links -->
                    <ul class="ps-0">
                        <li v-for="(link ,i) in section.links" :key="i">
                            <a class="myLink font-small" :href="link.url">
                                {{ link.title }}
                            </a>
                        </li>
                    </ul>

                </div>

            </div>

            <!-- contatti -->
            <div class="row justify-content-between contact-container">

                <div class="col-5 font-small">
                    {{ copyright }}
                </div>

                <div class="col-3 font-small" v-for="(contact, i) in contacts" :key="i">
                    {{ contacts[i] }}
                </div>

            </div>

        </div>
    </footer>
</template>

<style lang="scss">
  @use 'src/assets/scss/partials/page_header.scss' as *;
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
</style>