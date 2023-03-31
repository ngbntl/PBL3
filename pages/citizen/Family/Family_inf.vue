<template>
  <div class="container">
    <table>
      <thead>
        <tr>
          <th>STT</th>
          <th>Họ tên</th>
          <th>Năm sinh</th>
          <th>Giới tính</th>
          <th>Quan hệ</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(member, index) in familyMembers" :key="index">
          <td>{{ member.id }}</td>
          <td>{{ member.name }}</td>
          <td>{{ member.birth }}</td>
          <td>{{ member.gender }}</td>
          <td>{{ member.relationship }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      familyMembers: [
       
        { id: 1, name: "Jill Doe", birth: 5, gender: "Nam", relationship: "Vợ" },
        { id: 1, name: "Jdfsdfsd", birth: 5, gender: "Nam", relationship: "Vợ" },
      ],
    };
  },
};
</script>

<style scoped>
html,
body {
	height: 100%;
}


.container {
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
}

table {
	width: 800px;
	border-collapse: collapse;
	overflow: hidden;
	box-shadow: 0 0 20px rgba(0,0,0,0.1);
}

th,
td {
	padding: 15px;
	background-color: rgba(255,255,255,0.2);
	color: #000000;
}

th {
	text-align: left;
}

thead th{
	
		background-color: #4bc26b;
	
}

tbody tr:hover{

		
			background-color: rgba(91, 225, 160, 0.3);
		
	}
	tbody td {
		position: relative;
		
	}
  


</style>
