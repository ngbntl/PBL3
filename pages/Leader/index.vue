<template>
  <div class="container">
    <HeaderPage />
    <h2>Thông tin cán bộ:</h2>
    <div>
      <div>
        <div class="infor">
          <img src="https://i1-vnexpress.vnecdn.net/2023/01/18/ctn-nguyen-xuan-phuc-167403272-6482-7541-1674036541.jpg?w=0&h=0&q=100&dpr=2&fit=crop&s=vuuE4c08lrADCaRSzLHLww" alt="" />
          <div class="infor-content">
            <ul class="list-infor">
              <li>
                Họ và tên: <span>{{ listInfor.name }}</span>
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
                 Chức vụ:
                  <span>{{ listInfor.level }}</span>
                </li>
                <li>
                  Nhiệm kỳ:
                  <span>{{ listInfor.term }}</span>
                </li>
                <li>
                  Trình độ học vấn:
                  <span>{{listInfor.Edu }}</span>
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
                Tôn giáo:
                <span>{{ listInfor.religion }}</span>
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
</template>
    
<script>
export default {
  components: {},
  data() {
    return {
      listInfor: {
        name: "Nguyễn Xuân Phúc",
        birth: "12/03/1978",
        gender: true,
        ethinic: "Kinh",
        religion: "khong",
        address: "123 Ngo Si Lien",
        level: "Chủ tịch nước",
        term: "2019-2022",
        Edu:"Tiến sĩ",
        location: {
          location_id: 123,
          quarter: "Dau do",
          town: "Hoa Minh",
          district: "Lien Chieu",
          city: "Da Nang",
        },
          
        
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