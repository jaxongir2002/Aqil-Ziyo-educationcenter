<template>
    <div class="footer">
        <div class="footer_one container d-flex justify-content-between">
            <div class="my_white_logo w-25">
                <img src="@/assets/img/AZ-LOGO.png" alt="" >
            </div>
            <div class="s_medias d-flex">
                <div class="my_icon_group">
                    <box-icon class="my_icon" name='instagram' type='logo'  color='white'></box-icon>
                </div>
                <div class="my_icon_group facebookHover">
                    <box-icon class="my_icon" type='logo' name='facebook' color='white'></box-icon>
                </div>
                <div class="my_icon_group twitterHover">
                    <box-icon class="my_icon" type='logo' name='twitter' color='white'></box-icon>
                </div>
                <div class="my_icon_group telegramhover">
                    <box-icon class="my_icon" name='telegram' type='logo' color='white' ></box-icon>
                </div>
                
            </div>
        </div>
        <hr class="hr container" style="color: white;">

        <div class="footer_two container d-flex">
            <div class="footer_menu w-75">
                <h4>Company</h4>
                <ul class="fotter_media">
                    <li>
                        <a href="#">About US</a>
                    </li>
                     <li>
                        <a href="#">Press</a>
                    </li>
                     <li>
                        <a href="#">Investors</a>
                    </li>
                     <li>
                        <a href="#">Events</a>
                    </li>
                     <li>
                        <a href="#">Team of use</a>
                    </li>
                     <li>
                        <a href="#">Privacy policy</a>
                    </li>
                </ul>
            </div>
            <div class="footer_btn d-flex justify-content-end w-25">
                <button class="my_btn">Contact Us</button>
            </div>
        </div>  
       
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.footer{
    background-color: #26272b;
    margin-top: 10%;
}
.footer_one{
    padding: 55px 0;
}

.my_white_logo img{
    width: 100%;
    height: 100%;
}
.my_icon_group{
    width: 48px;
    height: 48px;
    background-color: darkred;
    color: white;
    border-radius: 50%;
    position: relative;
    margin: 0 7px;
    transition: .4s;
}
.my_icon_group:hover{
    background-color: #983b3b;
}
.facebookHover:hover{
    background-color: #3b5998;
}
.twitterHover:hover{
    background-color:#00aced;
}
.my_icon_group .my_icon{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
.telegramhover:hover{
    background-color:#007bb6;

}
.footer_two{
    padding: 55px 0;
}
.my_btn{
    border: none;
    background-color: darkred;
    color: white;
    border-radius: 12px;
    padding: 10px 40px;
    margin-top: 50px;
    transition: .4s;
    box-sizing: 5px 5px 60px rgba(139, 0, 0, 0.656);
}
.my_btn:hover{
    background-color: rgba(139, 0, 0, 0.802);
}
.footer_menu h4{
    color: #ccc;
}
ul{
    display: flex;
    justify-content: space-around;
    padding: 0;
    margin-top: 30px;
}
ul li{
    list-style: none;
    margin-right: auto;
}
ul li a{
    text-decoration: none;
    color: #ccc;
}

.hr{
    z-index: 2;
}
@media only screen and (max-width: 985px) {
    .my_icon_group{
        width: 40px;
        height: 40px;
        margin: 0 4px;
    }
    .my_btn{
        padding: 6px 20px;
        font-size: 14px;
    }
    .footer_menu h4{
        font-size: 20px;
    }
    .footer_menu ul li a{
        
        font-size: 12px;
    }
   

}
@media only screen and (max-width: 579px) {
    ul{
        flex-direction: column;
    }
    ul li {
        margin: 5px 0;
    }
    .footer_btn{
        display: flex;
        align-items: flex-end;
        z-index: 2;
    }
}
@media only screen and (max-width: 486px) {
   
    .footer{
        position: relative;
        z-index: 2;
    }
    .my_icon_group{
        width: 30px;
        height: 30px;
        margin: 0 3px;
        z-index: 2;
    }
    .hr{
        display: none;
    }
    .footer::after{
        content: '';
        position: absolute;
        top: 0;
        right: -19px;
        clip-path: inset(0 0 1% 65%);
        background-color: #2E3E5C;
        width: 60px;
        height: 101%;
        z-index: 0;
    }
    .footer_btn{
        width: 50% !important;
        display: flex;
        align-items: flex-end !important;
    }
    p{
        z-index: 10 !important;
    }
}
</style>