<template>
  <div class="container">

    <div class="sidebar close">
      <Logo />
      <ul class="nav-link">
        <li>

          <nuxt-link to="/" class="link">
            <svg width="30" height="30" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M12.5 25V17.5H17.5V25H23.75V15H27.5L15 3.75L2.5 15H6.25V25H12.5Z" fill="#FAFAFA" />
            </svg>


            <span class="link_name"> Trang chủ</span>
          </nuxt-link>
        </li>
        <li>
          <div class="icon-link">
            <nuxt-link to="/" class="link">
              <svg width="30" height="30" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path
                  d="M5 7.5H2.5V25C2.5 25.663 2.76339 26.2989 3.23223 26.7678C3.70107 27.2366 4.33696 27.5 5 27.5H22.5V25H5V7.5ZM25 2.5C25.663 2.5 26.2989 2.76339 26.7678 3.23223C27.2366 3.70107 27.5 4.33696 27.5 5V20C27.5 20.663 27.2366 21.2989 26.7678 21.7678C26.2989 22.2366 25.663 22.5 25 22.5H10C9.33696 22.5 8.70107 22.2366 8.23223 21.7678C7.76339 21.2989 7.5 20.663 7.5 20V5C7.5 4.33696 7.76339 3.70107 8.23223 3.23223C8.70107 2.76339 9.33696 2.5 10 2.5H25ZM21.25 8.75C21.25 7.75544 20.8549 6.80161 20.1516 6.09835C19.4484 5.39509 18.4946 5 17.5 5C16.5054 5 15.5516 5.39509 14.8483 6.09835C14.1451 6.80161 13.75 7.75544 13.75 8.75C13.75 9.74456 14.1451 10.6984 14.8483 11.4017C15.5516 12.1049 16.5054 12.5 17.5 12.5C18.4946 12.5 19.4484 12.1049 20.1516 11.4017C20.8549 10.6984 21.25 9.74456 21.25 8.75ZM10 18.75V20H25V18.75C25 16.25 20 14.875 17.5 14.875C15 14.875 10 16.25 10 18.75Z"
                  fill="#FAFAFA" />
              </svg>

              <span class="link_name blank"> Xem thông tin </span>

            </nuxt-link>
            <div class="icon-link">
              <svg width="20" height="20" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path
                  d="M4.70391 5.40302L7.55024 8.28685L10.4403 5.44682L11.3146 6.33463L7.53674 10.0553L3.81611 6.27737L4.70391 5.40302Z"
                  fill="white" />
              </svg>
            </div>

          </div>
          <ul class="sub-menu">
            <li>
              <nuxt-link to="/citizen/Family/Family_inf" class="link link_name">Thông tin nhân thân</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/citizen/Leader/" class="link">Thông tin cán bộ</nuxt-link>
            </li>
          </ul>
        </li>
        <li>


          <nuxt-link to="/citizen/GuiYC" class="link">
            <svg width="30" height="30" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path
                d="M27 6H25.5V18C25.5 18.825 24.825 19.5 24 19.5H6V21C6 22.65 7.35 24 9 24H24L30 30V9C30 7.35 28.65 6 27 6ZM22.5 13.5V3C22.5 1.35 21.15 0 19.5 0H3C1.35 0 0 1.35 0 3V22.5L6 16.5H19.5C21.15 16.5 22.5 15.15 22.5 13.5Z"
                fill="white" />
            </svg>
            <span class="link_name">
              Gửi yêu cầu
            </span></nuxt-link>

        </li>
        <li>
          <nuxt-link to="" class="link">
            <svg width="30" height="30" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path
                d="M26.25 16.1125V23.75C26.25 24.413 25.9866 25.0489 25.5178 25.5178C25.0489 25.9866 24.413 26.25 23.75 26.25H18.525C18 27.7 16.625 28.75 15 28.75C13.375 28.75 12 27.7 11.475 26.25H6.25C4.875 26.25 3.75 25.125 3.75 23.75V6.25C3.75 5.58696 4.01339 4.95107 4.48223 4.48223C4.95107 4.01339 5.58696 3.75 6.25 3.75H13.8875C15.4625 2.2 17.6125 1.25 20 1.25C24.8375 1.25 28.75 5.1625 28.75 10C28.75 12.3875 27.8 14.5375 26.25 16.1125ZM15 26.25C15.6875 26.25 16.25 25.6875 16.25 25C16.25 24.3125 15.6875 23.75 15 23.75C14.3125 23.75 13.75 24.3125 13.75 25C13.75 25.6875 14.3125 26.25 15 26.25ZM6.25 6.25V23.75H8.75V21.25H21.25V23.75H23.75V17.9C22.6125 18.4375 21.35 18.75 20 18.75H8.75V16.25H13.875C13.125 15.5375 12.55 14.6875 12.1 13.75H8.75V11.25H11.35C11.2875 10.8375 11.25 10.425 11.25 10C11.25 8.65 11.5625 7.3875 12.1 6.25H6.25ZM20 3.75C16.55 3.75 13.75 6.55 13.75 10C13.75 13.45 16.55 16.25 20 16.25C23.45 16.25 26.25 13.45 26.25 10C26.25 6.55 23.45 3.75 20 3.75ZM20.625 9.6875L24.2 7.575L23.2625 6.05L18.75 8.75V15H20.625V9.6875Z"
                fill="white" />
            </svg>

            <span class="link_name">Xem lịch hẹn</span>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to=" " class="link">
            <svg width="26" height="20" viewBox="0 0 26 20" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path
                d="M3 20C2.3125 20 1.72417 19.7554 1.235 19.2663C0.745 18.7763 0.5 18.1875 0.5 17.5V2.5C0.5 1.8125 0.745 1.22417 1.235 0.735C1.72417 0.245 2.3125 0 3 0H23C23.6875 0 24.2762 0.245 24.7662 0.735C25.2554 1.22417 25.5 1.8125 25.5 2.5V17.5C25.5 18.1875 25.2554 18.7763 24.7662 19.2663C24.2762 19.7554 23.6875 20 23 20H3ZM13 11.25L23 5V2.5L13 8.75L3 2.5V5L13 11.25Z"
                fill="white" />
            </svg>

            <span class="link_name">Đóng góp ý kiến</span>

          </nuxt-link>
        </li>
      </ul>

    </div>
    <div class="user">
      <svg width="37" height="37" viewBox="0 0 37 37" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path
          d="M32.375 29.2917V30.8333H4.625V29.2917L7.70833 26.2083V16.9583C7.70833 12.1792 10.8379 7.97043 15.4167 6.61376V6.16668C15.4167 5.34893 15.7415 4.56467 16.3198 3.98643C16.898 3.40819 17.6822 3.08334 18.5 3.08334C19.3178 3.08334 20.102 3.40819 20.6802 3.98643C21.2585 4.56467 21.5833 5.34893 21.5833 6.16668V6.61376C26.1621 7.97043 29.2917 12.1792 29.2917 16.9583V26.2083L32.375 29.2917ZM21.5833 32.375C21.5833 33.1928 21.2585 33.977 20.6802 34.5553C20.102 35.1335 19.3178 35.4583 18.5 35.4583C17.6822 35.4583 16.898 35.1335 16.3198 34.5553C15.7415 33.977 15.4167 33.1928 15.4167 32.375"
          fill="black" />
      </svg>
      <svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path
          d="M20 6.66666C21.7681 6.66666 23.4638 7.36904 24.714 8.61928C25.9643 9.86952 26.6667 11.5652 26.6667 13.3333C26.6667 15.1014 25.9643 16.7971 24.714 18.0474C23.4638 19.2976 21.7681 20 20 20C18.2319 20 16.5362 19.2976 15.2859 18.0474C14.0357 16.7971 13.3333 15.1014 13.3333 13.3333C13.3333 11.5652 14.0357 9.86952 15.2859 8.61928C16.5362 7.36904 18.2319 6.66666 20 6.66666ZM20 23.3333C27.3667 23.3333 33.3333 26.3167 33.3333 30V33.3333H6.66666V30C6.66666 26.3167 12.6333 23.3333 20 23.3333Z"
          fill="black" />
      </svg>
      <span class="nickname ">Nguyễn Văn Hiệu
        <nuxt-link to="/citizen/changePass" class="passchange example_b">Đổi mật khẩu</nuxt-link>
      </span>
      <nuxt-link to="/login">
        <svg width="30" height="26" viewBox="0 0 30 26" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path
            d="M15.7081 5.39418C15.7096 5.6046 15.6141 5.80714 15.4424 5.95725C15.2706 6.10735 15.0369 6.19272 14.7924 6.19457L7.41924 6.25044C7.33776 6.25106 7.25983 6.27951 7.2026 6.32955C7.14536 6.37958 7.1135 6.4471 7.11403 6.51724L7.21023 19.2118C7.21076 19.2819 7.24364 19.3489 7.30163 19.3981C7.35962 19.4473 7.43797 19.4745 7.51945 19.4739L14.8926 19.418C15.1371 19.4162 15.3721 19.498 15.5461 19.6455C15.7201 19.793 15.8187 19.994 15.8203 20.2045C15.8219 20.4149 15.7263 20.6174 15.5546 20.7675C15.3829 20.9176 15.1491 21.003 14.9046 21.0048L7.53147 21.0607C6.34439 21.0697 5.37468 20.2476 5.36694 19.2257L5.27074 6.53121C5.26702 6.04021 5.49002 5.56762 5.89069 5.21738C6.29136 4.86714 6.83687 4.66795 7.40722 4.66362L14.7804 4.60775C15.0248 4.6059 15.2599 4.68771 15.4339 4.8352C15.6078 4.98268 15.7065 5.18375 15.7081 5.39418Z"
            fill="black" />
          <path
            d="M10.3949 11.6604C10.3928 11.3798 10.5202 11.1098 10.7492 10.9096C10.9781 10.7095 11.2899 10.5957 11.6158 10.5932L17.5831 10.548C17.6085 10.1712 17.6413 9.79639 17.6803 9.41947L17.7147 9.09654C17.7275 8.97484 17.7742 8.85752 17.8509 8.75455C17.9275 8.65157 18.0319 8.56598 18.155 8.50503C18.2782 8.44408 18.4166 8.40958 18.5584 8.40445C18.7002 8.39931 18.8413 8.4237 18.9696 8.47554C21.223 9.38534 23.2663 10.6382 25.001 12.1739L25.0381 12.2064C25.1974 12.3472 25.2871 12.5357 25.2886 12.7324C25.2901 12.9292 25.2032 13.119 25.0461 13.2622L25.0095 13.2952C23.2982 14.857 21.2742 16.1407 19.0349 17.0845C18.9073 17.1383 18.7666 17.1649 18.6247 17.1619C18.4829 17.1589 18.344 17.1265 18.2199 17.0674C18.0958 17.0083 17.9902 16.9243 17.912 16.8225C17.8338 16.7207 17.7853 16.6041 17.7707 16.4826L17.7313 16.1603C17.6867 15.785 17.6482 15.4098 17.6171 15.0334L11.6498 15.0786C11.3238 15.0811 11.0104 14.972 10.7785 14.7753C10.5465 14.5787 10.415 14.3106 10.4129 14.03L10.3949 11.6604Z"
            fill="black" />
        </svg>

      </nuxt-link>
    </div>
    <div class="info">

    </div>
    <nuxt-child />
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
export default {
  components: { Logo },

}
</script>

