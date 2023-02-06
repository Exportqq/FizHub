<template>
  <div>
    <div :style="{ display: AllPageDisplay}">
      <div class="backround-app-site">
        <div class="all_padding">
          <div class="header_navigation">
            <ul class="list_header">
              <li>
                <img src="logo.svg" alt="logo" class="logo">
              </li>
              <li>
                <button class="header-txt">Законы</button>
              </li>
              <li>
                <button class="header-txt">Теория</button>
              </li>
              <li>
                <button class="header-txt-on">Лабораторные работы</button>
              </li>
            </ul>
            <div>
              <ul class="list">
                <li class="animation_navigation">
                  <p class="header_txt_two">С нами Физика станет <span style="color: #FFF500;">доступнее, проще, понятнее</span></p>
                </li>
                <li>
                  <img class="animation_cube" src="4dIu.gif" alt="animation_cube">
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="all_padding">
        <div class="container">
          <p class="cont_txt">Выполнили студенты</p>
          <table>
            <tr>
              <td>
                <div class="student_one_rectangle">
                  <table>
                    <tr>
                      <td>
                        <img class="student_img" src="unnamedone.png">
                      </td>
                    </tr>
                    <tr>
                      <td>
                        <p class="name_person">Саакян Михаил Группа: 117ИС</p>
                        <p class="work_person">Специальность: Информационные системы</p>
                      </td>
                    </tr>
                  </table>
                </div>
              </td>
              <td class="navigation_person_rectangle">
                <div class="student_two_rectangle">
                  <table>
                    <tr>
                      <td>
                        <img class="student_img" src="unnamedtwo.png">
                      </td>
                    </tr>
                    <tr>
                      <td>
                        <p class="name_person">Тян Артур Группа: 117ИС</p>
                        <p class="work_person">Специальность: Информационные системы</p>
                      </td>
                    </tr>
                  </table>
                </div>
              </td>
              <td>
                <div class="student_three_rectangle">
                  <table>
                    <tr>
                      <td>
                        <img class="student_img" src="unnamedthree.png">
                      </td>
                    </tr>
                    <tr>
                      <td>
                        <p class="name_person_three">Зверев Александр Группа: 117ИС</p>
                        <p class="work_person">Специальность: Информационные системы</p>
                      </td>
                    </tr>
                  </table>
                </div>
              </td>
            </tr>
          </table>
        </div>
      </div>
      <div class="all_padding_two">
        <div class="container_two">
          <p class="cont_two_txt">Законы</p>
          <div class="laws">
            <div class="navigation_laws_one">
              <div class="laws_rectangle">
                <ul class="laws_list">
                  <li>
                    <p class="laws_name_txt">Третий закон Ньютона</p>
                  </li>
                  <li>
                    <div class="navigation_btn_laws">
                      <button v-if="LawsNUMone_display == 'none'" @click="ff()">
                        <div class="laws_btn">
                          <img class="arrow_img" src="aaarrow.png">
                        </div>
                      </button>
                      <button v-if="LawsNUMone_display == 'block'" @click="close()">
                        <div style="transform: rotate(180deg) " class="laws_btn">
                          <img class="arrow_img" src="aaarrow.png">
                        </div>
                      </button>
                    </div>
                  </li>
                </ul>
              </div>
              <div :style="{ display: LawsNUMone_display}">
                <div class="navigation_laws_txt_vueblock">
                  <div class="laws_txt_vueblock">
                    <p class="lawstxt">Тела действуют друг на друга с силами равными по модулю и противоположными по направению</p>
                    <p class="lawstxt_two">F₁ = -F₂</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="navigation_laws_two">
              <div class="laws_rectangle">
                <ul class="laws_list">
                  <li>
                    <p class="laws_name_txt">Правило Ленца</p>
                  </li>
                  <li>
                    <div class="navigation_btn_laws">
                      <button v-if="LawsNUMtwo_display == 'none'" @click="cc()">
                        <div class="laws_btn">
                          <img class="arrow_img" src="aaarrow.png">
                        </div>
                      </button>
                      <button v-if="LawsNUMtwo_display == 'block'" @click="close()">
                        <div style="transform: rotate(180deg) " class="laws_btn">
                          <img class="arrow_img" src="aaarrow.png">
                        </div>
                      </button>
                    </div>
                  </li>
                </ul>
              </div>
              <div :style="{ display: LawsNUMtwo_display}">
                <div class="navigation_laws_txt_vueblock">
                  <div class="laws_txt_vueblock">
                    <p class="lawstxt">Индукционный ток направлен так, чтобы своим магнитным полем противодействовать тому изменению магнитного потока,которым он вызван</p>
                  </div>
                </div>
              </div>
            </div>
            <div>
              <div class="laws_rectangle">
                <ul class="laws_list">
                  <li>
                    <p class="laws_name_txt">Магнитная индукция</p>
                  </li>
                  <li>
                    <div class="navigation_btn_laws">
                      <button v-if="LawsNUMthree_display == 'none'" @click="dd()">
                        <div class="laws_btn">
                          <img class="arrow_img" src="aaarrow.png">
                        </div>
                      </button>
                      <button v-if="LawsNUMthree_display == 'block'" @click="close()">
                        <div style="transform: rotate(180deg) " class="laws_btn">
                          <img class="arrow_img" src="aaarrow.png">
                        </div>
                      </button>
                    </div>
                  </li>
                </ul>
              </div>
              <div :style="{ display: LawsNUMthree_display}">
                <div class="navigation_laws_txt_vueblock">
                  <div class="laws_txt_vueblock">
                    <p class="lawstxt">Магнитная индукция - силоавя характеристика магнитного поля</p>
                    <p class="lawstxt_two">B = F/i * l</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="all_padding_two">
        <p class="theory_txt">Теория</p>
        <table>
          <tr class="navigation_theory_two">
            <td class="navigation_theory">
              <button @click="OneTheory()" class="theory_rectangle">
                <p class="theoty_txt_two">Применение и практическое значение закона Джоуля – Ленца</p>
              </button>
            </td>
            <td>
              <button class="theory_rectangle_two">
                <p class="theoty_txt_two">Применение и практическое значение закона Джоуля – Ленца</p>
              </button>
            </td>
          </tr>
          <tr>
            <td class="navigation_theory">
              <button class="theory_rectangle_three">
                <p class="theoty_txt_two">Применение и практическое значение закона Джоуля – Ленца</p>
              </button>
            </td>
            <td>
              <button class="theory_rectangle_four">
                <p class="theoty_txt_two">Применение и практическое значение закона Джоуля – Ленца</p>
              </button>
            </td>
          </tr>
        </table>
      </div>
      <div class="all_padding_two">
        <div class="navigation_laboratory">
          <p class="laboratory_txt">Лабораторные работы</p>
          <div class="navigation_rectangle_laboratory">
            <div @click="Laboratory()">
              <div class="laboratory_rectangle">
                <div class="navigation_all_txt_laboratory_rectangle">
                  <p class="laboratory_name">Изменение ЭДС и внутреннего сопростивления источника тока</p>
                  <p class="laboratory_target_name">
                    <span style="color: #FFF500;">Цель работы:</span> измерить ЭДС и внутреннее сопротивление источника постоянного тока.
                  </p>
                </div>
              </div>   
            </div>
          </div> 
          <div class="laboratory_rectangle">
            <div class="navigation_all_txt_laboratory_rectangle">
              <p class="laboratory_name">Изучение устройства и работы трансформатора</p>
              <p class="laboratory_target_name">
                <span style="color: #FFF500;">Цель работы:</span> измерить ЭДС и внутреннее сопротивление источника постоянного тока.
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="navigation_footer">
        <div class="footer_rectangle">
          <ul class="footer_list">
            <li>
              <p class="footer_txt">Саакян Михаил:<a href="https://vk.com/nlemsaakyan"><span style="color: #2D9AFF;"> https://vk.com/nlemsaakyan</span></a></p>
              <div class="nav_txt_footer">
                <p class="footer_txt">Тян Артур:<a href="https://vk.com/furidashi1"><span style="color: #2D9AFF;"> https://vk.com/furidashi1</span></a></p>
              </div>
              <p class="footer_txt">Зверев Александр:<a href="https://vk.com/s.zv2357"><span style="color: #2D9AFF;"> https://vk.com/s.zv2357</span></a></p>
            </li>
            <li class="navigation_github">
              <div>
                <a href="https://github.com/Exportqq">
                  <img class="github" src="github.svg">
                </a>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div :style="{ display: OneTheoryDisplay}">
      <div class="all_padding">
        <div class="all_theory_navigation">
          <ul class="laws_list">
            <li>
              <div>
                <button @click="NoTheory()">
                  <img class="all_theory_img" src="theotybtnimg.svg">
                </button>
              </div>
            </li>
            <li>
              <div>
                <p class="new_theory_txt">Применение и практическое значение закона Джоуля – Ленца</p>
              </div>
            </li>
          </ul>
        </div>
        <div>
          <p class="all_theory_txt">На примере многих бытовых приборов понятно, что если через участок цепи проходит электроток и при этом не совершается какая-либо работа, то происходит нагревание проводника. Иногда оно идет на пользу — например, в лампе накаливания или в аппарате дуговой сварки. Но в других случаях тепловой эффект нежелателен — например, перегрев электрической проводки в здании может вызвать пожар. Поэтому в наших интересах управлять таким эффектом, и правило Джоуля-Ленца определяет, от чего зависит тепловое действие тока. <br><br>Правило было сформулировано в результате опытов двух ученых — англичанина Джеймса Прескотта Джоуля и российского физика Эмилия Христиановича Ленца. Поскольку ученые работали независимо друг от друга, новый закон назвали двойным именем. <br><br>Применение на практике закона Джоуля-Ленца заключается в том, что тепловым действием электрического тока можно управлять, подбирая проводники с нужным сопротивлением. К примеру, для электрических нагревательных приборов, которые должны выделять максимум тепла, выбирают проводники с высоким сопротивлением. <br><br>Низкое сопротивление, напротив, позволяет проводнику практически не нагреваться при прохождении тока. Поэтому на промышленных предприятиях с усиленными требованиями к пожаробезопасности для прокладки линий электропередач используется медный кабель. Удельное сопротивление меди сечением 1 мм2 равно 0,0175 Ом, в то время как у алюминия оно составляет 0,0271 Ом. Медь практически не нагревается, чем снижает риск возгораний.</p>
        </div>
      </div>
    </div>
    <div :style="{ display: LabOne}">
      <div class="all_padding">
        <div class="all_theory_navigation">
          <div style="float: left;">
            <button @click="NoTheory()">
              <img class="all_theory_img" src="theotybtnimg.svg">
            </button>
          </div>
          <div style="float: left;">
            <p class="new_theory_txt">Изменение ЭДС и внутреннего сопростивления источника тока</p>
          </div>
        </div>
        <div>
          <ul class="laws_list">
            <li>
              <div class="reostat">
                <div class="polznav">
                  <div class="slidecontainer">
                    <input type="range" step="10" class="slider" v-model="myRange">
                    <p class="vallue_txt" id="demo"></p>
                    <p style="display: block;" id="val1">50</p>
                  </div>
                </div>
              </div>
            </li>
            <li>
              <p>{{ myRange }}</p>
              <p>{{ I }}</p>
              <p>{{ U }}</p>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      AllPageDisplay: "block",
      OneTheoryDisplay: "none",
      LabOne: "none",
      LawsNUMone_display: "none",
      LawsNUMtwo_display: "none",
      LawsNUMthree_display: "none",
      myRange: "",
      S: 0.5,
      p: 0.017,
      l: 10,
      E: 12,
      r: 0.20,
      R: 0,
      I: 0,
      U: 0,
    }
  },

  watch: {
    myRange(new_myRange) {
      if (new_myRange > -1) {
        this.R = this.p * this.myRange / this.S;
        this.I = this.E / (this.r + this.R);
        this.I = this.I.toFixed(2)
        this.U = this.I / this.R;
        this.U = this.U.toFixed(2)
      }
    }
  },
  methods: {
    ff() {
      this.LawsNUMone_display = "block"
      this.LawsNUMtwo_display = "none"
      this.LawsNUMthree_display = "none"
    },
    cc() {
      this.LawsNUMone_display = "none"
      this.LawsNUMtwo_display = "block"
      this.LawsNUMthree_display = "none"
    },
    dd() {
      this.LawsNUMthree_display = "block"
      this.LawsNUMone_display = "none"
      this.LawsNUMtwo_display = "none"
    },
    close() {
      this.LawsNUMthree_display = "none"
      this.LawsNUMone_display = "none"
      this.LawsNUMtwo_display = "none"
    },
    OneTheory() {
      this.OneTheoryDisplay = "block"
      this.AllPageDisplay = "none"
    },
    NoTheory() {
      this.OneTheoryDisplay = "none"
      this.AllPageDisplay = "block"
    },
    Laboratory() {
      this.LabOne = "block"
      this.AllPageDisplay = "none"
    }

  }
}
</script>

