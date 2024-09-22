<script >
  export default {
	    data() {
	     return { 
            title: 'Unlock Your Online Growth Potential',
            message: 'Online marketing to secure customer retention, leads, and sales. We focus on the bigger picture.',
            button: 'Our service',
            
            card:{
                img: '/img/experts/marketing-consultant-expert.jpg',
                name: 'Richard Madsen',
                alt: 'Richard Madsen', 
                role: 'Marketing Consultant Expert',         
                number: '(555) 802-1234',
                terms: 'By submitting my data I agree to be contacted',
                button: 'Get a Callback',
            },
	      }
	   },
	 }
</script>

<template>

    <div class="jumbotron">

        <div class="container">

            <div class="my-container">

                <div class="row">
                    <!-- titolo -->
                    <div class="col text-white">
                        <h1 class="fw-bold mb-3">
                            {{title}}
                        </h1>
                        <p class="fs-5 mb-4">
                            {{ message }}
                        </p>
                        <button type="button" class="button white-button">
                            {{ button }} <i class="fa-solid fa-arrow-right ms-1"></i>
                        </button>
                    </div>

                    <!-- card -->
                    <div class="col">
                        <form class="myCard shadow-lg">
                            <!-- foto -->
                            <img :src="card.img" :alt="card.alt" class="pro-pic rounded-circle mb-2">
                            <p class="fs-5 mb-2">
                                {{ card.name }}
                            </p>
                            <p class="text-secondary font-small">
                                {{ card.role }}
                            </p>
                            <p class="phone-number">
                                <i class="fa-solid fa-phone"></i> 
                                {{ card.number }}
                            </p>

                            <!-- input form -->
                            <div class="form-floating mb-3 mt-3">
                                <input type="name" class="form-control" id="floatingInput" placeholder="Nome" required>
                                <label for="floatingInput" class="text-secondary name-label font-small">
                                    Your Name* <i class="fa-regular fa-id-badge"></i>
                                </label>
                            </div>
                            <div class="form-floating mb-3">
                                <input type="email" class="form-control" id="floatingInput" placeholder="name@example.com" required>
                                <label for="floatingInput" class="text-secondary font-small">
                                    Your Email*
                                </label>
                            </div>
                            <div class="form-floating mb-3">
                                <input type="email" class="form-control" id="floatingInput" placeholder="name@example.com" required>
                                <label for="floatingInput" class="text-secondary font-small">
                                    Your Phone Number*
                                </label>
                            </div>

                            <!-- bottone form -->
                            <button type="submit" class="button orange-button">
                                {{ card.button }}
                            </button>

                            <!-- agree -->
                            <p class="text-secondary card_declaration">
                                {{ card.terms }}
                            </p>
                        </form>
                    </div>
                </div>

            </div>

        </div>

    </div>
</template>

<style lang="scss">
  @use 'src/assets/scss/partials/page_jumbotron.scss' as *;
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
</style>