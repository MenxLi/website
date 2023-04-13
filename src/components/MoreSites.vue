
<script>
    const sites = [
        {
            site_name: "Github",
            site_url: "https://github.com/MenxLi"
        },
        {
            site_name: "Bilibili",
            site_url: "https://space.bilibili.com/2031376"
        },
    ];
    export default {
        mounted(){
            let div = document.querySelector("div.sites");
            for (const site of sites){
                const link = document.createElement("a");
                link.href = site.site_url;
                link.text = site.site_name;
                div.appendChild(link);
            }
        }
    }
</script>

<template>
    <div class="other_site">
        <h3>More</h3>
        <div class="sites">
        </div>
    </div>
</template>

<style scoped>
div.sites{
    width: 110px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
</style>