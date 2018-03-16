/* eslint-disable */
<template>
<v-container>
    <v-layout row wrap>
        <v-flex xs12 sm6 class="text-xs-center text-sm-right">
        <v-btn large router to="/meetups" class="primary">Explore Meetups</v-btn>    
        </v-flex>
        <v-flex xs12 sm6 class="text-xs-center text-sm-left">
            <v-btn large router to="/meetup/new" class="primary">Organize Meetup</v-btn>
        </v-flex>
    </v-layout>
    
    <v-layout row wrap class="mt-2">
        <v-flex xs12>
            <v-carousel>
                <v-carousel-item 
                v-for="meetup in meetups" 
                :src="meetup.imgURL" 
                :key="meetup.id">
                    <div class="title">
                    {{ meetup.title }}
                    </div>
                </v-carousel-item>
            </v-carousel>
        </v-flex>
    </v-layout>
    <v-layout row wrap class="mt-2">
        <v-flex xs12 class="text-xs-center">
        <p>Join our awesome meetups</p>    
        </v-flex>
    </v-layout>
    
</v-container>
</template>

<script>
export default {
    data () {
        return {
            meetups: [
                    { imgURL: 'https://www.dentons.com/-/media/images/website/background-images/offices/new-york/new_york_opt_02.jpg', id: 'img', title: 'Meetup in NY' },
                    { imgURL: 'https://www.gannett-cdn.com/-mm-/dba00a21f9448dcbdf124b912df7088dcabcc972/c=120-0-2001-1414&r=x404&c=534x401/local/-/media/2017/12/18/USATODAY/USATODAY/636492031286101875-GettyImages-505494458.jpg', id: 'paris', title: 'Meetup in Paris' }
                ]
        }
    }
}
</script>

<style scoped>
    .title {
        bottom: 50px;
        background-color: rgba(0, 0, 0, 0.5);
        color: white;
        font-size: 2em;
        padding: 20px;
        text-align: center;
    }
</style>
