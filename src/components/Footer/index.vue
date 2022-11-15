<template>
  <div class="footer_wrapper">
    <div class="footer_frame">
      <div class="footer-1">
        <div class="logo_img">
          <!-- <img alt="" src="/img/400x0/59e3d50d895b96506b314fa86e125b9e.png" /> -->
					<img src="../../assets/images/Dr.Usambaev.png" alt="pic" />
        </div>
      </div>
      <div class="footer2">
        <div class="address-and-ua">
          <div class="address1">
            <span style="font-size: 17px"
              >ООО «СтройТрейд», 123456, г.Москва, ул. Центральная 1, офис 1<br />ИНН
              1234567890 ОГРН 123456789012</span
            >
          </div>
          <div class="policy2">Политика конфиденциальности</div>
        </div>
        <div class="policy2_popup">
          <div class="policy2_title">Политика конфиденциальности</div>
        </div>
      </div>
      <div class="footer3">
        <div class="phone-and-address">
          <div class="phone1 zphone show_phone_icon">8 800 333 22 33</div>
          <div class="text1">Звонок по России бесплатный</div>
        </div>
      </div>
    </div>
  </div>
</template>

<div class="phone1 zphone show_phone_icon">8 800 333 22 33</div>

<script>
import { defineComponent } from "vue";
// import BgImg from "../../assets/images/header-bg.jpeg";

export default defineComponent({
  name: "Header",

  setup() {},
});
</script>

<style lang="scss" scoped>
.footer_wrapper {
	background-color:#EDF5FD ;
	padding: 30px 0;
}

.footer_frame {
	display: flex;
	justify-content: space-around;
	padding: 0 20px 0 20px;
}	

.footer3 {
	text-align: right;
}

img {
	max-width: 200px;
}
</style>
