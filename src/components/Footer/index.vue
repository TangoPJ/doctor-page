<template>
  <div class="footer_wrapper">
    <div class="footer_frame">
      <div class="fo-title">Вызовите врача на дом</div>
      <div class="footer1">
          <div class="" ></div>

          <div class="">
            
						<div class="logo_img"><img alt="" src="/img/400x0/59e3d50d895b96506b314fa86e125b9e.png"></div>
															
							<div class="address-and-ua">
								 
								<div class="address1"><span style="font-size:17px">ООО «СтройТрейд», 123456, г.Москва, ул. Центральная 1, офис 1<br>ИНН 1234567890 ОГРН 123456789012</span></div>
								 <div class="policy2">Политика конфиденциальности</div> 
							</div>
							<div class="phone-and-address">
								<div class="phone1 zphone show_phone_icon">8 800 333 22 33</div>
								<div class="text1">Звонок по России бесплатный</div>
								<a target="_blank" href="https://tobiz.net/" class="tobiz_link ">Сделано на платформе TOBIZ.NET</a>
									<div class="social_icons  hidden  ">
										<a target="_blank" class="sn sn-vk  link_vk" href=""></a>
										<a target="_blank" class="sn sn-ins  link_ins" href=""></a>
										<a target="_blank" class="sn sn-whatsup  link_whatsup" href=""></a>
										<a target="_blank" class="sn sn-fb  hidden   link_fb" href=""></a>
										<a target="_blank" class="sn sn-youtube  link_youtube" href=""></a>
										<a target="_blank" class="sn sn-o  hidden   link_o" href=""></a>
										<a target="_blank" class="sn sn-viber  hidden   link_viber" href=""></a>
										<a target="_blank" class="sn sn-tg  hidden   link_tg" href=""></a>
									<div class="clear"></div>
									</div>
							</div>
							<div class="clear"></div>
								<div class="policy2_popup">
									<div class="policy2_title">Политика конфиденциальности</div>
									<div class="policy2_body"><p>Данный сайт уважает Ваше право и соблюдает конфиденциальность при заполнении, передаче и хранении Ваших конфиденциальных сведений.<br>Размещение заявки на данном сайте означает Ваше согласие на обработку данных и дальнейшей передачи ваших контактных данных нашей компании.<br>Под персональными данными подразумевается информация, относящаяся к субъекту персональных данных, в частности имя, контактные реквизиты (адрес электронной почты) и иные данные, относимые Федеральным законом от 27 июля 2006 года № 152-ФЗ «О персональных данных» к категории персональных данных.<br>Целью обработки персональных данных является информирование об оказываемых услугах нашей компании.</p></div>
								</div>
						</div>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: "Header",

  setup() {
    
  },
})
</script>

<style lang="scss" scoped>

</style>



<div class="form_wrapper  " style="color:#71b6f9; border-color:#71b6f9;">
                                <div class="form_bg_color" style="opacity:0.5;"></div>
                                <div class="form_title"><span style="font-size:40px;"><span style="color:#424242;"><strong>Вызовите врача на дом</strong></span></span></div>
                                <div class="form1">
                                        <form action="handler.php" enctype="multipart/form-data" method="post">
                                          
                                                <input type="hidden" name="Название формы" value="">	
                                          
                                                <div class="field"><div class="field_title ">Введите имя</div><div class="field_description"></div><div class="field_input field_input_text"><input type="text" required="required" name="Введите имя" placeholder="Введите имя" autocomplete="off"></div></div>
                                          
                                                <div class="field"><div class="field_title  ">Введите номер телефона</div><div class="field_description"></div><div class="field_input field_input_phone"><input type="text" required="required" pattern="[+)( .-]*[0-9]+[0-9+)( .-]*" minlength="6" name="Введите номер телефона" placeholder="xxx-xxx-xxx" autocomplete="off"></div></div>
                                          
                                                <div class="field"><div class="field_title ">Введите адрес</div><div class="field_description"></div><div class="field_input field_input_text"><input type="text" required="required" name="Введите адрес" placeholder="Введите адрес" autocomplete="off"></div></div>
                                          
                                                <div class="field"><div class="field_input"><input type="submit" class="submit_btn surround dark" data-hcolor="#71b6f9" data-action="thanks" data-metrica_event="undefined" data-fb_pixel="undefined" data-vk_pixel="undefined" data-gtag_event="undefined" data-url="" data-amount="0" data-product_name="undefined" value="Оставить заявку" style="background-color: rgb(113, 182, 249); border-radius: 2em; font-size: 18px; border-color: transparent;" autocomplete="off" data-color="rgb(113, 182, 249)"></div></div>
                                        
                                        <div class="clear"></div>
                                        </form>
                                </div>
                                <div class="form_text">Нажимая на кнопку, Вы принимаете <a target="_blank" href="/?personal_data=1">Положение</a> и <a target="_blank" href="/?personal_data=2">Согласие</a> на обработку персональных данных.</div>
                        </div>