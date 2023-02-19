<template>
    <div class="bag play_confirm">
        <div class="play_confirm">
        <h1>Ushbu kurs haqida</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus corporis quidem aliquam dolores accusantium, explicabo sunt hic a magnam laborum excepturi reprehenderit, facilis nesciunt recusandae magni voluptatum. Harum, reiciendis facilis.</p>
        <button @click="$emit('closeModal')" class="btn btn-danger">Close</button>
    </div>
    </div>
   

</template>
<script>
export default {
    components: {
    },
}
</script>
<style scoped>
.play_confirm{
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    height: 450px;
    background-color: rgb(255, 255, 255);
    /* border: 2px solid rgba(0, 0, 0, 0.473); */
    box-shadow: 0px 0px  30px black;
    text-align: center;
    z-index: 100;
    border-radius: 7px;
}

.bag{
       width: 100% !important;
       height: 100%;
       background-color: rgba(43, 38, 38, 0.481);
}
.btn{
    position: absolute;
    bottom: 10px;
    right: 10px;
}
</style>