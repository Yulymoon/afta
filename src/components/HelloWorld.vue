<template>
  <div class="container">
    <div class="head">
      <div class="navbar">
        <div class="left logo">
          <img src="../assets/AFTA-LOGO.jpg" alt="">
          <span>AFTA TECHNOLOGY CO., LTD.</span>
        </div>
        <div class="right">
          <ul>
            <li><a href="#">Home</a></li>
            <li>About us</li>
            <li>News</li>
            <li class="toggle">Products</a>
              <ul class="toggleab">
                <li><a href="http://www.pullman-motor.com/">Tricycle</a></li>
                <li><a href="http://www.qqhometech.com/">QQHome</a></li>
                <li>Police</li>
                <li>Machine</li>
              </ul>
            </li>
            <li>Contact us</li>
            <li></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="home">
      <img src="../assets/PRODUCT.gif"  alt="">
    </div>
    <div class="aboutus">
      <h1>About us</h1>
      <div class="content">
        <div class="left">
          <iframe width="560" height="315" src="https://www.youtube.com/embed/j-4SvajCRLw" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>
        </div>
        <div class="right">
          AFTA Technology Co., Ltd., has more than 30 years of professional plastic technology  and plenty of marketing experiences with more than 80 countries, so that can meet the  needs for the customers about the equipments and coordinate with the perfect Global  sales and service networks. Meanwhile, its the greatest honor that the Managing  Director of AFTA, Susan Wang, has met with the Vice President of Taiwan and the King  of Swaziland for several times. Moreover, in October 2010, AFTA behalf on Taiwan   Machinery Industry to present a speech Taiwan Machinery Industry Development in   Germany, and won a wonderful response. We hope to establish the long-term  partnership relations with the friends of emerging countries and stand in India for our  global marketing service center and provide Beverage, Food processing and Solar  Energy completed Turnkey Solution equipment and service.
        </div>
      </div>
    </div>
    <div class="news">
      <h1>News</h1>
      <div class="content" v-for="n in news">
        <div class="title">
          <a href="#">{{n.title}}</a>
        </div>
        <div class="date">
          {{n.date}}
        </div>
        <div class="location">
          {{n.location}}
        </div>
      </div>
    </div>
    <div class="product">

    </div>
    <div class="contactus">
      <div class="">
        <h1>CONTACT</h1>
      　<div>AFTA TECHNOLOGY CO., LTD.</div>
        <div>5F, NO. 354 , SECT. 1, DONGMEN ROAD, TAIANAN, TAIWAN</div>
      　	<div>TEL: + 886-6-2094858  FAX: + 886-6-2098977</div>
      　	<div>EMAIL: service@afta.com.tw</div>
        <div class="">
          <iframe width='100%' height='500' frameborder='0' scrolling='no' marginheight='0' marginwidth='0' src='http://maps.google.com.tw/maps?f=q&hl=zh-TW&geocode=&q=701東區東門路一段354號&z=16&output=embed&t='></iframe>
        </div>
      <icon name="beer"></icon>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      news:[{
        	title:'2016 INVENT ARENA',
          date:'2016/6/18',
          location:'TRINEC, CZECK'
      },
    {
      title:'2016 GLOBAL SUMMIT OF WOMEN',
      date:'2016/6/09',
      location:'WARSAW, POLAND'
    }]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">

.cursor-pointer{
  cursor: pointer;
}

.home{
  margin:5%;
}
h1, h2 {
  font-weight: normal;
  color:#a6a6a6;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
  cursor: pointer;
}
a {
  color:#2c3e50;
  text-decoration:none;
}

.navbar{
  display:flex;
  justify-content: space-between;
  align-items: center;
  .left{

  }
}

.news{
  padding:5%;
  .content{
    display:flex;
    .title{
      flex:2;
      text-align: left;
    }
    .date,.location{
      flex:1;
    }
  }
}

.aboutus{
  background-color: #222;
  color:#fff;
  padding:5%;
  .content{
    display:flex;
  }
  .left,.right{
    flex:1;
  }
  .right{
    display:flex;
    align-items: center;
  }
}
.contactus{
  background-color: #222;
  color:#fff;
  padding:5%;
}
.toggle{
  position: relative;
  .toggleab{
    display:none;
    position: absolute;
  }
}
.toggle:hover{
  .toggleab{
    display:block;
    text-align: left
  }
}
</style>
