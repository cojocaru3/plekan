<template>
	<div class="plekan-template" v-html="_content" contenteditable="true"></div>
</template>
<script>
  import mixinComponent from 'src/core/mixin'

  var DEFAULT_CONTENT = `
    <section class="fdb-block pt-0">
      <div class="container-fluid p-0 pb-md-5">
        <iframe class="map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2848.8444388087937!2d26.101253041406952!3d44.43635311654287!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x40b1ff4770adb5b7%3A0x58147f39579fe6fa!2zR3J1cHVsIFN0YXR1YXIgIkPEg3J1yJthIEN1IFBhaWHIm2Ui!5e0!3m2!1sen!2sro!4v1507381157656"
          width="100%" height="300" frameborder="0" style="border:0" allowfullscreen=""></iframe>
      </div>
      <div class="container">
        <div class="row mt-5">
          <div class="col-12 col-md-6 col-lg-5">
            <h2>Contact Us</h2>
            <p class="lead">
              Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove.
            </p>
    
            <p class="lead">
              It is a paradisematic country, in which roasted parts of sentences fly into your mouth.
            </p>
    
    
            <p class="h3 mt-5">
              <strong>Email:</strong> <a href="https://www.froala.com">hello@website.com</a>
            </p>
            <p class="lead">
              <strong>Phone:</strong> <a href="https://www.froala.com">+44 123 123 1232</a>
            </p>
          </div>
    
          <div class="col-12 col-md-6 ml-auto pt-5 pt-md-0">
            <form>
              <div class="row">
                <div class="col-md-6">
                  <div class="form-group">
                    <input type="text" class="form-control" placeholder="First name">
                  </div>
                </div>
                <div class="col-md-6">
                  <div class="form-group">
                    <input type="text" class="form-control" placeholder="Last name">
                  </div>
                </div>
              </div>
    
              <div class="row mt-4">
                <div class="col-md-12">
                  <div class="form-group">
                    <input type="email" class="form-control" placeholder="Enter email">
                  </div>
                </div>
              </div>
    
              <div class="row mt-4">
                <div class="col-md-12">
                  <div class="form-group">
                    <input type="email" class="form-control" placeholder="Subject">
                  </div>
                </div>
              </div>
              <div class="row mt-4">
                <div class="col-md-12">
                  <div class="form-group">
                    <textarea class="form-control" name="message" rows="3" placeholder="How can we help?"></textarea>
                  </div>
                </div>
              </div>
              <div class="row mt-4">
                <div class="col-md-12">
                  <button type="submit" class="btn btn-primary">Submit</button>
                </div>
              </div>
            </form>
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