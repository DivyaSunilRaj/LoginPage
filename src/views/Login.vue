
<template>
    <div id="background">
      <div id="logo">DecideWhatToEat</div>
      <div id="TopLink">
      <el-link href="https://element.eleme.io" target="_blank">About</el-link> | 
         <el-link href="https://element.eleme.io" target="_blank">Contact us</el-link>
      </div>
      <div id="login">
      <el-card class="box-card">
        <div id="form">
        <el-input v-model="username" placeholder="Please enter your username"></el-input>
        <el-input placeholder="Please enter your password" v-model="password" show-password></el-input>
          <el-button type="warning">Log in</el-button>
          <br>
          <el-link type="primary">Not registered? Creare a new account</el-link>
        </div>
</el-card>
      </div>
    </div>
</template>
<style scoped>

#background{
    
    position:fixed;
    height:100%;
    width:100%;
    top:0;
    left:0;
    background-image:linear-gradient(
        90deg,
        #feae8b,
        #f7e4ce
    );
    background-size:400%;
    animation:myanimation 10s infinite;
}
@keyframes myanimation{
0%{
    background-position:0% 50%;
}
50%{
    background-position:100% 50%;
}
100%{
    background-position:0% 50%;
}
}
#logo{
color:#00552e;
font-size: 35px;
font-weight: 800;
position:absolute;
top:15%;
left:15%;
}
#login{
    position:absolute;
    top:30%;
    left:38%
}
#TopLink{
   
}
.el-card{
    width:373px;
    height:250px;
    background-color:rgba(255,255,2555,0.4);
    border-radius:15px;
}
#form{
    line-height:60px;
    padding-left:15px;
    padding-right:15px;
}
</style>
<script>
export default{
   data(){
    return{
        username:"",
        password:"",
    }
   }
}
</script>