<template lang="html">
    <div class="container">
        <div class="header-people">
            <div class="search-box">
                <h2>Search for a user</h2>
                <input type="text" placeholder="Search" class="search">
            </div>
            <img src=".././assets/logo.png" alt="logo">
        </div>
        <div>
            <h1>Users</h1>
            <table>
                <thead>
                    <tr>
                        <th>Nome</th>
                        <th>Cpf</th>
                        <th>Data nascimento</th>
                        <th>Acoes</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Kelvis Delapena</td>
                        <td>118.176.469-66</td>
                        <td>24/06/2001</td>
                        <td>
                            <button class="edit">Add</button>
                            <button class="remove">remove</button>
                        </td>
                    </tr>
                    <tr>
                        <td>Kelvis Delapena</td>
                        <td>118.176.469-66</td>
                        <td>24/06/2001</td>
                        <td>
                            <button class="edit">Add</button>
                            <button class="remove">remove</button>
                        </td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</template>

<script lang="ts">
import Header from '../components/layout/Header.vue'

export default {
    name: "People",
    components: { Header }
}
</script>

<style>
.container {
    width: 100vw;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #1A202C;
    color: #ffffff;
}

.header-people {
    margin: 50px 0px;
    width: 50%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.search-box {
    margin-bottom: 70px;
}

.search {
    width: 300px;
    height: 20px;
    border-radius: 5px;
    border: none;
    padding: 5px;
}

.edit {
    background-color: transparent;
    border: none;
    color: #ffffff;
    font-weight: bold;
}

.remove {
    background-color: transparent;
    border: none;
    color: #ffffff;
    font-weight: bold;
}

table {
    width: 50vw;
    border-collapse: collapse;
}

th,
td {
    padding: 1rem;
    text-align: left;
    border-bottom: 1px solid #ccc;
    border-spacing: 0;
}
</style>