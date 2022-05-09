<template>
  <main id="home">
    <div class="btnVoltar">
      <a href="#home"><i class="bi bi-arrow-up-circle"></i></a>
    </div>

    <HeaderPage />
    <NavbarPage />

 <!-- seção banner -->
    <section id="propaganda1" class="container-fluid bg-black p-0">
      <div
        id="carouselExampleControls"
        class="carousel slide"
        data-bs-ride="carousel"
      >
        <div class="carousel-inner">
          <div class="carousel-item active imgBG1">
            <!-- <img src="img/produtos/p1.jpg" class="d-block w-100" alt="..."> -->
          </div>
          <div class="carousel-item imgBG2">
            <!-- <img src="img/produtos/produto02.jpg" class="d-block w-100" alt="..."> -->
          </div>
          <div class="carousel-item imgBG3">
            <!-- <img src="img/produtos/p3.jpg" class="d-block w-100" alt="..."> -->
          </div>
        </div>
        <button
          class="carousel-control-prev"
          type="button"
          data-bs-target="#carouselExampleControls"
          data-bs-slide="prev"
        >
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button
          class="carousel-control-next"
          type="button"
          data-bs-target="#carouselExampleControls"
          data-bs-slide="next"
        >
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
    </section>
  <!-- fim seção banner -->

    <!--área propaganda-->
    <section id="propaganda" class="bg-yellow p-4">
        <h1 class="menu-propaganda text-center">Ofertas Especiais</h1>
        <div class="container">
          <div class="row">  
            <div class="col-md-4 col-12">
                <img src="@/assets/img/pizza1.jpg" alt="" class="img-fluid rounded-circle imagem-propaganda">
                <p class="menu-propaganda text-center p-4 fs-3">Sabor Calabresa</p>
            </div>
            <div class="col-md-4 col-12">
                <img src="@/assets/img/pizza2.jpg" alt="" class="img-fluid rounded-circle imagem-propaganda">
                <p class="menu-propaganda text-center p-4 fs-3">Pizza Vegana</p>
            </div>
            <div class="col-md-4 col-12">
                <img src="@/assets/img/pizza3.jpg" alt="" class="img-fluid rounded-circle imagem-propaganda">
                <p class="menu-propaganda text-center p-4 fs-3">Pizza Portuguesa</p>
            </div>
          </div>
        </div>
           
    </section>
    <!--fim área propaganda--> 

    <!--área cardápio-->
    <section id="cardapio" class="container bg-red">
        <h2 class="text-center menu-text p-5 fs-1">Nosso Cardápio</h2>
        <div class="row">
            <div class="col-md-2 col-12 p-2 mx-3 mt-4">
                <img src="@/assets/img/imagem1.png" alt="" class="card-img-top img-fluid">
                    <h5 class="menu-text text-center py-3">Título</h5>
                    <p class="menu-text text-center fs-6">Lorem Ipsum is simply dummy text of the printing and typesetting industry. </p>
                    <span class="menu-text text-center">R$ 30,00</span>
                    <input type="number" step="1" min="0" max="10" value="0" class="col-12">
                    <button type="button" class="btn btn-dark col-12">Comprar</button>
            </div>

            <div class="col-md-2 col-12 p-2 mx-3 mt-4">
                <img src="@/assets/img/imagem2.png" alt="" class="card-img-top img-fluid">
                    <h5 class="menu-text text-center py-3">Título</h5>
                    <p class="menu-text text-center fs-6">Lorem Ipsum is simply dummy text of the printing and typesetting industry. </p>
                    <span class="menu-text text-center">R$ 30,00</span>
                    <input type="number" step="1" min="0" max="10" value="0" class="col-12">
                    <button type="button" class="btn btn-dark col-12">Comprar</button>
            </div>

            <div class="col-md-2 col-12 p-2 mx-3 mt-4">
                <img src="@/assets/img/imagem3.png" alt="" class="card-img-top img-fluid">
                    <h5 class="menu-text text-center py-3">Título</h5>
                    <p class="menu-text text-center fs-6">Lorem Ipsum is simply dummy text of the printing and typesetting industry. </p>
                    <span class="menu-text text-center">R$ 30,00</span>
                    <input type="number" step="1" min="0" max="10" value="0" class="col-12">
                    <button type="button" class="btn btn-dark col-12">Comprar</button>
            </div>

        </div>   
    </section>
  <!--fim área cardápio-->

   <!--área galeria-->
    <section id="galeria" class="bg-black">
        <div class="container-fluid p-5">
          <div class="row">
            <div class="col-12 col-md-4">
                  <img src="@/assets/img/img-galeria1.jpg" alt="" >
              </div>
            <div class="col-12 col-md-4">
                <img src="@/assets/img/img-galeria2.jpg" alt="" >
            </div>
            <div class="col-12 col-md-4">
                <img src="@/assets/img/img-galeria3.jpg" alt="" >
            </div>
            <div class="col-12 col-md-4">
                <img src="@/assets/img/img-galeria4.jpg" alt="" >
            </div>
            <div class="col-12 col-md-4">
                <img src="@/assets/img/img-galeria5.jpg" alt="" >
            </div>
            <div class="col-12 col-md-4">
                <img src="@/assets/img/img-galeria2.jpg" alt="" >
            </div>
            
        </div>
    </div>    
    </section>
   <!--fim área galeria-->
   
    <!--área sobre-->
    <section id="sobre" class="bg-white">
        <div class="container">
            <div class="row">
                <div class="about-us-txt col-6 m-auto">
                    <h2 class="text-center p-4 fs-1">Sobre Nós</h2>
                    <p class="fs-5">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Placeat eligendi suscipit voluptatem maxime, ducimus consequatur illum perspiciatis, magni eum ad cupiditate deleniti reiciendis deserunt quaerat Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores cum debitis quasi iure iste minima facere pariatur, ab harum corporis.</p>
                </div>
                <h2 class="text-center pt-5 fs-2">Nosso Time</h2>
                <div class="col-6 col-md-3 p-3">
                    <img src="@/assets/img/chef-1.jpg" alt="">
                    <h2>Chef</h2>
                    <p class="fs-6">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                </div>

                <div class="col-6 col-md-3 p-3">
                    <img src="@/assets/img/chef-2.jpg" alt="">
                    <h2>Chef</h2>
                    <p class="fs-6">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                </div>

                <div class="col-6 col-md-3 p-3">
                    <img src="@/assets/img/chef-3.jpg" alt="">
                    <h2>Chef</h2>
                    <p class="fs-6">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                </div>

                <div class="col-6 col-md-3 p-3">
                    <img src="@/assets/img/chef-4.jpg" alt="">
                    <h2>Chef</h2>
                    <p class="fs-6">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                </div>
            </div>
        </div>
    </section>
    <!--fim área sobre-->

    <!--área do contato----------------->
        <section id="contato">
            <div class="container-fluid p-5">
                <div class="row">
                    <div class="col-md-12 col-12 areaMap">
                        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d467692.04890141165!2d-46.875499869998976!3d-23.681531440024322!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94ce448183a461d1%3A0x9ba94b08ff335bae!2zU8OjbyBQYXVsbywgU1A!5e0!3m2!1spt-PT!2sbr!4v1643416886303!5m2!1spt-PT!2sbr" width="98%" height="350" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
                    </div>
                    <h2>Inscreva-se e Receba nossas promoções!</h2>
                    <form class="">
                        <div class="pt-4">
                            <input class="" type="text" name="" id="" size="40" placeholder="Nome">
                        </div>
                        <div class="pt-4">
                            <input type="email" name="" id="" size="40" placeholder="E-mail ou telefone">
                        </div>
                        <button class="mt-4 btn btn-dark">Enviar</button>
                    </form>
                </div>
                
            </div>
        </section>
       
    <!--fim área contato-->

     <footer>
  <div class="container col-12 p-4">
     <div class="row">
        <div class="col-md-2">
          <ul class="list-group list-group-flush">
             <li class="listLink">
               <a class="noLink" href="#propaganda">Demonstração</a>
             </li>
             <li class="listLink">
               <a class="noLink" href="#sobre">Sobre</a>
             </li>
             <li class="listLink">
               <a class="noLink" href="#galeria">Galeria</a>
             </li>
             <li class="listLink">
               <a class="noLink" href="#contato">Contato</a>
             </li>
          </ul>
        </div>
          <div class="col-md-3">
             <h4 class="ps-4">Formas de Pagamento</h4>
             <img src="@/assets/img/pagamento.jpg" alt="" class="img-fluid">
          </div>
          
          <div class="col-2">
            <h4>Horário de Atendimento</h4>
            <ul>
              <li>Seg/Terç<span> 7h até 12h</span></li>
              <li>Qua/Qui<span> 7h até 12h</span></li>
              <li>Sext/Sáb<span> 7h até 12h</span></li>
              <li>Dom<span> - Fechado</span></li>
            </ul>
          </div>
          <div class="col-3">
             <h4>Social</h4>
          </div>
          <div class="col-2">
            <h4>Segurança</h4>
          </div>
    </div>
  </div>
   </footer>
    
   
  </main>
