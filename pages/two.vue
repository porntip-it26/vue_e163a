<template>
<center>
<div style="padding-top:20%;">
    <img src="https://scontent.fbkk3-1.fna.fbcdn.net/v/t1.15752-9/115714488_730176997770994_6572136305799341902_n.jpg?_nc_cat=105&_nc_sid=b96e70&_nc_eui2=AeHoHNrBgn7pbDE-XMiSkkniZVXTOFdx0RVlVdM4V3HRFfqXlE9utFQGdQaxCA4Reig9gO0Gudks7Hm5BAOR3Gy1&_nc_ohc=BSmfoSLiThUAX-TvxZ7&_nc_ht=scontent.fbkk3-1.fna&oh=e618581d97bd49b90344d71a806fd3c1&oe=5F429A76" height="100" width="100" style="margin-top:-225px:100px;border-radius:50%;">
</div>
<br>
<v-card
    class="mx-auto"
    max-width="344"
    style="background:#BDBDBD;"
  >
    <v-card-text>
      <v-form>
    <v-container>
      <v-row>
        <v-col cols="12" sm="4">
          <v-text-field
            label="Username"
            single-line
            outlined
          ></v-text-field>
        </v-col>
         <v-col cols="12" sm="6" style="margin-top:-30px;">
          <v-text-field
            label="Password"
            single-line
            outlined
          ></v-text-field>
        </v-col>

        
      </v-row>
       <v-checkbox
          v-model="absolute"
          label="remember me"
          style="margin-top:-30px;"
        >
        </v-checkbox>
         <p style="margin-top:-45px; margin-left:170px;color:#000;">Forgot Password</p>
    </v-container>
  </v-form>
    </v-card-text>
    <v-card-actions>
      <v-btn
        text
        color="deep-purple accent-4"
      >
       <center><nuxt-link to="three"> <v-btn color="#EC407A" dark style="width:300px; margin-top:-40px;">SIGN IN</v-btn></nuxt-link></center>
      </v-btn>
    </v-card-actions>
  </v-card>
</center>

</template>
<script>
export default {
    layout:'them2',
   
}
</script>
<style>
#app{
    background: #f8f8f8;
}
</style>