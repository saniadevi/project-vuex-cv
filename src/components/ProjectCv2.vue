<template>
<div class="all">
<div class="one">
    <img  src="https://4.bp.blogspot.com/-FOZ-RymNN8c/UQKamE83EGI/AAAAAAAARkk/zhuVK94iW1k/s1600/Lonely+Tree+Paography+Wallpapers+07.jpg" height="135px" width="255px ">
    <h2 style="border-top: 2px dashed black;">PROFILE</h2>
    <p v-for="wk in dataList" :key="wk"><b>NAME</b><br>{{wk.nama}}</p>
    <p v-for="wk in dataList" :key="wk"><b>DATE OF BIRTH</b><br>{{wk.date }}</p>
    <p v-for="wk in dataList" :key="wk"><b>ADDRESS</b><br>{{wk.adres}}</p>
    <p v-for="wk in dataList" :key="wk"><b>WEBSITE</b><br>{{wk.website}}</p><br>
    <h2 style="border-top: 2px dashed black;">AWARDS</h2>
    <p v-for="wk in dataList" :key="wk"><b>CHARTER AWARD 2012 </b><br> {{wk.charter}}</p>
    <p v-for="wk in dataList" :key="wk"><b>INTERFACE DESIGN 2013 </b><br> {{wk.inter}}</p><br>
<h2 style="border-top: 2px dashed black;">CONTACT</h2>
    <p v-for="wk in dataList" :key="wk"><b>HOME NUMBER&#x260E;&#xFE0F; </b><br> {{wk.home}}</p>
    <p v-for="wk in dataList" :key="wk"><b>PHONE NUMBER&#x1F4DE; </b><br>{{wk.phone}}</p>
    <p v-for="wk in dataList" :key="wk"><b>EMAIL&#x1F4E7; </b><br> {{wk.email}}</p><br>
    <div>
<h2 style="border-top: 2px dashed black;">SOCIAL</h2>
    <p><b>TWITTER</b><br>@Azafnia</p>
    <p><b>FACEBOOOK </b><br>Azafnia</p>

 
     </div>
     </div>
     <div class="two">
     <h1  v-for="wk in dataList" :key="wk">{{wk.nma0}}<br>{{wk.nma1}}</h1><br>
     <h2>BOOTCAMP PARTICIPANTS</h2><hr>
     <div class="satu">
        <h2 style="border-bottom: 2px dashed black;">WORK EXPERIENCE</h2>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.creat0}}</b><br>{{wk.creat1}}</p>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.creat2}}</b><br>{{wk.creat3}}</p>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.creat4}}</b><br>{{wk.creat5}}</p>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.senior0}}</b><br>{{wk.senior1}}</p>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.senior2}}</b><br>{{wk.senior3}}</p>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.senior4}}</b><br>{{wk.senior5}}</p>
 </div>
 <br>
        <div class="dua">
        <h2 style="border-top: 2px dashed black;">EDUCATION</h2>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.educa0}}</b><br>{{wk.educa1}}</p>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.educa0}}</b><br>{{wk.educa1}}</p>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.educa0}}</b><br>{{wk.educa1}}</p>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.educa2}}</b><br>{{wk.educa3}}</p>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.educa2}}</b><br>{{wk.educa3}}</p>
        <p  v-for="wk in dataList" :key="wk"><b>{{wk.educa2}}</b><br>{{wk.educa3}}</p>
</div>
     </div>   
</div>
</template>
<script>
export default { 
        name: 'ProjectCv2', 
        computed: { 
            dataList() { 
                return this.$store.state.data
            } 
        } 
    } 
</script>
<style scoped> 
 all{ 
    padding: 20px; 
    margin-left: 40px; 
} 
 
.one { 
    border: 1px solid lightgrey; 
    padding: 20px; 
    width: 300px; 
    background-color: lightgrey; 
    float: left; 
    margin-bottom: 30px;
    height: 1200px;
    text-align: right;
} 
 
.two { 
    border: 1px solid white; 
    padding: 20px; 
    background-color: white; 
    float: left; 
    width: 60%; 
    height: 1000px; 
     margin-bottom: 30px;
} 
 
.satu{ 
  background-color: darkgrey; 
  padding: 20px; 
  height: auto                                         ; 
} 
.dua {
    background-color: darkgrey; 
  padding: 20px; 
  height: 420px;      
  margin-bottom: 30px;
}
h1 {
    border: 1px solid black;
    background-color: navy;
    color: white;
}
 
</style>