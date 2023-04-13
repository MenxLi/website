
<script>
    export default {
        data(){
            return {
                profilePhotoSrc: "http://limengxun.com/imgs/profile_photo.jpg"
                // profilePhotoSrc: "assets/profile_photo.jpg"
            }
        }
    }
</script>

<template>
    <div class="short_intro">
        <img src="../assets/profile_photo.jpg" alt="" id="portrait">
        <div class="text">
                <!-- <div id="full_name">
                    About me
                </div> -->
                <h3 class="subtitle">About me</h3>
                <hr>

                <div class="gradIn">
                    <p>
                    I got my Doctor of Medicine degree in Dentistry from Wuhan University in June, 2021. <br>
                    </p>
                    <p>
                        Currently, I'm a dentist in the Department of Prosthodontics, School of Stomatology in Wuhan University. <br>
                        I'm also a researcher and I work with the <a href="http://www.captain-whu.com/team_En.html">CAPTAIN team</a>. 
                        My research interests are focused on the application of computer methods in dentistry.
                    </p>
                    <p>
                        Email: <a href="mailto:mengxunli@whu.edu.cn?subject=Hello from your webpage">mengxunli@whu.edu.cn</a>
                    </p>
                </div>
        </div>
    </div>
</template>

<style scoped>
div#full_name {
    font-family: Arial, "MS Trebuchet", sans-serif;
    font-size: larger;
    font-weight:bolder;
}
div.short_intro {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;

    justify-content: center;
    align-items: center;
}
div.short_intro div.text {
    flex: 3;
    min-width: 400px;
    /* margin: 10px; */
    word-wrap: break-word;
    /* text-align:justify; */
}

#portrait{
    flex: 1;
    margin: 10px;
    width: 180px;
    max-width: 50vw;
}
</style>