<template>
  <div class="wrapper">
    <div class="contener">
      <div class="menu" :class="{ onScroll: !topOfPage }" v-if="isShowMenuPC">
        <ul class="menu-link">
          <li class="menu-item">
            <router-link to="/" class="menu-item_logo">
              <img src="../../assets/img/logo.svg" alt="error-image" id="logoHeader" />
            </router-link>
          </li>
          <li class="menu-item itemMenu">
            <router-link to="/" class="menu-item_product">
              <div class="menu-item_product">Sản phẩm</div>
            </router-link>
          </li>
          <li class="menu-item itemMenu">
            <router-link to="/" class="menu-item_service">
              <div class="menu-item_service">Dịch vụ khách hàng</div>
            </router-link>
          </li>
          <li class="menu-item itemMenu">
            <router-link to="/aboutMirae" class="menu-item_aboutMirae">
              Về Mirae Asset Prévoir
            </router-link>
          </li>
          <li class="menu-item itemMenu">
            <router-link to="/" class="menu-item_news"> Tin tức </router-link>
          </li>
          <li class="menu-icon_mobile" @click="btnMenu">
            <img src="../../assets/img/menu-icon.svg" alt="" id="iconMenum" />
          </li>
        </ul>
        <div class="menu-last">
          <div class="btn-buy">
            <div class="btn-buy_insurance">Mua bảo hiểm trực tuyến</div>
          </div>
          <div class="language">
            <div class="language-icon">
              <img src="../../assets/img/iconHeader.svg" alt="error-language" />
            </div>
            <div class="language-dropdown">
              <img src="../../assets/img/dropdown.svg" alt="error-dropdown" />
            </div>
          </div>
        </div>
      </div>
      <div class="menu-mobile" v-if="isShowMenuMobile">
        <ul class="menu-link">
          <li class="menu-item">
            <router-link to="/" class="menu-item_product menuTxt">
              <div class="menu-item_product" @click="isOfMenu">Sản phẩm</div>
            </router-link>
          </li>
          <li class="menu-item">
            <router-link to="/" class="menu-item_service">
              <div class="menu-item_service" @click="isOfMenu">Dịch vụ khách hàng</div>
            </router-link>
          </li>
          <li class="menu-item" @click="isOfMenu">
            <router-link to="/aboutMirae" class="menu-item_aboutMirae">
              Về Mirae Asset Prévoir
            </router-link>
          </li>
          <li class="menu-item" @click="isOfMenu">
            <router-link to="/" class="menu-item_news"> Tin tức </router-link>
          </li>
          <li class="menu-item">
            <div class="btn-buy">
              <div class="btn-buy_insurance" @click="isOfMenu">
                Mua bảo hiểm trực tuyến
              </div>
            </div>
          </li>
        </ul>
        <div class="closeMenu" @click="showMenuMobile">
          <img src="../../assets/img/x.svg" alt="error-Close" id="closeMobile" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      topOfPage: true,
      isShowMenuMobile: false,
      isShowMenuPC: true
    }
  },
  methods: {
    /**
     * @description: hàm này dùng để tắt form menu
     * Author: NSDThinh 12/02/2023
     */
    isOfMenu () {
      this.isShowMenu(false)
      this.isMenuPC(true)
    },
    /**
     * @description: hàm này dùng để nhận giá trị khi ta truyền vào từ menu
     * @param: {any}
     * Author: NSDThinh 11/02/2023
     */
    isShowMenu (isShowMenuMobile) {
      this.isShowMenuMobile = isShowMenuMobile
    },
    isMenuPC (isShowMenuPC) {
      this.isShowMenuPC = isShowMenuPC
    },
    /**
     * @description: hàm này dùng nhấn để hiển thị thanh menu
     * Author: NSDThinh 11/02/2023
     */
    btnMenu () {
      this.isShowMenu(true)
      this.isMenuPC(false)
    },
    showMenuMobile () {
      this.isShowMenu(false)
      this.isMenuPC(true)
    },
    /**
     * @description: hàm này dùng để cuộn xuống mà vẫn hiển thị thanh menu
     * Author: NSDThinh 09/02/2023
     */
    handleScroll () {
      if (window.pageYOffset > 0) {
        if (this.topOfPage) this.topOfPage = false
      } else {
        if (!this.topOfPage) this.topOfPage = true
      }
    }
  },
  beforeMount () {
    window.addEventListener('scroll', this.handleScroll)
  }
}
</script>

<style lang="scss" scoped>
@import "../../assets/scss/app.scss";
</style>
