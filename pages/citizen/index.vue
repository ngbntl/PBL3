<template>
    <div class="overlay">
        <img src="https://top10dienbien.com/wp-content/uploads/2022/10/avatar-cute-11.jpg" alt="" />
        <h2>{{ listInfor.name }}</h2>
        <div class="container">
            <h2 class="h2">Thông tin cá nhân:</h2>

            <div>
                <div>
                    <div class="infor">

                        <div class="infor-content">
                            <ul class="list-infor">
                                <li>
                                    Họ và tên: <span>{{ listInfor.name }}</span>
                                </li>
                                <li>
                                    Số CCCD:
                                    <span>{{ listInfor.citizen_id }}</span>
                                </li>

                                <li>
                                    Giới tính:
                                    <span :keyup="gender(listInfor)"> {{ genderEx }}</span>
                                </li>
                                <li>
                                    Quốc tịch:
                                    <span>{{ listInfor.nationality }}</span>
                                </li>
                                <li>
                                    Nghề nghiệp:
                                    <span>{{ listInfor.profession }}</span>
                                </li>
                                <li>
                                    Số điện thoại:
                                    <span function="gender(listInfor)">{{ genderEx }}</span>
                                </li>
                            </ul>
                            <ul class="list-infor">
                                <li>
                                    Ngày sinh:
                                    <span>{{ listInfor.birth }}</span>
                                </li>
                                <li>
                                    Dân tộc:
                                    <span>{{ listInfor.ethinic }}</span>
                                </li>
                                <li>
                                    Số hộ khẩu:
                                    <span>{{ listInfor.idFamily }}</span>
                                </li>
                                <li>
                                    Tôn giáo:
                                    <span>{{ listInfor.religion }}</span>
                                </li>
                                <li>
                                    Quê quán:
                                    <span>
                                        {{
                                            listInfor.address +
                                            " " +
                                            listInfor.location.quarter +
                                            " " +
                                            listInfor.location.town +
                                            " " +
                                            listInfor.location.district +
                                            " " +
                                            listInfor.location.city
                                        }}</span>
                                </li>
                                <li>
                                    Email:
                                    <span>123@gmail.com</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                
            </div>
        </div>
        <div class="crimiantion">
                        <h2 class="h2">Tiền án tiền sự:</h2>
                        <div class="crimimal-content">
                            Nội dung: {{ listInfor.criminalRecord }}
                        </div>
                    </div>
    </div>
</template>
    
<script>
export default {
    components: {},
    data() {
        return {
            listInfor: {
                citizen_id: '52',
                name: "Nhan",
                pass: "nhan",
                birth: "121212",
                idFamily: "123",
                gender: false,
                ethinic: "Kinh",
                religion: "khong",
                nationality: "Viet Nam",
                address: "123 Ngo Si Lien",
                location: {
                    location_id: 123,
                    quarter: "Dau do",
                    town: "Hoa Minh",
                    district: "Lien Chieu",
                    city: "Da Nang",
                },
                profession: "Sinh vien",
                criminalRecord: "khong co",
                number: 84123456789,
                email: "123@gmail.com",
            },
            genderEx: "nu",
        };
    },
    methods: {
        gender(list) {
            if (list.gender === false) return (this.genderEx = "nữ");
            else return (this.genderEx = "nam");
        },
    },
};
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

.overlay img {
    position: absolute;
    width: 94px;
    height: 94px;
    left: 500px;
    top: 126px;

    background: #D9D9D9;
}

.overlay h2 {
    position: absolute;
    width: 234px;
    height: 49px;
    left: 570px;
    top: 145px;

}

.container {
    position: absolute;
    width: 1027px;
    height: 538px;
    left: 500px;
    top: 245px;

    background: #FFFFFF;
    border-radius: 13px;
}

.container .h2 {
    position: absolute;
    width: 224px;
    height: 49px;
    left: 7px;
    top: 2px;

}

ul {
    list-style: none;
}

.infor {
    display: flex;
    align-items: center;
    justify-content: center;
    
}

.infor-content {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 70%;
}

.list-infor {
    padding-top: 40px;
    width: 50%;
}

.list-infor li {

    padding-bottom: 20px;
    line-height: 2;
    font-weight: 550;

}

.list-infor li span {
    font-weight: 400;
}

img {
    width: 180px;
    height: 210px;
    margin-right: 20px;
}

.crimiantion {
position: absolute;
width: 1027px;
height: 186px;
left: 500px;
top: 806px;
background: #FFFFFF;
border-radius: 13px;
}

.crimimal-content {
   
    padding: 70px 40px;
    border-radius: 10px;
    min-height: 100px;
    margin-bottom: 10px;
}
</style>