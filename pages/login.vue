<template>
    <div class="container">
        <div class="logo-login">
            <img src="../static/logo.jpg" alt="" />
            <h2>Hệ thống quản lý hồ sơ điện tử công dân</h2>
        </div>
        <div class="card">
            <div class="content">
                <form @submit.prevent="login">
                    <div class="form">
                        <h2>Đăng nhập</h2>
                        <p>Tài Khoản</p>
                        <input v-model="citizen_id" type="text" class="box" name="" id="" placeholder="Nhập số CCCD"
                            required />
                        <p>Mật khẩu</p>
                        <input class="box" :type="showPassword ? 'text' : 'password'" v-model="password"
                            placeholder="Nhập mật khẩu" required />
                        <div class="showButton">
              <!-- <button @click="showPassword = !showPassword" class="show-pass">
                {{ showPassword ? "Ẩn" : "Hiện" }} Mật khẩu
              </button> -->
            </div>
                        <button class="login">Đăng nhập</button>
                        
                    </div>
                </form>
            </div>
        </div>
        <FooterPage />
    </div>
</template>
  
<script>
import FooterPage from "~/components/Footer/FooterPage.vue";
export default {
    components: {
        FooterPage,
    },
    data() {
        return {
            citizen_id: "",
            password: "",
            showPassword: false,
            list: {},
        };
    },
    mounted() {
        this.id = localStorage.getItem("id");
        // this.fectchData();
    },
    methods: {
        async login() {
            try {
                await this.$auth.loginWith('local', {
                    data: {
                        citizen_id: this.citizen_id,
                        password: this.password,
                    }
                })
                this.$router.push('/');
            } catch (error) {
                console.error(error);
            }
        },
        // async fectchData() {
        //   try {
        //     await this.$axios.get(
        //         `http://localhost:8080/api/citizen/listCitizen/id=${this.id}`
        //       )
        //       .then((res) => {
        //         this.list = res['data'];
        //         // alert("aaaa");
        //       });
        //   } catch (error) {
        //     console.log(error);
        //   }
        // },

    },
    // async login(){
    //   try {
    //     await this.$axios.post("http://localhost:8080/api/v1/auth/authenticate", {
    //       citizen_id: this.citizen_id,
    //       password: this.password
    //     }).then(
    //       res=> {
    //         localStorage.setItem("id", this.citizen_id);
    //         this.$router.push('/');
    //       }
    //     )
    //   } catch (error) {
    //     console.log(error);
    //   }
    //},
    // async login() {
    //   try {
    //     const response = await fetch("http://localhost:8080/api/v1/auth/authenticate", {
    //       method: "POST",
    //       body: JSON.stringify({
    //         username: this.username,
    //         password: this.password,
    //       }),
    //       headers: {
    //         "Content-Type": "application/json",
    //       },
    //     });
    //     if (response.ok) {
    //       const data = await response.json();
    //       // Lưu token vào Vuex store
    //       this.$store.commit("auth/setToken", data.token);
    //       // Chuyển hướng đến trang chủ
    //       this.$router.push("/");
    //     } else {
    //       const error = await response.text();
    //       console.error(error);
    //     }
    //   } catch (error) {
    //     console.error(error);
    //   }
    // },
    //},
};
</script>
<style scoped>
body {
    padding: 0;
    margin: 0;
}

html {
    margin: 0;
    padding: 0;
    overflow: hidden;
}

.container {
    width: 100%;
}

.content {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 50px;
    margin-top: 25px;
}

.logo-login {
    text-align: center;
    padding-top: 20px;
}

img {
    width: 100px;
    height: auto;
}

.form {
    padding: 10px 40px 40px;
    background-color: #fff;
    height: 380px;
    width: 300px;
    border: 0.5px solid black;
}

.form h2 {
    font-size: 40px;
    color: green;
    text-align: center;
}

input {
    width: 300px;
    height: 30px;
    border: 1px solid green;
    border-radius: 4px;
}

.checkbox {
    width: 20px;
    height: auto;
}

.showButton {
    text-align: end;
    padding-top: 10px;
}

.show-pass {
    text-align: end;
    padding-top: 10px;
    background-color: green;
    color: #fff;
    margin-top: 10px;
    padding: 5px 10px;
    border-radius: 5px;
    border: none;
    cursor: pointer;
}

.login {
    width: 305px;
    height: 35px;
    margin-top: 30px;
    background: green;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

.box {
    padding: 5px 10px;
}
</style>