<template>
  <div class="about">
    <div class="aboutSlide">
      <div class="aboutSlide-img">
        <div class="aboutme">
          <img src="../assets/img/image2.png" alt="error-img" id="aboutme" />
        </div>
        <div class="aboutme-opa"></div>
        <div class="aboutme-txt">
          <div class="txt-aboutme">Về chúng tôi</div>
        </div>
      </div>
      <div class="aboutSlide-txt">
        <div class="aboutSlide-txt_img">
          <img
            src="../assets/img/img-contentLast.png"
            alt="error-img"
            id="aboutSlide-txt_img"
          />
        </div>
        <div class="aboutSlide-txt_txt">
          <div class="txt-title">Về Mirae Asset Prévoir</div>
          <div class="txt-p">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Odio tincidunt cum
            risus morbi adipiscing mauris non. Eget malesuada lectus nisl pellentesque
            elementum dignissim aliquet. Rhoncus pulvinar at amet, et dolor ullamcorper
            gravida nunc sit. Ipsum nisi, nunc tellus lacus, ac lacus ultricies quis
            facilisis.
          </div>
        </div>
      </div>
      <div class="manganer">
        <div class="manganer-target">
          <div class="manganer-target_title">Ban Giám đốc</div>
          <div class="manganer-target_txt">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Odio tincidunt cum
            risus morbi adipiscing mauris non.
          </div>
        </div>
        <!-- <img src="../assets/img/docter1.png" alt="" />
        <img src="../assets/img/docter2.png" alt="" />
        <img src="../assets/img/docter3.png" alt="" />
        <img src="../assets/img/abbank.svg" alt="" />
        <img src="../assets/img/acb.svg" alt="" />
        <img src="../assets/img/msb.svg" alt="" />
        <img src="../assets/img/tbbank.svg" alt="" />
        <img src="../assets/img/pbbank.svg" alt="" />
        <img src="../assets/img/ncb.svg" alt="" />
        <img src="../assets/img/icon-finance.svg" alt="" />
        <img src="../assets/img/icon-finance2.svg" alt="" />
        <img src="../assets/img/noty-dt.png" alt="" />
        <img src="../assets/img/noty-mayin.png" alt="" />
        <img src="../assets/img/noty.png" alt="" />
        <img src="../assets/img/notyy.png" alt="" />
        <img src="../assets/img/finDropDow-right.svg" alt="" />
        <img src="../assets/img/video1.png" alt="" />
        <img src="../assets/img/video2.png" alt="" />
        <img src="../assets/img/video3.png" alt="" /> -->

        <div class="maganer-Icon">
          <vueper-slides
            autoplay
            class="slide-manganer no-shadow thumbnails"
            :arrows="false"
            fixed-height="260px"
          >
            <vueper-slide
              v-for="(item, index) in manganer"
              :key="index"
              :image="item.img"
              id="imgageSlide"
              style="width: 370px; height: 300px"
            />
          </vueper-slides>

          <!-- <div
            class="maganer-leader slider"
            v-for="(item, index) in manganer"
            :key="index"
          >
            <img :src="item.img" alt="error-docter" id="manganerIcon" />
            <div class="managaner-icon_title">{{ item.name }}</div>
            <div class="managaner-icon_txt">{{ item.magan }}</div>
          </div>
          <div class="dropdow-maganer">
            <div class="maganerLeft">
              <img
                src="../assets/img/dropdow-left.png"
                alt="error-slideLeft"
                id="maganerLeft"
              />
            </div>
            <div class="maganerRight">
              <img
                src="../assets/img/dropdow-right.png"
                alt="error-slideReft"
                id="maganerRight"
                @click="nextManganer"
              />
            </div>
          </div> -->
        </div>
      </div>
      <div class="about-distribution">
        <div class="distribution_txt">
          <div class="distribution-title">Kênh phân phối</div>
          <div class="distribution-txt">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Odio tincidunt cum
            risus morbi adipiscing mauris non.
          </div>
        </div>
        <div class="btn_bank">
          <button class="btn-bank">Kênh hợp tác ngân hàng</button>
          <button class="btn-bank">Tổ chức tài chính</button>
          <button class="btn-bank">Tổ chức doanh nghiệp</button>
        </div>
        <div class="about-bank">
          <ul class="bank-about">
            <li class="list-bank">
              <div class="ncb-bank" v-for="(item, index) in bank" :key="index">
                <div class="bank-nc">
                  <img :src="item.img" alt="error-ncb" id="ncb-img" />
                  <div class="ncb-title">{{ item.title }}</div>
                  <div class="ncb-txt">{{ item.txt }}</div>
                </div>
              </div>
            </li>
          </ul>
        </div>
        <div class="abou-Notification">
          <div class="abou-Notification_txt">
            <div class="Notification-title">Thông cáo báo chí</div>
            <div class="Notification-txt">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vulputate amet sit.
            </div>
          </div>

          <div class="abou-Notification_img">
            <ul class="Notification-img">
              <li class="list-Notification">
                <div
                  class="img-Notification"
                  v-for="(item, index) in notification"
                  :key="index"
                >
                  <div class="Notification-ttxt">
                    <img :src="item.img" alt="error-ncb" id="Notification-img" />
                    <div class="ncb-title Notification-title">{{ item.title }}</div>
                    <div class="ncb-txt Notification-txt">{{ item.txt }}</div>
                    <div class="icon-chiteit">
                      <div class="chitiet-txt">{{ item.chitiet }}</div>
                      <div class="chitiet-icon">
                        <img :src="item.icon" alt="" />
                      </div>
                    </div>
                  </div>
                </div>
              </li>
              <div class="NotificationAll">
                <a href="#" class="allNotifion">Xem tất cả</a>
              </div>
            </ul>
          </div>
        </div>
        <div class="finance">
          <ul class="finance-img">
            <li class="list-finance" v-for="(item, index) in finance" :key="index">
              <div class="finance-colum">
                <div class="finance-colum_img">
                  <img :src="item.img" alt="error-finance" />
                </div>
                <div class="finance-colum_title">{{ item.title }}</div>
                <div class="finance-colum_txt">{{ item.txt }}</div>
                <div class="finance-colum_detail">
                  <div class="colum_detail-txt">{{ item.detail }}</div>
                  <div class="colum_detail-img">
                    <img :src="item.icon" alt="" />
                  </div>
                </div>
              </div>
            </li>
          </ul>
        </div>
        <div class="aboutvideo">
          <div class="aboutvideo-item">
            <div class="about-video">
              <div class="about-title">Videos & ảnh</div>
              <div class="about-txt">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vulputate amet
                sit.
              </div>
            </div>
            <ul class="about-video">
              <li class="list-video">
                <!-- <div class="img-video" v-for="(item, index) in video" :key="index">
                  <div class="video-ttxt">
                    <img :src="item.img" alt="error-video" id="video-img" />
                    <div class="video-title">{{ item.title }}</div>
                    <div class="video-txt">{{ item.txt }}</div>
                  </div>
                </div> -->
              </li>
              <div class="NotificationAll">
                <div class="video-nextIcon">
                  <ul class="dots">
                    <!--  -->
                    <li
                      v-for="(dot, index) in slides"
                      :key="index"
                      :class="{ active: ++index === active }"
                      @click="activeClickNex(index)"
                    ></li>
                  </ul>
                </div>
                <a href="#" class="allNotifion">Xem tất cả</a>
              </div>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="contac" v-if="isShowContac">
      <ul class="contac-item">
        <li class="contac-item_link">
          <img src="../assets/img/maytinh.svg" alt="error-maytinh" />
          <div class="border-contac"></div>
        </li>
        <li class="contac-item_link">
          <img src="../assets/img/phoneNumber.svg" alt="error-phone" />
          <div class="border-contac"></div>
        </li>
        <li class="contac-item_link">
          <img src="../assets/img/use.png" alt="error-use" />
          <div class="border-contac"></div>
        </li>
        <li class="contac-item_link">
          <img src="../assets/img/mess.svg" alt="error-mess" />
        </li>
      </ul>
    </div>
    <div class="hover-contac" @click="showIsContac" v-if="isShowBtnContac">
      <div class="contac-item_link contack-Show">
        <img src="../assets/img/mess.svg" alt="error-mess" />
      </div>
    </div>
  </div>
