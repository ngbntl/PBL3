<template>
    
    <div class="container">
        <div>
                <HeaderPage />
            </div>
        <h2>Thông tin nhân thân:</h2>
        <div>
            <div>
                <div class="infor">
    
                    <div class="infor-content">
                        <ul class="list-infor">
                            <li>
                               Cha: <span>{{ listInfor.namec }}</span>
                            </li>
                            <li>
                               Mẹ:
                                <span>{{ listInfor.namem }}</span>
                            </li>
                            <li>
                               Chủ hộ:
                                <span > {{ listInfor.Chuho }}</span>
                            </li>
                            <li>
                                Mối quan hệ với chủ hộ:
                                <span>{{ listInfor.nationality }}</span>
                            </li>
                           
                        </ul>
                        <ul class="list-infor">
                            <li>
                                Ngày sinh:
                                <span>{{ listInfor.birthc }}</span>
                            </li>
                            <li>
                                Ngày sinh:
                                <span>{{ listInfor.birthm }}</span>
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
                           
                        </ul>
                    </div>
                </div>
            </div>
            
        </div>
        <div>
            <FooterPage />
        </div>
    </div>
</template>
    
<script>
import HeaderPage from '~/components/Header/HeaderPage.vue'
import FooterPage from '../../components/Footer/FooterPage.vue';
export default {
    components: {
        HeaderPage,
        FooterPage,
    },
    data() {
        return {
            listInfor: {
                namec: "Mo coi",
                namem:"KHong co",
                birthc: "121212",
                birthm: "121212",
                idFamily: "123",
                Chuho:"Mo coi",
                address: "123 Ngo Si Lien",
                location: {
                    location_id: 123,
                    quarter: "Dau do",
                    town: "Hoa Minh",
                    district: "Lien Chieu",
                    city: "Da Nang",
                },
               
            },
        };
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

.container {
    padding: 0;
    overflow: hidden;
}

.container h2 {
    padding: 10px;
    width: fit-content;
    margin-bottom: 0;
}

ul {
    list-style: none;
}

.infor {
    display: flex;
    align-items: center;
    justify-content: center;
    border-top: 2px solid green;
    border-bottom: 2px solid green;
}

.infor-content {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 70%;
}

.list-infor {
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
    padding: 20px;
    border-bottom: 2px solid green;
    margin-bottom: 30px;
}

.crimimal-content {
    background-color: #f3f3f3;
    padding: 20px 10px;
    border-radius: 10px;
    min-height: 100px;
    margin-bottom: 10px;
}
</style>