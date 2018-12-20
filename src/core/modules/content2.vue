<template>
	<div class="plekan-template" v-html="_content" contenteditable="true"></div>
</template>
<script>
  import mixinComponent from 'src/core/mixin'

  var DEFAULT_CONTENT = `
<section class="fdb-block">
  <div class="col-fill-right" style="background-image: url(https://picsum.photos/600/600/?random);">
  </div>

  <div class="container py-5">
    <div class="row">
      <div class="col-12 col-md-5 text-center">
        <h1>Froala Blocks</h1>
        <p class="lead">Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.</p>
        <p class="mt-4 mb-5"><a class="btn btn-secondary" href="https://www.froala.com">Button</a></p>

        <p>Follow us on</p>
        <p>
          <a href="https://www.froala.com" class="mx-2 text-secondary"><i class="fa fa-twitter"></i></a>
          <a href="https://www.froala.com" class="mx-2 text-secondary"><i class="fa fa-facebook"></i></a>
          <a href="https://www.froala.com" class="mx-2 text-secondary"><i class="fa fa-instagram"></i></a>
          <a href="https://www.froala.com" class="mx-2 text-secondary"><i class="fa fa-pinterest"></i></a>
          <a href="https://www.froala.com" class="mx-2 text-secondary"><i class="fa fa-google"></i></a>
        </p>
      </div>
    </div>
  </div>
</section>`

  export default {
    mixins:[ mixinComponent ],
    data () {
      return {
        DEFAULT_CONTENT : DEFAULT_CONTENT
      }
    }
  }
</script>