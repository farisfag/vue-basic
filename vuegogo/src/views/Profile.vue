<template>
  <div class="profile">
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-lg-6">
                <div class="media text-left">
                    <img  src="../assets/instagramlogo.png" class="mr-3 user-pic " >
                    <div class="media-body">
                        <h5 class="mt-0">{{ firstName }}{{ lastName }}</h5>
                        <p>{{content}}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>

import 'bootstrap/dist/css/bootstrap.css'

export default {
  name: 'Profile',
  data: function (){
      return {
      firstName: 'Instagram',
      lastName : '.com',
      content : 'Instgram is a social media platform for anybody to share about their activities. They can share photos or videos to their profile and it shwon to their follower.'
      }
  },
  components: {

  }
}
</script>

<style  scoped>
    .user-pic{
        height :120px;
        width :120 px;
       
    }
</style>