</template>


<script>
// @ is an alias to /src -- "@" é um atalhos para a pasta principal do projetos "/src"
import HeaderPage from "@/components/HeaderPage.vue";
import NavbarPage from "@/components/NavbarPage.vue";

export default {
  //name: "PrincipalPage", //Podemos Apagar por que vamos usar o nome do arquivo.
  components: {
    HeaderPage,
    NavbarPage,
  },
};
</script>


<style scope>


.imgBG1,
.imgBG2,
.imgBG3 {
  background-size: cover;
  background-position: center;
  min-height: 500px;
}

.imgBG1 {
  background-image: url(@/assets/img/banner1.jpg);
}

.imgBG2 {
  background-image: url(@/assets/img/banner2.jpg);
}

.imgBG3 {
  background-image: url(@/assets/img/banner3.jpg);
}
/*seção propaganda----------------*/
.menu-propaganda{
    color: #000000;
}
.imagem-propaganda{
    width: 300px;
    padding-top: 40px;
}
/*----seçao cardapio------*/
.menu-text{
    color: #ffffff;
}
.card-img-top:hover {
    transform: scale(1.3);
}
.card-img-top{
    transition: transform 0.2s;
}

/*section galeria */
#galeria img{
    border: 1px solid black;
    width: 100%;
    transition: transform, border-radius, 0.3s; 
}
#galeria img:hover{
   transform: scale(1.1);
   border-radius: 100% 0% 0% 100% / 0% 99% 1% 100%;
}
#galeria h1{
    color: white;
}



.btnVoltar {
  position: fixed;
  bottom: 20px;
  right: 20px;
  padding: 10px;
  font-size: 2em;
  /* border: solid 3px;
    border-radius: 50px; */
}

.btnVoltar a {
  text-decoration: none;
}

a {
  color: #555;
}

.nolink {
  text-decoration: none;
  color: inherit;
}

/*area de contato -----------*/
#contato{
    border-top: 1px solid black;
}

/*--------footer*/
footer{
    border: 1px solid black;
    font-size: 0.9em;
    background-color: #121619;
}
footer ul li{
    list-style: none;
}
footer li, a, h4{
    color: #FFFFFF;
}
footer h4 {
    font-size: 0.9em;
    font-weight: bold;
}
.noLink{
    text-decoration: none;
    color: inherit;
}
.listLink{
    text-decoration: none;
    list-style: none;
    
}
</style>






