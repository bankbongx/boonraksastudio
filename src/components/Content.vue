<template>
    <v-container>
        <v-parallax src="https://firebasestorage.googleapis.com/v0/b/pages-3cfa2.appspot.com/o/images%2F56828190_580124655811425_8632822082423488512_o.jpg?alt=media&token=19f369dc-5efd-4650-82f3-751c35e5027a">
            <v-layout text-center wrap>
                <v-flex xs12 mt-12 pt-10>
                    <v-img :src="require('../assets/logos.png')" class="mt-12 pt-12" contain height="200"></v-img>
                </v-flex>
    
                <v-flex mb-4>
                    <h1 class="font-weight-light mb-3 wrap change-font">
                        ยินดีต้อนรับเข้าสู่ บุญรักษา สตูดิโอ
                    </h1>
                    <p class="subheading font-weight-thin change-font">
                        ชมผลงานเพิ่มเติมได้ที่
                        <a  class="white--text " href="https://www.facebook.com/boonruksastudio" target="_blank">บุญรักษา สตูดิโอ</a>
                    </p>
                </v-flex>
            </v-layout>
        </v-parallax>
        <v-layout text-center wrap>
            <v-flex xs12 mt-4 pt-4>
                  <h1 class="font-weight-light mb-3 blue-grey--text change-font">
                       บริการของเรา
                    </h1>
                     <v-container fluid>
      <v-row dense>
        <v-col xs="12" sm="12" md="3" lg="3" xl="3"
          v-for="card in cards"
          :key="card.title"
        >
          <v-card>
            <v-img
              :src="card.src"
              class="white--text align-end change-font font-weight-light"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="400px"
            >
              <v-card-title v-text="card.title"></v-card-title>
            </v-img>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
            </v-flex>
        </v-layout>

<v-layout text-center wrap>
            <v-flex xs12 mt-12 pt-12>
        <v-parallax src="https://firebasestorage.googleapis.com/v0/b/pages-3cfa2.appspot.com/o/boonraksa%2FCAM3_IMG_0003.jpg?alt=media&token=95f535ca-814a-4b4c-9aa6-b88bbbf3ede8">
            <v-layout text-center wrap>
                <v-flex xs12 mt-12 pt-12>
                </v-flex>
    
                <v-flex mb-4>
                    <h1 class=" change-font font-weight-light mb-3">
                        ให้เราได้เก็บภาพความประทับใจของคุณ
                    </h1>
                </v-flex>
            </v-layout>
        </v-parallax>
            </v-flex>
</v-layout>
 <v-layout text-center wrap>
            <v-flex xs12 mt-4 pt-4>
                  <h1 class="change-font font-weight-light mb-3 blue-grey--text">
                      แกลเลอรี่
                    </h1>
                     <v-container fluid>
      <v-row dense>
        <v-col xs="12" sm="12" md="3" lg="3" xl="3"
          v-for="portfolio in portfolios"
          :key="portfolio.title" 
        >
          <v-card xs12 link :href="portfolio.link" target="_blank">
            <v-img
              :src="portfolio.src"
              :href="portfolio.link" target="_blank"
              class="white--text align-end change-font font-weight-light"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="400px"
            >
              <v-card-title class= "change-font font-weight-light" v-text="portfolio.title"></v-card-title>
            </v-img>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
            </v-flex>
        </v-layout>

    </v-container>
</template>

<script>
export default {
    name: 'Content',

    data: () => ({
        cards: [
        { title: 'ถ่ายภาพและถ่ายวิดีโอพรีเวดดิ้ง', src: 'https://firebasestorage.googleapis.com/v0/b/pages-3cfa2.appspot.com/o/boonraksa%2F31603761_370853906738502_139967692776931328_o.jpg?alt=media&token=01119489-0b2f-4cf1-810a-a1a8da5bd601', flex: 3 },
        { title: 'ถ่ายภาพและถ่ายวิดีโองานแต่งงาน', src: 'https://firebasestorage.googleapis.com/v0/b/pages-3cfa2.appspot.com/o/images%2F56830175_580124529144771_7976625146305708032_o.jpg?alt=media&token=46be9754-92e5-4d5f-92d8-ef5a7d3b1657', flex: 3 },
        { title: 'ถ่ายภาพและถ่ายวิดีโองานอีเวนท์', src: 'https://firebasestorage.googleapis.com/v0/b/pages-3cfa2.appspot.com/o/boonraksa%2FCAM3_IMG_0032.jpg?alt=media&token=a63bc899-6977-43f4-8923-5f1e492557a9', flex: 3 },
        { title: 'ถ่ายภาพและถ่ายวิดีโอสินค้าและบริการ', src: 'https://firebasestorage.googleapis.com/v0/b/pages-3cfa2.appspot.com/o/boonraksa%2F57127014_580124722478085_1164299109197152256_o%20(1).jpg?alt=media&token=8da91898-a6f7-4347-97f4-10831d025e56', flex: 3 },
      ],
        portfolios: [
        { title: 'งานแต่งงานคุณจอยและคุณเต้ย', src: 'https://firebasestorage.googleapis.com/v0/b/pages-3cfa2.appspot.com/o/boonraksa%2FIMG_8079.JPG?alt=media&token=754915f3-de09-4dcd-ac4b-7e4d97ad1034', flex: 3, link: 'https://spark.adobe.com/page/T1FDo8cu4SP8N/' },
        { title: 'งานแต่งงานคุณเตยและคุณบิ๊ก', src: 'https://firebasestorage.googleapis.com/v0/b/pages-3cfa2.appspot.com/o/images%2F56830175_580124529144771_7976625146305708032_o.jpg?alt=media&token=46be9754-92e5-4d5f-92d8-ef5a7d3b1657', flex: 3, link: 'https://spark.adobe.com/page/TYdi0NNt09L0l/' },
        { title: 'งานแต่งงานคุณหนูและคุณอุ๊ย', src: 'https://firebasestorage.googleapis.com/v0/b/pages-3cfa2.appspot.com/o/boonraksa%2F43311630_479366119220613_6739889416501723136_o.jpg?alt=media&token=b23fae0d-f578-4231-8cb6-ff1d0ab5c03e', flex: 3 },
        { title: 'งานแต่งงานคุณเอกและคุณกิ๊ก', src: 'https://firebasestorage.googleapis.com/v0/b/pages-3cfa2.appspot.com/o/boonraksa%2F31543442_370789673411592_8877704045146406912_o.jpg?alt=media&token=6ccfea62-ecad-4acb-8cba-cfb31cd44d7d', flex: 3 },
      ],
    }),
};
</script>


<style  scoped>
.change-font {
font-family: 'Sarabun', sans-serif;
}
</style>