</template>

<script>
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";
// const $ = require("jquery");
// window.$ = $;
export default {
  components: {
    VueperSlides,
    VueperSlide,
  },
  data() {
    return {
      slides: 4, // chuyển video
      activeClick: 1,
      active: 1,
      selectVideo: 0,
      isShowContac: false,
      isShowBtnContac: true,
      selectManganer: 0,

      // swiper
      onSwiper: null,
      onSlideChange: true,
      swiperOptions: {
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
        loop: true,
        slidesPerView: 4.5,
        spaceBetween: 4,
        slidesPerGroup: 4,
        freeMode: true,
        observer: true,
      },
    };
  },
  mounted() {
    // $(document).ready(function ($) {})
  },
  methods: {
    nextManganer() {
      this.selectManganer++;
      if (this.selectManganer >= this.manganer.length) this.manganer = 0;
    },
    /**
     * @description: hàm này dùng để hiển thị thông tin liên hệ với shop
     * Author: NSDThinh 09/02/2023
     */
    showIsContac() {
      this.isShowBtnContac = !this.isShowBtnContac;
      this.isShowContac = !this.isShowContac;
    },
    /**
     * @description: hàm này dùng để chuyển qua lại giữa các video và ảnh
     * Author: NSDThinh 10/02/2023
     */
    jump(index) {
      this.active = index;
    },
    /**
     * @description: hàm này dùng để chuyển qua lại giữa các video và ảnh
     * @param {Object} index - Lấy dữ liệu index của các ảnh
     * Author: NSDThinh - 12//09/2022
     */
    activeClickNex(index) {
      this.selectVideo++;
      if (this.selectVideo >= this.video.length) this.selectVideo = 0;
      this.active = index;
    },
    resetPlay: function () {
      clearInterval(this.timer);
      this.play();
    },
  },
  created() {},
  computed: {
    /**
     * @description: hàm này dùng để lấy dữ liệu từ store giám đốc
     * Author: NSDThinh 09/02/2023
     */
    manganer() {
      return this.$store.state.manganer;
    },
    /**
     * @description: hàm này dùng để lấy dữ liệu từ store ngân hàng
     * Author: NSDThinh 09/02/2023
     */
    bank() {
      return this.$store.state.bank;
    },
    notification() {
      return this.$store.state.notification;
    },
    finance() {
      return this.$store.state.finance;
    },
    video() {
      return this.$store.state.video;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../../src/assets/scss/app.scss";
</style>
