<template>
  <div class="plekan-template" v-html="_content" contenteditable="true"></div>
</template>
<script>
  import mixinComponent from 'src/core/mixin'

  var DEFAULT_CONTENT = `
<section class="fdb-block fdb-viewport bg-dark" style="background-image: url(https://picsum.photos/800/600/?random);">
  <div class="container align-items-center justify-content-center d-flex">
    <div class="row align-items-center text-left">
      <div class="col-12 col-sm-10 col-md-8 col-lg-8">
        <h1>Froala Design Blocks is build on Boostrap Framework</h1>
        <p class="lead">Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there.</p>
        <p class="mt-5">
          <a href="https://www.froala.com" class="btn btn-light">Call to Action</a>
          <a href="https://www.froala.com" class="btn btn-dark ml-4">Button</a>
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