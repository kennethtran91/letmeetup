<template>
<v-container>
    <v-layout row wrap>
        <v-flex xs12 sm10 md8 offset-sm1 offset-md2>
            <v-card class="info">
                <v-container fluid>
                    <v-layout row>
                        <v-flex xs5>
                            <v-card-media 
                            src="https://www.dentons.com/-/media/images/website/background-images/offices/new-york/new_york_opt_02.jpg"
                            height="130px"
                            >
                            </v-card-media>
                        </v-flex>
                        <v-flex xs7 sm8 md9>
                            <v-card-title primary-title>
                                <div> <h1 class="white--text mb-0">My Meetup</h1>
                                        <div>April 9th, 2017</div>
                            </div>
              </v-card-title>
              <v-card-actions>
                <v-btn flat dark to="/meetups/1"><v-icon left>arrow_forward</v-icon>View Meetup</v-btn>
              </v-card-actions>
                        </v-flex>
                    </v-layout>
                </v-container>
            </v-card>
        </v-flex>  
    </v-layout>
</v-container>
</template>
