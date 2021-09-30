<template>
    <header>
        <img src="../assets/img/logo-sidearea-1.png" alt="">
        <ul>
            <li class="selected">HOME</li>
            <li>PAGES</li>
            <li>PORTFOLIOBLOG</li>
            <li>SHOP</li>
            <li>ELEMENTS</li>
            <li><img src="../assets/svg/svg-1.svg" alt=""></li>
        </ul>
    </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped lang="scss">
header {
    height: 80px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 30px;
    ul {
        display: flex;
        justify-content: space-between;
        align-items: center;
        list-style: none;
        width: 40%;
        li {
            position: relative;
            font-weight: 600;
            font-size: 11px;
        }
        .selected::after {
            position: absolute;
            bottom: 2px;
            left: 0;
            content: "";
            width: 100%;
            border-bottom: 5px solid #F3D0C7;
            z-index: -1;
        }
    }
}
</style>
