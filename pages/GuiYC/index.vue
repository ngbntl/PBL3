<template>
 <div class="container">
    <HeaderPage />
    <h2>Gửi yêu cầu: </h2>
    <div>
        <div class="listRe">
           
          <h3> Danh mục yêu cầu: </h3>
            <ul>
                <li >
                    <button class="button" >Gửi yêu cầu</button>
                </li>
                <li class="content">Loại yêu cầu:</li>
            </ul>
                
           
          
        </div>
    </div>
    <div class="listRe">
    <h3>Nội dung yêu cầu:</h3>
    <ul>
        <li>
             <button class="button">Lập đơn</button>
        </li>
        <li class="content">
            Loại đơn:
        </li>
        <li class="content">Nội dung:</li>
    </ul>
       
    </div>
     <div class="listRe">
        <h3>Chỉnh sửa thông tin: </h3>
            <ul>
                <li class="content">Thông tin cần sửa: </li>
            </ul>
     </div>
     <div class="listRe">
        <h3>Danh sách yêu cầu đã gửi:</h3>

     </div>
     <FooterPage />
 </div>
</template>

<script>
import HeaderPage from '~/components/Header/HeaderPage.vue'
import FooterPage from '~/components/Footer/FooterPage.vue'
export default {
    components: {
        HeaderPage,
        FooterPage
    }

}
</script>

<style scope>
body {
    margin: 0;
}

html {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.container {
    padding: 0;
    overflow: hidden;
}
.container h2 {
    padding: 10px;
    width: fit-content;
    margin: 0px 30px;
}
ul {
    list-style: none;
}
.listRe {
    background-color: #f3f3f3;
    padding: 30px 10px;
    min-height: 100px;
    margin: 10px 30px;
    margin-bottom: 50px;

}
.listRe h3 {
    padding: 10px;
    width: fit-content;
    margin-top: -40px;
}
.content {
   display: flex;
    justify-content: space-around;
    align-items: center;
    width: 50%;
    top: -10px;
    margin-bottom: 20px;
}
.button {
    box-sizing: border-box;
    padding: 10px;
    border-radius: 10px;
    color: #f3f3f3;
    border: none;
    position: absolute;
    background-color: green;
    font-family: 'Times New Roman', Times, serif;
    font-size: 14px;
    margin: 0px 40px;
}



</style>