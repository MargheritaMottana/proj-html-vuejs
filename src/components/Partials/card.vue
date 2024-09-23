<script >
  export default {
	    data() {
	     return { 
            card:{
                img: '/img/experts/marketing-consultant-expert.jpg',
                name: 'Richard Madsen',
                alt: 'Richard Madsen', 
                role: 'Marketing Consultant Expert',
                iconNumber: '<i class="fa-solid fa-phone"></i>',     
                number: '(555) 802-1234',
                terms: 'By submitting my data I agree to be contacted',
                button: 'Get a Callback',
            },

            input:{
              name: 'Your Name*' ,
              email: 'Your Email*',
              phone: 'Your Phone Number*',
            },
	      }
	   },
	 }
</script>

<template>
    <!-- card -->
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
            <!-- v-html per utilizzare tag html dai data -->
            <span v-html="card.iconNumber"></span>
            {{ card.number }}
        </p>
        

        <!-- input form -->
        <div class="form-floating mb-3 mt-3">
            <input type="text" class="form-control" id="floatingTextarea" placeholder="Nome" required>
            <label for="floatingTextarea" class="text-secondary name-label font-small">
                {{ input.name }} <i class="fa-regular fa-id-badge"></i>
            </label>
        </div>
        <div class="form-floating mb-3">
            <input type="email" class="form-control" id="floatingInput" placeholder="nome@esempio.com" required>
            <label for="floatingInput" class="text-secondary font-small">
                {{ input.email }}
            </label>
        </div>
        <div class="form-floating mb-3">
            <input type="number" class="form-control" id="floatingNumber" placeholder="333 1234 567" required>
            <label for="floatingNumber" class="text-secondary font-small">
                {{ input.phone }}
            </label>
        </div>

        <!-- bottone form -->
        <button type="submit" class="button orange-button">
            {{ card.button }}
        </button>

        <!-- terms -->
        <p class="text-secondary card_terms">
            {{ card.terms }}
        </p>
    </form>
</template>

<style lang="scss">
  @use 'src/assets/scss/partials/card.scss' as *;
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
</style>