<style>
* {
  margin: 0px;
  padding: 0px;
}

.all_padding {
  padding: 0px 0px 0px 450px;
}

.all_padding_two {
  padding: 0px 0px 0px 450px;
}

.backround-app-site {
  background-image: url(static/backroundfizhub.png);
  width: 1920px;
  height: 883px;
}

.list_header li {
  float: left;
}

.list_header {
  height: 83px;
}

ul li {
  list-style: none;
}

.logo {
  padding: 0px 273px 0px 0px;
}

.list li {
  float: left;
}

.header-txt {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 29px;
  color: #FFFFFF;
  padding: 25px 70px 0px 0px;
}

.header_txt_two {
  font-family: 'Montserrat';
  width: 653px;
  height: 234px;
  font-style: normal;
  font-weight: 700;
  font-size: 64px;
  line-height: 78px;
  color: #FFFFFF;
  padding: 143px 0px 0px 0px;
}

.header-txt-on {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 29px;
  color: #FFFFFF;
  padding: 25px 70px 0px 0px;
}

.animation_navigation {
  padding: 0px 200px 0px 0px;
}

.animation_cube {
  border-radius: 500px;
  padding: 28px 0px 0px 0px;
}

.header_navigation {
  padding: 45px 0px 0px 0px;
}

/**/ 

