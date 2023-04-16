<template>
  <div class="wrapper">
    <div class="main_content">

      <div class="header">
        <h2 class="logo">
          <img src="../assets/logo_1.png" alt="" width="60" height="60" />
        </h2>
      </div>
      <div class="info" id="info-home">
        <p class="name-home" style="font-size: 80px; color: antiquewhite;">ET ENERGY</p>
        <p class="desc" style="font-size: 20px; color: darkgrey;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; . . . ในปัจจุบัน
          ชีวิตประจำวันของเราคงหนีไม่พ้นการใช้ไฟฟ้าไม่ว่าจะเป็นการเปิดไฟ เปิดพัดลม
          หรือว่าในตอนที่เราใช้โทรศัพท์มือถือ เราก็ต้องชาร์จแบตเมื่อแบตหมด
          ดังนั้นไฟฟ้าถือเป็นสิ่งหนึ่งที่สำคัญกับเราในชีวิตประจำวันมาก
          และพวกคุณรู้กันหรือไม่ว่าไฟฟ้าที่เราใช้กันมีราคาเท่าไรกันบ้าง ET ENERGY ของเราจะคำนวนให้พวกคุณเอง . . .</p>
      </div>
      <div class="columns">
        <div class="column is-2 is-offset-2">
          <div class="box has-text-centered" id="box-1">
            <div class="pic-bl">
              <router-link to="/calelectic">
                <img src="../assets/elelctic.png" alt="" width="50" height="50" /><br />
              </router-link>
            </div>
            <p style="font-weight: bold; padding-bottom: 5px; padding-top: 15px;">Calculator Electic Cost</p>
            <p>อยากคำนวนค่าไฟใช่ไหม ลองคลิ๊กที่รูปสายฟ้าแล้วไปคำนวนกันเลย</p>
          </div>
        </div>
        <div class="column is-2">
          <div class="box has-text-centered" id="box-1">
            <div class="pic-bl">
              <router-link to="/calair">
                <img src="../assets/air.png" alt="" width="50" height="50" /><br />
              </router-link>
            </div>
            <p style="font-weight: bold; padding-bottom: 5px; padding-top: 15px;">Calculator Air Cost</p>
            <p>มาลองคำนวนค่าแอร์กัน ลองคลิ๊กที่รูปแอร์แล้วไปคำนวนกันเลย</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {},
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Chakra+Petch&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  list-style: none;
  text-decoration: none;
  font-family: 'Chakra Petch', sans-serif;
}

body {
  background-image: linear-gradient(to bottom,
      rgba(18, 18, 17, 0.5),
      rgba(220, 228, 199, 0.5)), url("../assets/bg_1.jpg");
  height: 100%;
  width: 100%;
  background-size: cover;
  position: fixed;
}

.logo {
  color: #fff;
  text-align: center;
  cursor: pointer;
  padding-top: 15px;
  transition: rotate 1s;
}

.logo:hover {
  rotate: 180deg;
}

.main_content {
  width: 100%;
}

#info-home {
  margin-top: 5%;
  margin-left: 10%;
}

.name-home {
  font-size: 40px;
  color: rgb(255, 255, 255);
  font-weight: bold;
}

.desc {
  color: #000;
  width: 50%;
}

#box-1 {
  margin: 5%;
  margin-top: 30%;
  background-color: rgba(244, 245, 216, 0.896);
  border: 5px solid rgba(208, 218, 145, 0.744);
  margin-bottom: 100px;
}

.pic-bl {
  transform: scale(1);
  transition: transform 1s;
  /* text-align: center; */
  opacity: 0.6;
}

.pic-bl:hover {
  transform: scale(1.1);
  opacity: 0.7;
}
</style>

