<script >
  export default {
	    data() {
	     return { 
            logo: {
                img: '/img/avada-marketing-logo.png',
                azienda: 'Avada Marketing',
                url: '#',
            },
            links: [
                {
                    title: 'Home',
                    url: '#',
                    active: true,
                    dropDown:[
                        {
                            text: "Hello ( ˘ ³˘)♥",
                            dropurl: '#'
                        },
                        {
                            text: "I'm something ʕ •ᴥ•ʔ",
                            dropurl: '#'
                        },
                        {
                            text: "I'm Something else ૮꒰ ˶• ༝ •˶꒱ა",
                            dropurl: '#'
                        },
                    ]                    
                },
                {
                    title: 'Services',
                    url: '#',
                    active: false,
                    dropDown:[
                        {
                            text: "Hello ( ˘ ³˘)♥",
                            dropurl: '#'
                        },
                        {
                            text: "I'm something ʕ •ᴥ•ʔ",
                            dropurl: '#'
                        },
                        {
                            text: "I'm Something else ૮꒰ ˶• ༝ •˶꒱ა",
                            dropurl: '#'
                        },
                    ]   
                },
                {
                    title: 'Why Us',
                    url: '#',
                    active: false,
                    dropDown: null
                },
                {
                    title: 'Case Studies',
                    url: '#',
                    active: false,
                    dropDown: null
                },
                {
                    title: 'About',
                    url: '#',
                    active: false,
                    dropDown: null
                },
                {
                    title: 'Blog',
                    url: '#',
                    active: false,
                    dropDown: null
                },
                {
                    title:'(555) 802-1234',
                    url: '#',
                    active: false,
                    dropDown: null
                },
            ],
            activeLink: 0,
            button: 'Free Quote',
	      }
	   },
	 }
</script>

<template>

    <header class="my-container">
        <div class="container">

            <ul class="nav">

                <!-- logo -->
                <a class="nav-item" :href="logo.url">
                    <img class="logo" :src="logo.img" :alt="logo.azienda">
                </a>

                <!-- menu -->
                <!-- Ciclo per leggere tutti i link nell'array -->
                <li class="nav-item" v-for="(link, i) in links" :key="i">
                    <!-- 
                    - Al click cambia l'indice del link attivo e si aggiunge la classe active 
                    - Mostra il dropdown solo se dropDown non ha valore null
                    -->
                    <a @click="activeLink = i"
                        :class="{
                            'active' : i == activeLink,
                            'dropdown-toggle' : link.dropDown != null
                        }" 
                        class="nav-link" data-bs-toggle="dropdown" aria-expanded="false" aria-current="page" :href="link.url">
                        {{ link.title }}
                    </a>

                    <!-- Mostra il dropdown menu solo se dropDown non ha valore null -->
                    <ul class="dropdown-menu" v-if="link.dropDown != null">
                        <li v-for="(dropLink, j) in link.dropDown" :key="j">
                            <a class="dropdown-item font-small" :href="dropLink.dropurl">
                                {{ dropLink.text }}
                            </a>
                        </li>
                    </ul>
                    
                </li>

                <!-- bottone finale -->
                <div class="nav-item">
                    <button type="button" class="button light-orange-button">
                        {{ button }}
                    </button>
                </div>

            </ul>
        </div>

    </header>

</template>

<style lang="scss">
  @use 'src/assets/scss/partials/page_header.scss' as *;
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
</style>