.cont_txt {
  height: 230px;
  width: 795px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 48px;
  line-height: 59px;
  color: #3F49A3;
  padding: 97px 0px 0px 226px;
}

.student_one_rectangle {
  width: 310px;
  height: 500px;
  background: linear-gradient(21.44deg, #333399 0%, #0D92CB 98.49%);
  border-radius: 20px;
}

.student_two_rectangle {
  width: 310px;
  height: 500px;
  background: linear-gradient(21.44deg, #E98F0A 0%, #A44153 98.49%);  
  border-radius: 20px;
}

.student_three_rectangle {
  width: 310px;
  height: 500px;
  background: linear-gradient(21.44deg, #8F00FF 0%, #0500FF 98.49%);
  border-radius: 20px;
}

.navigation_person_rectangle {
  padding: 0px 45px 0px 45px;
}

.name_person {
  width: 256px;
  height: 58px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 29px;
  text-align: center;
  color: #FFFFFF;
  padding: 16px 0px 0px 54px;
}

.work_person {
  width: 277px;
  height: 87px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 29px;
  text-align: center;
  color: #FFFFFF;
  padding: 35px 0px 0px 34px;
}

.name_person_three {
  width: 277px;
  height: 58px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 29px;
  text-align: center;
  color: #FFFFFF;
  padding: 16px 0px 0px 32px;
}

.student_img {
  width: 245px;
  height: 245px;
  padding: 65px 0px 0px 65px;
}

/**/

.cont_two_txt {
  width: 197px;
  height: 209px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 48px;
  line-height: 59px;
  color: #3F49A3;
  padding: 150px 0px 0px 411px;
}

.laws_rectangle {
  width: 1020px;
  height: 96px;
  background: #393939;
  border-radius: 15px;
}

.laws_list li {
  float: left;
}

.laws_name_txt {
  width: 925px;
  height: 39px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 32px;
  line-height: 39px;
  color: #FFFFFF;
  padding: 28px 0px 0px 45px;
}

.laws_btn {
  width: 50px;
  height: 50px;
  background: #FFFFFF;
  border-radius: 10px;
}

.navigation_btn_laws {
  padding: 23px 0px 0px 0px;
}

.navigation_laws_one {
  padding: 70px 0px 0px 0px;
}

.navigation_laws_two {
  padding: 37px 0px 37px 0px;
}

/**/

.arrow_img {
  padding: 14px 0px 0px 0px;
}

.theory_txt {
  width: 188px;
  height: 59px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 48px;
  line-height: 59px;
  color: #3F49A3;
  padding: 150px 0px 95px 416px;
}

.theory_rectangle {
  background-image: url(static/Rectangle8.png);
  width: 485px;
  height: 161px;
}

.theory_rectangle_two {
  background-image: url(static/Rectangle.png);
  width: 500px;
  height: 161px;
}

.theory_rectangle_three {
  background-image: url(static/Rectangle10.png);
  width: 485px;
  height: 161px;
}

.theory_rectangle_four {
  background-image: url(static/Rectangle11.png);
  width: 500px;
  height: 161px;
}

.navigation_theory {
  padding: 0px 35px 0px 0px;
}

.navigation_theory_two {
  height: 231px;
}

.theoty_txt_two {
  width: 461px;
  height: 58px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 29px;
  text-align: center;
  vertical-align: middle;
  color: #393939;
  padding: 0px 0px 0px 23px;
}

/**/

.laboratory_rectangle {
  width: 1020px;
  height: 267px;
  background: #393939;
  border-radius: 20px;
}

.laboratory_txt {
  width: 807px;
  height: 59px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 48px;
  line-height: 59px;
  color: #3F49A3;
  padding: 0px 0px 0px 214px;
}

.navigation_laboratory {
  padding: 150px 0px 0px 0px;
}

.laboratory_name {
  height: 88px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 36px;
  line-height: 44px;
  color: #FFFFFF;
}

.laboratory_target_name {
  width: 861px;
  height: 88px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 36px;
  line-height: 44px;
  color: #FFFFFF;
  padding: 22px 0px 0px 0px;
}

.navigation_all_txt_laboratory_rectangle {
  padding: 35px 0px 0px 35px;
}

.navigation_rectangle_laboratory {
  padding: 70px 0px 40px 0px;
}

/**/

.footer_rectangle {
  width: 1920px;
  height: 394px;
  background: #393939;
}

.navigation_footer {
  padding: 165px 0px 0px 0px;
}


.footer_list li{
  float: left;
}

.footer_txt {
  height: 44px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 36px;
  line-height: 44px;
  color: #8C8C8C;
}

a {
  text-decoration: none;
}

.navigation_github{
  padding: 0px 0px 0px 121px;
}

.footer_list {
  padding: 116px 0px 0px 450px;
}

/**/

.laws_txt_vueblock {
  width: 868px;
  height: 365px;
  background: #FFFFFF;
  border-width: 0px 5px 5px 5px;
  border-style: solid;
  border-color: #393939;
  border-radius: 0px 0px 12px 12px;
}

.navigation_laws_txt_vueblock {
  padding: 0px 0px 0px 76px;
}

.lawstxt {
  width: 821px;
  height: 237px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 32px;
  line-height: 39px;
  text-align: center;
  color: #3F49A3;
  padding: 85px 0px 0px 47px;
}

.lawstxt_two {
  width: 868px;
  height: 78px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 64px;
  line-height: 78px;
  text-align: center;
  color: #A33F8D;
}

/**/

.new_theory_txt {
  width: 920px;
  height: 100px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 40px;
  line-height: 49px;
  text-align: center;
  color: #393939;
}

.all_theory_txt {
  width: 1062px;
  height: 1029px;
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 40px;
  line-height: 49px;
  letter-spacing: -0.03em;
  color: #393939;
}

.all_theory_navigation {
  width: 1020px;
  padding: 65px 0px 200px 0px;
}

.slidecontainer {
    width: 100%; 
}


.slider {
    -webkit-appearance: none;  
    appearance: none;
    width: 480px;
    height: 6px; 
    outline: none; 
    opacity: 0.7; 
    -webkit-transition: .2s; 
    transition: opacity .2s;
}

.slider:hover {
    opacity: 1; 
}

.slider::-webkit-slider-thumb {
    -webkit-appearance: none; 
    appearance: none;
    border-radius: 12px;
    width: 30px; 
    height: 50px; 
    background: #3F49A3; 
    cursor: pointer; 
}

.slider::-moz-range-thumb {
    background: #3F49A3; 
    cursor: pointer; 
}

.reostat {
  background-image: url(static/reostat.png);
  width: 523px;
  height: 252px;
}

.polznav {
  padding: 10px 0px 0px 23px;
}
@media (min-width: 300px) and (max-width: 320px) {
  * {
    margin: 0px;
    padding: 0px;
  }

  .all_padding {
    padding: 0px 0px 0px 15px;
  }

  .all_padding_two {
    padding: 0px 0px 0px 20px;
  }

  .backround-app-site {
    background-image: url(static/AdobeStock_4373633.png);
    width: 320px;
    height: 150px;
  }

  .list_header li {
    float: left;
  }

  .header_navigation {
    padding: 2px 0px 0px 23px;
  }

  ul li {
    list-style: none;
  }

  .list_header {
    height: 25px;
  }

  .logo {
    width: 70px;
    height: 20px;
    padding: 5px 40px 0px 0px;
  }

  .list li {
    float: left;
  }

  .header-txt {
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 6px;
    line-height: 7px;
    color: #FFFFFF;
    padding: 0px 15px 0px 0px;
  }

  .header_txt_two {
    width: 123px;
    height: 39px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 11px;
    line-height: 13px;
    color: #FFFFFF;
    padding: 24px 0px 0px 0px;
  }

  .header-txt-on {
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 6px;
    line-height: 7px;
    color: #FFFFFF;
    padding: 0px 15px 0px 0px;
  }

  .animation_navigation {
    padding: 0px 54px 0px 0px;
  }

  .animation_cube {
    border-radius: 500px;
    padding: 0px 0px 0px 0px;
    width: 100px;
    height: 100px;
  }

  /**/

  .cont_txt {
    width: 210px;
    height: 50px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 11px;
    line-height: 13px;
    color: #3F49A3;
    padding: 22px 0px 0px 80px;
  }

  .student_one_rectangle {
    width: 90px;
    height: 178px;
    background: linear-gradient(21.44deg, #333399 0%, #0D92CB 98.49%);
    border-radius: 10px;
  }

  .student_two_rectangle {
    width: 90px;
    height: 178px;
    background: linear-gradient(21.44deg, #E98F0A 0%, #A44153 98.49%);  
    border-radius: 10px;
  }

  .student_three_rectangle {
    width: 90px;
    height: 178px;
    background: linear-gradient(21.44deg, #8F00FF 0%, #0500FF 98.49%);
    border-radius: 10px;
  }

  .navigation_person_rectangle {
    padding: 0px 10px 0px 10px;
  }

  .name_person {
    width: 79px;
    height: 29px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 8px;
    line-height: 10px;
    text-align: center;
    color: #FFFFFF;
    padding: 9px 0px 0px 7px;
  }

  .work_person {
    width: 81px;
    height: 30px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 8px;
    line-height: 10px;
    text-align: center;
    color: #FFFFFF;
    padding: 11px 0px 0px 4px;
  }

  .name_person_three {
    width: 86px;
    height: 29px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 8px;
    line-height: 10px;
    text-align: center;
    color: #FFFFFF;
    padding: 9px 0px 0px 1px;
  }

  .student_img {
    width: 80px;
    height: 89px;
    padding: 19px 0px 0px 10px;
  }

  .cont_two_txt {
    width: 46px;
    height: 13px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 11px;
    line-height: 13px;
    color: #3F49A3;
    padding: 25px 0px 15px 117px;
  }

  .laws_rectangle {
    width: 280px;
    height: 30px;
    background: #393939;
    border-radius: 5px;
  }

  .laws_list li {
    float: left;
  }

  .laws_name_txt {
    width: 250px;
    height: 12px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 10px;
    line-height: 12px;
    color: #FFFFFF;
    padding: 9px 0px 0px 15px;
  }

  .arrow_img {
    width: 12px;
    height: 9px;
    padding: 0px 2px 3px 1px;
  }

  .laws_btn {
    width: 15px;
    height: 15px;
    background: #FFFFFF;
    border-radius: 2px;
  }

  .navigation_btn_laws {
    padding: 7px 0px 0px 0px;
  }

  .navigation_laws_one {
    padding: 15px 0px 0px 0px;
  }

  .navigation_laws_two {
    padding: 10px 0px 10px 0px;
  }

  .theory_txt {
    width: 44px;
    height: 13px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 11px;
    line-height: 13px;
    color: #3F49A3;
    padding: 25px 0px 15px 117px;
  }

  .theory_rectangle {
    background-image: url(static/Rectangle153.png);
    width: 135px;
    height: 64px;
  }

  .theory_rectangle_two {
    background-image: url(static/Rectangle152.png);
    width: 135px;
    height: 64px;
  }

  .theory_rectangle_three {
    background-image: url(static/Rectangle151.png);
    width: 135px;
    height: 64px;
  }

  .theory_rectangle_four {
    background-image: url(static/Rectangle15.png);
    width: 135px;
    height: 64px;
  }

  .navigation_theory {
    padding: 0px 10px 0px 0px;
  }

  .navigation_theory_two {
    height: 85px;
  }

  .theoty_txt_two {
    width: 114px;
    height: 49px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 10px;
    line-height: 12px;
    text-align: center;
    color: #393939;
    padding: 0px 0px 0px 21px;
  }

  .laboratory_rectangle {
    width: 280px;
    height: 88px;
    background: #393939;
    border-radius: 8px;
  }

  .laboratory_txt {
    width: 208px;
    height: 13px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 11px;
    line-height: 13px;
    color: #3F49A3;
    padding: 0px 0px 0px 72px;
  }

  .navigation_laboratory {
    padding: 25px 0px 0px 0px;
  }

  .laboratory_name {
    height: 24px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 10px;
    line-height: 12px;
    color: #FFFFFF;
  }

  .laboratory_target_name {
    width: 239px;
    height: 24px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 10px;
    line-height: 12px;
    padding: 10px 0px 0px 0px;
  }

  .navigation_all_txt_laboratory_rectangle {
    padding: 8px 0px 0px 8px;
  }

  .navigation_rectangle_laboratory {
    padding: 16px 0px 10px 0px;
  }

  .footer_rectangle {
    width: 100%;
    height: 86px;
    background: #393939;
  }

  .navigation_footer {
    padding: 25px 0px 0px 0px;
  }


  .footer_list li{
    float: left;
  }

  .footer_txt {
    width: 184px;
    height: 10px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 8px;
    line-height: 10px;
    color: #8C8C8C;
  }

  a {
    text-decoration: none;
  }

  .navigation_github{
    padding: 0px 0px 0px 76px;
  }

  .footer_list {
    padding: 22px 0px 0px 20px;
  }

  .github {
    width: 20px;
    height: 20px;
  }

  .nav_txt_footer {
    padding: 5px 0px 5px 0px;
  }

  .laws_txt_vueblock {
    width: 256px;
    height: 94px;
    background: #FFFFFF;
    border-width: 0px 2px 2px 2px;
    border-style: solid;
    border-color: #393939;
    border-radius: 0px 0px 5px 5px;
  }

  .navigation_laws_txt_vueblock {
    padding: 0px 0px 0px 12px;
  }

  .lawstxt {
    width: 216px;
    height: 57px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 9px;
    line-height: 11px;
    text-align: center;
    color: #3F49A3;
    padding: 14px 0px 0px 20px;
  }

  .lawstxt_two {
    width: 256px;
    height: 78px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 20px;
    line-height: 24px;
    text-align: center;
    color: #A33F8D;
  }

  .new_theory_txt {
    width: 260px;
    height: 30px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 10px;
    line-height: 12px;
    text-align: center;
    color: #393939;
  }

  .all_theory_txt {
    width: 290px;
    height: 204px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 10px;
    line-height: 12px;
    letter-spacing: -0.03em;
    color: #393939;
  }

  .all_theory_navigation {
    width: 300px;
    padding: 25px 0px 50px 0px;
  } 

  .all_theory_img {
    width: 30px;
    height: 30px;
  }
}














































</style>