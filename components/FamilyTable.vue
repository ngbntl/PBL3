<template>
    <div class="family-table">
        <table>
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Age</th>
                    <th>Gender</th>
                    <th>Relationship</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="(member, index) in familyMembers" :key="index">
                    <td>{{ member.name }}</td>
                    <td>{{ member.age }}</td>
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
                { name: "John Doe", age: 35, gender: "Male", relationship: "Father" },
                { name: "Jane Doe", age: 32, gender: "Female", relationship: "Mother" },
                { name: "Jack Doe", age: 7, gender: "Male", relationship: "Son" },
                { name: "Jill Doe", age: 5, gender: "Female", relationship: "Daughter" },
            ],
        };
    },
};
</script>

<style scoped>
.family-table {
    margin: 20px auto;
    max-width: 600px;
}

table {
    width: 100%;
    border-collapse: collapse;
}

th {
    text-align: left;
    padding: 10px;
    background-color: #f5f5f5;
    border: 1px solid #ccc;
}

td {
    text-align: left;
    padding: 10px;
    border: 1px solid #ccc;
}

tr:nth-child(even) {
    background-color: #f2f2f2;
}

tr:hover {
    background-color: #ddd;
}
</style>