<style scoped>
* {
  font-family: 'Poppins', sans-serif;


}

html {
  margin: 0;
  padding: 0;
  box-sizing: border-box;


}

.container {
  margin: 0;
  padding: 0;
  overflow: hidden;
  box-sizing: border-box;

}

.sidebar {
  position: absolute;
  width: 272px;
  height: 100%;
  left: -10px;
  top: -2px;

  background: #127E23;
}

.sidebar .nav-link {

  height: 100%;
  padding-top: 35px;

}

.sidebar .nav-link li {

  position: relative;
  list-style: none;
  transition: all 0.4s ease;



}

.sidebar .nav-link li:hover {
  background: #2d953c;


}

.sidebar .nav-link svg {

  text-align: center;
  line-height: 30px;
  padding: 10px;

}

.sidebar .nav-link li .link {
  display: flex;
  align-items: center;
  text-decoration: none;
}

.sidebar .nav-link li .link .link_name {
  font-size: 16px;
  font-weight: 300;
  color: #fff;


}

.sidebar .nav-link li .icon-link {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.sidebar .nav-link li .sub-menu {

  margin-top: -10px;
  background: #197026;
  /*display: none;*/

}

.sidebar .nav-link li .sub-menu .link {
  color: #fff;
  font-size: 15px;
  padding: 5px 0;
  white-space: nowrap;
  opacity: 0.6;
  transition: all 0.3 ease;
}

.sidebar .nav-link li .sub-menu .link:hover {
  opacity: 1;
}

.sidebar.close .nav-link li .sub-menu {

  position: absolute;
  left: 100%;
  top: -10px;
  margin-top: 0;
  padding: 10px 20px;
  border-radius: 0 6px 6px 0;
  transition: all 0.4s ease;
  opacity: 0;
  pointer-events: none;

}

.sidebar.close .nav-link li:hover .sub-menu {
  top: 0;
  opacity: 1;
  pointer-events: auto;
}

.sidebar .nav-link li .sub-menu .link_name {
  display: none;

}

.sidebar.close .nav-link li .sub-menu .link_name {
  font-size: 16px;
  opacity: 1;
  display: block;
}

.sidebar .nav-link li .sub-menu.blank {
  opacity: 1;
  pointer-events: auto;
  padding: 3px 20px 6px 16px;
}

.header .item li {
  position: absolute;
  width: 37px;
  height: 37px;
  left: 1132px;
  top: 19px;

}

.user {
  display: flex;
  justify-content: right;
  align-items: center;
  padding-right: 0px;


}

.user svg {
  width: 40px;
  height: auto;
  padding: 0 15px;
  fill: black;

}

.passchange {
  text-decoration: none;
  display: none;
  color: #000000;
  position: absolute;
  top: 50px;
  right: 45px;
  padding: 10px;
  width: 150px;
}

.nickname:hover .passchange {
  display: block;
}

.nickname {
  padding: 15px 10px;
  border-radius: 4px;
  font-family: 'Poppins', sans-serif;
}

.nickname:hover {
  background-color: #fff;
  color: black;
}</style>