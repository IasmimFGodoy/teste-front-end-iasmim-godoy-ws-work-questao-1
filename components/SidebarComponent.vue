<template>
    <div class="sidebar">
        <h2>Categories</h2>
        <ul>
            <li id="current-item">Healthy & Care</li>
            <li>Food</li>
            <li>Pet</li>
            <li>Hardware</li>
            <li>Flowers</li>
            <li>Garden's</li>
            <li>Beauty & Hair</li>
        </ul>
    </div>
</template>
<style>
.sidebar {
    width:150px;
    height: 560px;
    border-right: 3px solid black;
    background-image: linear-gradient(to right, #D7FFF1, #AAFCB8);
}
.sidebar h2 {
    text-align: center;
    position:relative;
    top: 1rem;
    font-size: 20px;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
.sidebar ul {
    position:relative;
    top: 2rem;
}
.sidebar ul li {
    list-style-type: '-';
    font-size: 13px;
    margin-left: 10%;
    margin-bottom: 1%;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
.sidebar ul li:hover {
    cursor: pointer;
    color: #285943;
}
#current-item {
    text-decoration: underline;
    font-weight: bold;
}

</style>