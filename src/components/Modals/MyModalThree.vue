<template>
    <div class="bag play_confirm">
        <div class="play_confirm">
        <h1>Ushbu kurs haqida 3</h1>
        <p>Ipsum dolor sit amet consectetur adipisicing elit. Rerum earum dolorum quam sed eaque fugiat unde ratione, commodi consequatur quaerat excepturi vitae, veniam distinctio minima officiis animi provident cupiditate vero!</p>
        <button @click="$emit('closeModalThree')" class="btn btn-danger">Close</button>
    </div></div>
    

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
@media (max-width: 1000px) {

.bag{
   width: 100% !important;
   height: 500% !important;
   background-color: rgba(43, 38, 38, 0.481);

}
.play_confirm{

width: 300px;
height: 250px;


}

}
</style>