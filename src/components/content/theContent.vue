<template>
  <div class="content">
    <div class="content-image">
      <vueper-slides autoplay class="slide-Image no-shadow thumbnails" :bullets="false">
        <vueper-slide
          v-for="(item, index) in contentImg"
          :key="index"
          :image="item.slide"
          id="imgageSlide"
        />
      </vueper-slides>

      <!-- <img src="../../assets/img/image.png" alt="" /> -->
      <div class="slide">
        <div class="search-Image">
          <ul class="content-search">
            <li class="content-search_txt">
              <p>
                Sản phẩm <span>Bảo hiểm nhân thọ của MAP Life</span> được thiết kế để phù
                hợp với nhu cầu nhu cầu nhu cầu của bạn
              </p>
            </li>
            <li class="content-search_txt">
              <div class="input-search">
                <input
                  type="text"
                  placeholder="Chọn sản phẩm phù hợp với bạn"
                  id="searchBuy"
                />
                <img
                  src="../../assets/img/dropdown.svg"
                  alt="error-dropdown"
                  id="dropSearch"
                />
              </div>
              <div class="btn-search">Khám phá</div>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="content-body">
      <div class="body_title">
        <div class="body_title-subject">Sản phẩm nổi bật</div>
        <div class="body_title-txt">Khám phá các giải pháp tài chính</div>
      </div>
      <div class="body_column">
        <div class="body_column-link">
          <div class="body_column-image">
            <img
              srcset="../../assets/img/body-column1.png 2x"
              alt="error-image"
              id="body_column-image"
            />
          </div>
          <div class="column-txt">
            <div class="body_column-title">Tên sản phẩm</div>
            <div class="body_column-txt">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit
            </div>
            <a href="#" class="body_column-last">
              <p>Xem chi tiết</p>
              <div class="dropRight">
                <img
                  src="../../assets/img/drop-right.svg"
                  alt="error-dropRight"
                  id="dropRight"
                />
              </div>
            </a>
          </div>
        </div>
        <div class="body_column-link">
          <div class="body_column-image">
            <img
              srcset="../../assets/img/body-column2.png 2x"
              alt="error-image"
              id="body_column-image"
            />
          </div>
          <div class="column-txt">
            <div class="body_column-title">Tên sản phẩm</div>
            <div class="body_column-txt">Lorem ipsum dolor sit amet.</div>
            <a href="#" class="body_column-last">
              <p>Xem chi tiết</p>
              <div class="dropRight">
                <img
                  src="../../assets/img/drop-right.svg"
                  alt="error-dropRight"
                  id="dropRight"
                />
              </div>
            </a>
          </div>
        </div>
        <div class="body_column-link">
          <div class="body_column-image">
            <img
              srcset="../../assets/img/body-column3.png 2x"
              alt="error-image"
              id="body_column-image"
            />
          </div>
          <div class="column-txt">
            <div class="body_column-title">Tên sản phẩm</div>
            <div class="body_column-txt">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut scelerisque
              pulvinar arcu purus commodo egestas suspendisse
            </div>
            <a href="#" class="body_column-last">
              <p>Xem chi tiết</p>
              <div class="dropRight">
                <img
                  src="../../assets/img/drop-right.svg"
                  alt="error-dropRight"
                  id="dropRight"
                />
              </div>
            </a>
          </div>
        </div>
      </div>
    </div>
    <div class="content-service">
      <div class="content-service_column">
        <div class="column_service">
          <div class="column-service">
            <div class="column-service_title">Dịch vụ khách hàng</div>
            <div class="column-service_txt">
              Giải đáp những thắc mắc của khách hàng, chúng tôi cam kết mang đến trải
              nghiệm dịch vụ tối ưu: <span>Nhanh chóng - Hữu ích</span>
            </div>
            <div class="column-service_btn">
              <span class="btn-service">Các dịch vụ khác</span>
            </div>
          </div>
        </div>
        <div class="column-serviceLink">
          <div class="serviceLink-item serviceLink-item2">
            <div class="serviceLink-item_icon">
              <img
                srcset="../../assets/img/icon-insurance.png 2x"
                alt="error-insurance"
                id="serviceLink-item_icon"
              />
            </div>
            <div class="serviceLink-item_title">Đóng phí bảo hiểm</div>
            <div class="serviceLink-item_txt">Lorem ipsum dolor sit amet.</div>
            <a href="#" class="serviceLink-item_last">
              <p class="serviceLink-item-detail">Xem chi tiết</p>
              <div class="dropRight">
                <img
                  src="../../assets/img/drop-right.svg"
                  alt="error-dropRight"
                  id="dropRight"
                />
              </div>
            </a>
          </div>
        </div>
        <div class="column-serviceLink">
          <div class="serviceLink-item serviceLink-item2">
            <div class="serviceLink-item_icon">
              <img
                srcset="../../assets/img/icon-user.png 2x"
                alt="error-user"
                id="serviceLink-item_icon"
              />
            </div>
            <div class="serviceLink-item_title">Cổng thông tin khách hàng</div>
            <div class="serviceLink-item_txt">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit
            </div>
            <a href="#" class="serviceLink-item_last">
              <p class="serviceLink-item-detail">Xem chi tiết</p>
              <div class="dropRight">
                <img
                  src="../../assets/img/drop-right.svg"
                  alt="error-dropRight"
                  id="dropRight"
                />
              </div>
            </a>
          </div>
        </div>
        <div class="column-serviceLink">
          <div class="serviceLink-item serviceLink-item2">
            <div class="serviceLink-item_icon">
              <img
                srcset="../../assets/img/icon-execl.png 2x"
                alt="error-iconExecl"
                id="serviceLink-item_icon"
              />
            </div>
            <div class="serviceLink-item_title">Giải quyết quyền lợi bảo hiểm</div>
            <div class="serviceLink-item_txt">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Platea morbi
              blandit nunc nisl.
            </div>
            <a href="#" class="serviceLink-item_last">
              <p class="serviceLink-item-detail">Xem chi tiết</p>
              <div class="dropRight">
                <img
                  src="../../assets/img/drop-right.svg"
                  alt="error-dropRight"
                  id="dropRight"
                />
              </div>
            </a>
          </div>
        </div>
      </div>
      <div class="content-service_image">
        <img
          srcset="../../assets/img/img-service.png 2x"
          alt="error-service"
          id="service_image"
        />
        <div class="content-service_buy"></div>
        <div class="service_title">
          <div class="service_buy_title">
            <div class="service_buy-txt">Mua bảo hiểm trực tuyến</div>
            <span class="service_buy-btn">Mua ngay</span>
          </div>
        </div>
      </div>
    </div>
    <div class="content-news">
      <div class="content-news_title">
        <div class="news_title">Tin tức mới nhất</div>
        <div class="news_txt">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vulputate amet sit.
        </div>
      </div>
      <div class="content-news_img">
        <div class="news_img-column">
          <div class="img-column">
            <img
              srcset="../../assets/img/news-family.png 2x"
              alt="erro-imgFamily"
              id="img-column"
            />
          </div>
          <div class="news-title">Tên tin tức</div>
          <div class="news-txt">Lorem ipsum dolor sit amet</div>
          <a href="#" class="serviceLink-item_last">
            <p class="serviceLink-item-detail">Xem chi tiết</p>
            <div class="dropRight">
              <img
                src="../../assets/img/drop-right.svg"
                alt="error-dropRight"
                id="dropRight"
              />
            </div>
          </a>
        </div>
        <div class="news_img-column">
          <div class="img-column">
            <img
              srcset="../../assets/img/news-oto.png 2x"
              alt="erro-imgOto"
              id="img-column"
            />
          </div>
          <div class="news-title">Tên tin tức</div>
          <div class="news-txt">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit.
          </div>
          <a href="#" class="serviceLink-item_last">
            <p class="serviceLink-item-detail">Xem chi tiết</p>
            <div class="dropRight">
              <img
                src="../../assets/img/drop-right.svg"
                alt="error-dropRight"
                id="dropRight"
              />
            </div>
          </a>
        </div>
        <div class="news_img-column">
          <div class="img-column">
            <img
              srcset="../../assets/img/news-money.png 2x"
              alt="erro-imgMoney"
              id="img-column"
            />
          </div>
          <div class="news-title">Tên tin tức</div>
          <div class="news-txt">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Semper viverra
            sagittis
          </div>
          <a href="#" class="serviceLink-item_last">
            <p class="serviceLink-item-detail">Xem chi tiết</p>
            <div class="dropRight">
              <img
                src="../../assets/img/drop-right.svg"
                alt="error-dropRight"
                id="dropRight"
              />
            </div>
          </a>
        </div>
        <div class="news_img-column">
          <div class="img-column">
            <img
              srcset="../../assets/img/news-measure.png 2x"
              alt="erro-imgMeasure"
              id="img-column"
            />
          </div>
          <div class="news-title">Tên tin tức</div>
          <div class="news-txt">Lorem ipsum dolor sit amet.</div>
          <a href="#" class="serviceLink-item_last news-title_detial">
            <p class="serviceLink-item-detail">Xem chi tiết</p>
            <div class="dropRight">
              <img
                src="../../assets/img/drop-right.svg"
                alt="error-dropRight"
                id="dropRight"
              />
            </div>
          </a>
        </div>
      </div>
      <div class="news-detailAll">
        <a href="#" class="detailAll">Xem tất cả tin tức</a>
      </div>
    </div>
    <div class="content-last">
      <div class="content-last_img">
        <img
          srcset="../../assets/img/img-contentLast.png 2x"
          alt="error-imgContentLast"
          id="content-last_img"
        />
      </div>
      <div class="content-last_flex">
        <div class="content-last_ipIpadt">
          <div class="Available-ipad">
            <div class="Available-ipad_txt">
              <div class="arrow arrow-down"></div>
              <span class="ipad_txt"> Available</span>
            </div>

            <img srcset="../../assets/img/iPad.png 2x" alt="error-imgIpad" id="ipad" />
          </div>
          <div class="Available-ip">
            <div class="Available-ip_txt">
              <div class="arrow1 arrow-down1"></div>
              <span class="ip_txt"> Available </span>
            </div>
            <img
              srcset="../../assets/img/iPhone.png 2x"
              alt="error-imgIphone"
              id="iphone"
            />
          </div>
        </div>
        <div class="content-last_txt">
          <div class="title-review">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Neque, viverra
            sagittis vitae amet, eu elit.
          </div>
          <div class="txt-review">Ứng dụng phục vụ khách hàng</div>
          <div class="shopPhone">
            <a href="#" class="appStore">
              <img
                srcset="../../assets/img/appStore.png 2x"
                alt="error-imgAppstore"
                id="shopPhone"
              />
            </a>
            <a href="#" class="googlePlay">
              <img
                srcset="../../assets/img/googlePlay.png 2x"
                alt="error-imgGooglePlay"
                id="googlePlay"
              />
            </a>
          </div>
        </div>
      </div>
    </div>

    <div class="contac mobile-contat" v-if="isShowContac">
      <ul class="contac-item">
        <li class="contac-item_link">
          <img src="../../assets/img/maytinh.svg" alt="error-maytinh" />
          <div class="border-contac"></div>
        </li>
        <li class="contac-item_link">
          <img src="../../assets/img/phoneNumber.svg" alt="error-phone" />
          <div class="border-contac"></div>
        </li>
        <li class="contac-item_link">
          <img src="../../assets/img/use.png" alt="error-use" />
          <div class="border-contac"></div>
        </li>
        <li class="contac-item_link">
          <img src="../../assets/img/mess.svg" alt="error-mess" />
        </li>
      </ul>
    </div>
    <div class="hover-contac" @click="showIsContac" v-if="isShowBtnContac">
      <div class="contac-item_link contack-Show">
        <img src="../../assets/img/mess.svg" alt="error-mess" />
      </div>
    </div>
  </div>
</template>

<script>
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";

export default {
  name: "the-content",
  components: {
    VueperSlides,
    VueperSlide,
  },
  data() {
    return {
      selectedSlide: 0, // chọn slide đầu tiên của mảng
      getSlideCount: null, // giá trị ban đầu của ảnh
      isShowContac: false,
      isShowBtnContac: true,
      timer: 0, // cài đặt thời gian ban đầu là 0
    };
  },

  methods: {
    /**
     * @description: hàm này dùng để hiển thị thông tin liên hệ với shop
     * Author: NSDThinh 09/02/2023
     */
    showIsContac() {
      this.isShowBtnContac = !this.isShowBtnContac;
      this.isShowContac = !this.isShowContac;
    },
  },
  computed: {
    /**
     * @description: hàm này dùng để lấy dữ liệu từ store
     * Author: NSDThinh 09/02/2023
     */
    contentImg() {
      return this.$store.state.contenImage;
    },
  },
  created() {
    this.play();
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/app.scss";
</style>
