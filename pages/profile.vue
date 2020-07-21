<template>
    <div>
        <v-card
    :loading="loading"
    class="mx-auto my-12"
    max-width="374"
  >
    <v-img
      height="250"
      src="https://scontent.xx.fbcdn.net/v/t1.15752-0/p280x280/109532145_293940018358357_8769506646343876945_n.jpg?_nc_cat=103&_nc_sid=b96e70&_nc_eui2=AeE7hdall10Dumu9PylFbUa8PTKNfxMcsyY9Mo1_ExyzJugQxqnQ3QxHhH1RWGx6w0guqj8CbBmYWSpvHE5oihGm&_nc_ohc=NDMbobTdjxwAX8NEHMz&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&_nc_tp=6&oh=e2010758053b0a7c617092da04f7aa65&oe=5F3B1F7B"
    ></v-img>

    <v-card-title>นางสาวพรทิพย์  คุณมี</v-card-title>

    <v-card-text>
      <v-row
        align="center"
        class="mx-0"
      >
      </v-row>

      <div class="my-4 subtitle-1">
        ชื่อเล่น อ้อม ปวส.2 E.1
      </div>
      <div>อายุ 19 ปี เกิดวันจันทร์</div>
      <div>ศึกษาอยู่ที่ วิทยาลัยเทคนิคชัยภูมิ</div>
      <div>แผนกเทคโนโลยีสารสนเทศ</div>
    </v-card-text>

    <v-divider class="mx-4"></v-divider>


      </v-btn>
    </v-card-actions>
     <div class="text-center">
            <nuxt-link to="home">
        <v-btn class="ma-2" outlined color="indigo">หน้า Home</v-btn>
        </nuxt-link>
        </div>
  </v-card>
    </div>
</template>
<script>
export default {
    layout:"public",
}
</script>
