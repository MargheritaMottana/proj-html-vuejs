<script >
  export default {
	    data() {
	     return { 
	      }
	   },
	 }
</script>

<template>
    <header class="container my-container">
        <ul class="nav">
            <!-- logo -->
            <a class="nav-item p-1" href="#">
                <img class="logo" src="/public/img/avada-marketing-logo.png" alt="Avada Marketing">
            </a>

            <!-- menu -->
            <li class="nav-item p-1">
                <a class="nav-link active dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false" aria-current="page" href="#">
                    Link
                </a>

                <ul class="dropdown-menu">
                    <li><a class="dropdown-item" href="#">Hello ( ˘ ³˘)♥</a></li>
                    <li><a class="dropdown-item" href="#">I'm something ʕ •ᴥ•ʔ</a></li>
                    <li><a class="dropdown-item" href="#">I'm Something else ૮꒰ ˶• ༝ •˶꒱ა</a></li>
                </ul>
            </li>

            <li class="nav-item p-1">
                <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false" aria-current="page" href="#">
                    Link
                </a>

                <ul class="dropdown-menu">
                    <li><a class="dropdown-item" href="#">Hello ( ˘ ³˘)♥</a></li>
                    <li><a class="dropdown-item" href="#">I'm something ʕ •ᴥ•ʔ</a></li>
                    <li><a class="dropdown-item" href="#">I'm Something else ૮꒰ ˶• ༝ •˶꒱ა</a></li>
                </ul>
            </li>

            <li class="nav-item p-1">
                <a class="nav-link" href="#">Link</a>
            </li>

            <li class="nav-item p-1">
                <a class="nav-link" href="#">Link</a>
            </li>

            <!-- bottone finale -->
             <div class="nav-item p-1">
                <button type="button" class="btn header-button light-orange-button">
                    Free Quote
                </button>
             </div>
        </ul>
    </header>
</template>

<style lang="scss">
  @use 'src/assets/scss/partials/header.scss' as *;
  @use 'src/assets/scss/partials/buttons.scss' as *;
  @use 'src/assets/scss/partials/variables.scss' as *;
</style>