<template lang="">
<div class="social">
            <a href="#"><i class='bx bxl-facebook'></i></a>
            <a href="#"><i class='bx bxl-twitter'></i></a>
            <a href="#"><i class='bx bxl-instagram'></i></a>
            <a href="#"><i class='bx bxl-youtube'></i></a>
        </div>

        <p>&#169; Test.</p>
</template>
<script>
export default {

}
</script>
<style scoped>
.footer {
   position: fixed;
   left: 0;
   bottom: 0;
   height: 30px;
   width: 100%;
   background-color: #333;
   color: rgb(0, 0, 0);
   text-align: center;
}
.social a {
    font-size: 27px;
    margin: 0.5rem;
    padding-top: 50%;
}

.social a .bx {
    padding: 5px;
    color: #fff;
    background: #000000;
    border-radius: 50%;
}
</style>