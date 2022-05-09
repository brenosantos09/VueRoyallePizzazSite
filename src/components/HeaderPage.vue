<template>
    <header class="bg-red">
        <div class="logo">
           <img src="@/assets/img/logo.png" alt="">
           <p><span>R</span>oyalle Pizzaz</p>
        </div>
      
    </header>
</template>

<script>
export default {
  name: "HeaderPage",
};
</script>

<style scoped>
     header{
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center; 
}
.logo img{
    width: 150px;
}
.material-icons {
    text-decoration: none;
    color: #FFFFFF;
    font-size: 45px;
    transition: transform 0.3s;
}
header span{
    color: rgb(7, 7, 7);
}
.material-icons:hover{
    color: rgb(2, 2, 2);
     transform: scale(1.5);
}
.logo{
    display: flex;
    align-items: center;
    padding-left: 15px;
    padding-top: 10px;
}
.logo p{
    font-size: 25px;
    padding-left: 10px;
    color: #FFFFFF;
}
.card-body span{
    color: rgb(13, 14, 13);
}
.navbar{
    padding: 15px 0;
}
.nav-item{
    margin-left: 10px;
    
}
</style>