
<script>
    export default {
        data(){
            return {
                pubs: [
                    {
                        content: "Li, M., Punithakumar, K., Major, P. W., Le, L. H., Nguyen, K. C. T., Pacheco-Pereira, C., ... & Almeida, F. T. (2022). Temporomandibular joint segmentation in MRI images using deep learning. Journal of Dentistry, 127, 104345.",
                        url: "https://limengxun.com:8080/doc/79939b8d-3b5e-424c-8bec-cf44e401b19f"
                    },
                    {
                        content: "Li, M., Xu, X., Punithakumar, K., Le, L.H., Kaipatur, N. and Shi, B., 2020. Automated integration of facial and intra-oral images of anterior teeth. Computers in Biology and Medicine, p.103794. ",
                        url: "https://limengxun.com:8080/doc/48ef21bc-5178-4676-b4ad-d03b4f1aad1b"
                    },
                    {
                        content: "Chifor, R., Li, M., Nguyen, K. C. T., Arsenescu, T., Chifor, I., Badea, A. F., ... & Le, L. H. (2021). Three-dimensional periodontal investigations using a prototype handheld ultrasound scanner with spatial positioning reading sensor. Medical Ultrasonography, 23(3), 297-304.",
                        url: "https://limengxun.com:8080/doc/ce59387a-d79b-4d06-be60-767edb588ea7"
                    },
                    {
                        content: "Li, M.X., Xing, X., Li, Z.B. and Li, Z., 2021. Classification and treatment strategies for condylar fractures in children. British Journal of Oral and Maxillofacial Surgery, 59(7), pp.776-782. ",
                        url: "https://limengxun.com:8080/doc/b21b0fe3-4b7d-444d-b0e6-ddb1e159c4fa"
                    },
                    {
                        content: "Nguyen, K. C. T., Le, B. M., Li, M., Almeida, F. T., Major, P. W., Kaipatur, N. R., ... & Le, L. H., 2021. Localization of cementoenamel junction in intraoral ultrasonographs with machine learning. Journal of Dentistry, 112, 103752.",
                        url: "https://limengxun.com:8080/doc/2c267924-a769-4e76-b5cf-711b4761c42a"
                    },
                    {
                        content: "Zeng, H., Pathak, J.L., Shi, Y., Ran, J., Liang, L., Yan, Q., Wu, T., Fan, Q., Li, M. and Bai, Y., 2020. Indirect selective laser sintering-printed microporous biphasic calcium phosphate scaffold promotes endogenous bone regeneration via activation of ERK1/2 signaling. Biofabrication, 12(2), p.025032.",
                        url: ""
                    },
                ]
            }
        }
    }
</script>

<template>
    <div class="publications">
            <h3 class="subtitle">Publications</h3>
            <ul>
                <li v-for="pub in pubs">
                    {{ pub.content }} <label v-if="pub.url">[<a v-bind:href="pub.url">file</a>]</label>
                </li>
            </ul>

        </div>
</template>

<style scoped>
div.publications{
    max-width: 100vw;
}
li{
    text-align:justify;
    line-height: 145%;
    margin-bottom: 10px
}
</style>
