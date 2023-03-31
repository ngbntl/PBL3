<template>
 <div class="container">
    <h2>Gửi yêu cầu: </h2>
    <div>
        <div class="listRe">
           
          <h3> Danh mục yêu cầu: </h3>
            <ul>
                <li >
                    <button class="button" >Gửi yêu cầu</button>
                </li>
                <li class="content">
                   <b> <label for=""> Loại yêu cầu:</label></b>
                    <select name="" id="">
                        <option value="">Đơn</option>
                        <option value="">Giấy xin</option>
                    </select>
                   </li>
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
            <div>
                <b><label for="">Loại đơn:</label></b>
                <select name="" id="">
                    <option value="">Đơn xin </option>
                    <option value="">Đơn xin ẻ</option>
                </select>
            </div>
            
        </li>
        <li class="content">
            <b>
            <label for=""> Nội dung:</label></b>
            <input type="Tôi bị gay">
           </li>
    </ul>
       
    </div>
     <div class="listRe">
        <h3>Chỉnh sửa thông tin: </h3>
            <ul>
                <li class="content">
                    <b><label for="">Thông tin cần sửa: </label></b>
                    <select name="" id="">
                    <option value="">Họ tên</option>
                    <option value="">Số CCCD</option>
                    <option value="">Ngày sinh</option>
                    <option value="">Giới tính</option>
                    <option value="">Địa chỉ</option>
                    </select>
                </li>
            </ul>
     </div>
     <div class="listRe">
        <h3>Danh sách yêu cầu đã gửi:</h3>
     </div>
     <FooterPage />
 </div>
</template>

<script>
import FooterPage from '~/components/Footer/FooterPage.vue'
export default {
    components: {
        
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
    padding: 20px;
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
input {
  margin: 0px -10px;
  width: 70%;
  padding: 10px;
  border: 2px solid green;
  box-sizing: border-box;
  border-radius: 10px; ;
  
}
select {
 width: 80%;
  padding:10px;
  border: none;
  border-radius: 4px;
  background-color: rgb(181, 230, 181);
  
}

</style>