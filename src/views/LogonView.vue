<template>
  <div>
    <NavbarPage />
    <section class="container">
      <form action="" class="col-12 col-md-6 m-auto bg-white p-5">
      <h3 class="text-center">Login do Cliente</h3>
       <i class="bi bi-person-fill fs-1 text-center d-block"></i>
        <div class="form-group">
          <label class="text-center d-block fs-5">E-mail</label>
          <input
            type="email" placeholder="Ex. joaodasilva@gmail.com"
            v-model="dadosUsuario.usuario"
            class="form-control"
          />
        </div>
        <div class="form-group py-4">
          <span class="d-block text-center fs-5"
            ><label>Senha</label> </span
          >
          <input
            type="password"
            v-model="dadosUsuario.senha"
            class="form-control"
          />
        </div>

        <div class="form-group my-1">
          <div class="d-grid gap-2 d-md-flex justify-content-md-end">
            <button
              type="button"
              class="btn btn-danger mx-1 px-3"
              @click="logonUsuario()"
            >
              Entrar
            </button>
            <button
              type="button"
              class="btn btn-danger px-3"
              @click="logoffUsuario()"
            >
              Sair
            </button>
          </div>
        </div>
        <hr />
        <div class="form-group right my-1">
          <!-- <button type="button" @click="$router.push('usuario_add')" class="btn btn-danger mx-1">
            Cadastrar
          </button> -->
          <div class="d-grid gap-2">
            <router-link to="usuario_add" class="btn cadastrar mx-1 bg-red">
              Cadastrar
            </router-link>
          </div>
        </div>
      </form>
    </section>
  </div>
</template>

<script>
import NavbarPage from "@/components/NavbarPage.vue";
import UsuarioService from "@/services/usuarioService";
import router from "@/router";

export default {
  components: {
    NavbarPage,
  },
  data() {
    return {
      dadosUsuario: {
        usuario: "",
        senha: "",
      },
    };
  },
  mounted() {
    //this.loadDoc("http://localhost/api/usuario/list", myFunction);
    //this.listarUsuarios();
  },
  methods: {
    // function loadDoc(url, xFunction) {
    //   const xhttp = new XMLHttpRequest();
    //   xhttp.onload = function () {
    //     xFunction(this);
    //   };
    //   xhttp.open("GET", url);
    //   xhttp.send();
    // }
    // function myFunction(xhttp) {
    //   console.log(xhttp.responseText);
    // }

    listarUsuarios() {
      UsuarioService.list().then((res) => {
        console.log(res);
      });
    },
    logonUsuario() {
      UsuarioService.login(this.dadosUsuario)
        .then((res) => {
          console.log(res);
          localStorage.setItem("token", res.data.result.token);
          localStorage.setItem("user", JSON.stringify(res.data.result));
          alert("Usuario logado!");
          router.push("/");
        })
        .catch((err) => {
          console.log(err);
          alert("Erro ao fazer o login!");
        });
    },
    logoffUsuario() {
      localStorage.clear();
      router.push("/");
    },
  },
};
</script>

<style scoped>
   .cadastrar:hover{
     background-color: rgb(226, 63, 63);
   }
</style>