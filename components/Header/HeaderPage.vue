<template>
  <div class="container">
            <Logo />
            <div class="header">
                <ul class="content">
                    <li class="nav-item">
                        <svg class="logo-home" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512">
                            <path
                                d="M575.8 255.5c0 18-15 32.1-32 32.1h-32l.7 160.2c0 2.7-.2 5.4-.5 8.1V472c0 22.1-17.9 40-40 40H456c-1.1 0-2.2 0-3.3-.1c-1.4 .1-2.8 .1-4.2 .1H416 392c-22.1 0-40-17.9-40-40V448 384c0-17.7-14.3-32-32-32H256c-17.7 0-32 14.3-32 32v64 24c0 22.1-17.9 40-40 40H160 128.1c-1.5 0-3-.1-4.5-.2c-1.2 .1-2.4 .2-3.6 .2H104c-22.1 0-40-17.9-40-40V360c0-.9 0-1.9 .1-2.8V287.6H32c-18 0-32-14-32-32.1c0-9 3-17 10-24L266.4 8c7-7 15-8 22-8s15 2 21 7L564.8 231.5c8 7 12 15 11 24z" />
                        </svg>
                        <nuxt-link to="/citizenn" href="" class="link">Trang chủ</nuxt-link>
                    </li>
                    <li class="nav-item see-inf">
                        <a href="" class="link" >Xem thông tin</a>
                        
                        <ul class="seeing-child button_cont ">
                            <li>
                                <a class="example_b " href="/Family/Family_inf"  rel="nofollow noopener">thông tin gia đình</a> 
                            </li>
                            <li>
                                <a class="example_b" href="/Leader" rel="nofollow noopener">Xem thông tin công chức nhà nước</a>
                            </li>
                        </ul>
                    </li>
                    <li class="nav-item send-inf">
                        <nuxt-link to="/GuiYC">
                        <a href="" class="link"> Gửi yêu cầu</a>
                        </nuxt-link>
                    </li>
                    <li class="nav-item">
                        <a href="" class="link">Hẹn lịch</a>
                    </li>
                    <li class="nav-item">
                        <a href="" class="link">Nhận thông báo</a>
                    </li>
                    <li class="nav-item">
                        <a href="" class="link">Đóng góp ý kiến</a>
                    </li>
                </ul>

                <div class="user">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512">
                        <path
                            d="M224 256A128 128 0 1 0 224 0a128 128 0 1 0 0 256zm-45.7 48C79.8 304 0 383.8 0 482.3C0 498.7 13.3 512 29.7 512H418.3c16.4 0 29.7-13.3 29.7-29.7C448 383.8 368.2 304 269.7 304H178.3z" />
                    </svg>
                    <span class="nickname ">Eimi Fukada
                        <nuxt-link to="/citizen/changePass" class="passchange example_b" >Đổi mật khẩu</nuxt-link>
                    </span>

                    <nuxt-link to="/login">
                        <svg xmlns="http://www.w3.org/2000/svg" class="logout" viewBox="0 0 512 512">
                            <path
                                d="M377.9 105.9L500.7 228.7c7.2 7.2 11.3 17.1 11.3 27.3s-4.1 20.1-11.3 27.3L377.9 406.1c-6.4 6.4-15 9.9-24 9.9c-18.7 0-33.9-15.2-33.9-33.9l0-62.1-128 0c-17.7 0-32-14.3-32-32l0-64c0-17.7 14.3-32 32-32l128 0 0-62.1c0-18.7 15.2-33.9 33.9-33.9c9 0 17.6 3.6 24 9.9zM160 96L96 96c-17.7 0-32 14.3-32 32l0 256c0 17.7 14.3 32 32 32l64 0c17.7 0 32 14.3 32 32s-14.3 32-32 32l-64 0c-53 0-96-43-96-96L0 128C0 75 43 32 96 32l64 0c17.7 0 32 14.3 32 32s-14.3 32-32 32z" />
                        </svg>
                    </nuxt-link>                              
                </div>
            </div>
           <nuxt-child />
        </div>
</template>

<script>
export default {

}
</script>

<style scoped>
 body {
    margin: 0;

 }
 html {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.container {
    margin: 0;
    padding: 0;
    overflow: hidden;
    box-sizing: border-box;
    
   
}

.header {
   
    display: flex;
    align-self:center;
    justify-content: space-between;
    background-color: green;
    height: auto;
    color: #fff;

}
.hoverr:hover{
    color: aquamarine;
}
.content {
    display: flex;
    height: auto;
    margin: 0;
}

.nav-item {
    text-align: center;
    border-radius: 4px;
    padding: 15px 30px;
    margin-right: 0px;
}

.nav-item:hover {
    background-color: #fff;
}

.nav-item:active {
    background-color: #fff;
}

.nav-item:active .link {
    color: black;
}

.nav-item svg {
    width: 18px;
    height: auto;
    fill: #fff;
    padding-right: 10px;
}

.passchange {
    display: none;
    background-color: green;
    color: #fff;
    position: absolute;
    top: 150px;
    right: 71px;
    padding: 10px;
    width: 150px;
}

.nickname:hover .passchange {
    display: block;
}

.nickname {
    padding: 15px 10px;
    border-radius: 4px;
}

.nickname:hover {
    background-color: #fff;
    color: black;
}

.seeing-child {
    display: none;
    position: absolute;
    left: 208px;
    top: 150px;
    border-radius:10px ;
    text-align: start;
    width: 250px;
    height: 80px;
    background-color: green;
    color: #fff;
}

.seeing-child li {
    padding-top: 10px ;
    padding-left:0px ;
    
}


.nav-item:hover .seeing-child {
    display: block;
}

.nav-item:hover .link {
    color: black;
}

.nav-item:hover .logo-home {
    fill: black;
}

.user {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-right: 10px;
}

.user svg {
    width: 20px;
    height: auto;
    padding: 0 20px;
    fill: #fff;
}

a {
    cursor: pointer;
    text-decoration: none;
    color: #fff;
}

.container h2 {
    padding: 10px;
    width: fit-content;
    margin-bottom: 0;
}

ul {
    list-style: none;
}

.logout:hover {
    background-color: #fff;
    padding: 5px 10px;
    fill: black;
    margin-left: 20px;
    border-radius: 5px;
}
.example_b {
color: #fff !important;
text-decoration: none;
padding: 10px;
border: none;
transition: all 0.4s ease 0s;
}
.example_b:hover {
text-shadow: 0px 0px 6px rgba(255, 255, 255, 1);
transition: all 0.4s ease 0s;
}

</style>