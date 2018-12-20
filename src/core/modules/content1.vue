<template>
	<div class="plekan-template" v-html="_content" contenteditable="true"></div>
</template>
<script>
  import mixinComponent from 'src/core/mixin'

  var DEFAULT_CONTENT = `
    <section class="fdb-block">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-10 col-sm-6 col-md-5 col-lg-4 m-auto pb-5 pb-md-0">
            <img alt="image" class="img-fluid rounded-0" src="https://picsum.photos/500/300/?random">
          </div>
    
          <div class="col-12 ml-md-auto col-md-7 col-lg-6 pb-5 pb-md-0">
            <img alt="image" class="fdb-icon" src="https://picsum.photos/100/50/?random">
            <h1>Design Blocks</h1>
            <p class="lead">Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts</p>
            <p class="mt-4">
              <a class="btn btn-secondary" href="https://www.froala.com">Download</a>
              <a class="btn btn-dark ml-3" href="https://www.froala.com">Register</a>
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