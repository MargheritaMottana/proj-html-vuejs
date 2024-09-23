<script >
  export default {
	    data() {
	     return { 

            cta:{
                title: 'Grow Your Online Business Strategically, and Improve Customer Retention.',
            },

            sections:{
                Services: 'Services',
                Resources: 'Resources',
                Company: 'Company',
            },
            servicesLinks: [
                {
                    title: 'Marketing Plan',
                    url: '#',               
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
            ],
            ResourcesLinks: [
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
            ],
            CompanyLinks: [
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
            ],
            contacts: {
                info: '© 2020 · Avada Consultant · Powered by WordPress',
                number: 'Call Us (555)802-1234',
                email: 'info@yourcompany.com'
            }
	      }
	   },
	 }
</script>

<template>
    <footer class="container">
        <div class="my-container">

            <div class="row justify-content-between mb-5">
                <h4 class="col-4">
                    {{ cta.title }}
                </h4>
                
                <!-- sezione link 1 -->
                <div class="col-2">
                    <div class="font-small fw-bold mb-3">
                        {{ sections.Services }}
                    </div>
                    <ul class="ps-0">
                        <li v-for="(link, i) in servicesLinks" :key="i">
                            <a class="myLink font-small" :href="link.url">
                                {{ link.title }}
                            </a>
                        </li>
                    </ul>
                </div>

                <!-- sezione link 2 -->
                <div class="col-2">
                    <div class="font-small fw-bold mb-3">
                        {{ sections.Resources }}
                    </div>
                    <ul class="ps-0">
                        <li v-for="(link, i) in ResourcesLinks" :key="i">
                            <a class="myLink font-small" :href="link.url">
                                {{ link.title }}
                            </a>
                        </li>
                    </ul>
                </div>

                <!-- sezione link 3 -->
                <div class="col-2">
                    <div class="font-small fw-bold mb-3">
                        {{ sections.Company }}
                    </div>
                    <ul class="ps-0">
                        <li v-for="(link, i) in CompanyLinks" :key="i">
                            <a class="myLink font-small" :href="link.url">
                                {{ link.title }}
                            </a>
                        </li>
                    </ul>
                </div>

            </div>

            <div class="row">
                <div class="col-5 font-small">
                    {{ contacts.info }}
                </div>
                <div class="col font-small">
                    {{ contacts.number }}
                </div>
                <div class="col font-small text-end">
                    {{ contacts.email }}
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