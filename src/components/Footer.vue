<template>
    <footer>
        <div class="container">
            <div>
                <img src="../assets/img/logo-sidearea-1.png" alt="">
                <p>Let's Get Creatvie</p>
            </div>
            <div>
                <p>maree.qode@gmail.com</p>
                <p class="phone">+8563 950 600</p>
            </div>
            <div>
                <p>Avenue d'Auderghem 10</p>
                <p class="city">1040 Brussels, Belgium</p>
            </div>
            <div>
                <p>Stay in touch with us</p>
                <div class="socials">
                    <i class="fab fa-twitter"></i>
                    <i class="fab fa-pinterest-p"></i>
                    <i class="fab fa-facebook-f"></i>
                    <i class="fab fa-linkedin-in"></i>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped lang="scss">
footer {
    background-color: #d6e9de;
    .container {
        display: flex;
        justify-content: space-between;
        height: 200px;
        width: 60%;
        margin: auto;
        padding-top: 50px;
        &>div {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            height: 60px;
        }
        .socials {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }
    }
}
</style>
