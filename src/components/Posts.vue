<template>
    <div>

        <v-row class="ma-3 mb-3">
            <v-col cols="3" v-for="post in posts" :key="post.id" class="mb-3">
                <v-card
                        class="mx-auto"
                        elevation="20"
                >
                    <v-card-text class="fnt-vaz">
                        <div class="text-center text--primary">{{post.title}}</div>
                        <div class="text-justify fnt-s-12">
                            {{post.content}}
                        </div>
                    </v-card-text>
                    <v-divider></v-divider>
                    <v-card-actions class="pa-0">
                        <v-col class="text-center" cols="3">
                            <v-btn icon color="gray" small>
                                <v-icon dense small>mdi-telegram</v-icon>
                            </v-btn>
                        </v-col>
                        <v-col class="text-center" cols="3">
                            <v-btn icon color="gray" small>
                                <v-icon dense small>mdi-heart-outline</v-icon>
                            </v-btn>
                        </v-col>
                        <v-col class="text-center" cols="3">
                            <v-btn icon color="gray" small>
                                <v-icon dense small>mdi-instagram</v-icon>
                            </v-btn>
                        </v-col>
                        <v-col class="text-center" cols="3">
                            <v-btn icon color="gray" small>
                                <v-icon dense small>mdi-content-copy</v-icon>
                            </v-btn>
                        </v-col>
                    </v-card-actions>
                </v-card>
            </v-col>

        </v-row>
    </div>


</template>

<script>
    export default {
        name: "Posts",
        data: () => ({
            posts :[
                {
                    id:0,
                    title:"خوشبختی",
                    content:"همیشه داشتنِ چیزی نیست.\n" +
                        "\n" +
                        "گاهی خوشبختی لذت عمیق\n" +
                        "\n" +
                        "از نداشته هاست!" +
                        "«نوعی رهایی» که شبیه به هیچ چیز نیست؛ و گاهی ساده و غیرقابل تصور است",
                    author:"میم"
                },{
                    id:1,
                    title:"انسان بزرگ نمیشود",
                    content:"انسان بزرگ نمیشود\n" +
                        "\n" +
                        "جز با افڪارش،\n" +
                        "\n" +
                        "شریف نمیشود،\n" +
                        "\n" +
                        "جز با رفتارش،\n" +
                        "\n" +
                        "و قابل احترام نمیگردد\n" +
                        "\n" +
                        "جز به واسطه اعمال نیڪش...",
                    author:"میم"
                }
            ]
        }),
    }
</script>

<style scoped>
    @font-face {
        font-family: Vazir;
        src: url('/fonts/vazir/Vazir.eot');
        src: url('/fonts/vazir/Vazir.eot?#iefix') format('embedded-opentype'),
        url('/fonts/vazir/Vazir.woff2') format('woff2'),
        url('/fonts/vazir/Vazir.woff') format('woff'),
        url('/fonts/vazir/Vazir.ttf') format('truetype');
        font-weight: normal;
        font-style: normal;
    }

    @font-face {
        font-family: Vazir;
        src: url('/fonts/vazir/Vazir-Bold.eot');
        src: url('/fonts/vazir/Vazir-Bold.eot?#iefix') format('embedded-opentype'),
        url('/fonts/vazir/Vazir-Bold.woff2') format('woff2'),
        url('/fonts/vazir/Vazir-Bold.woff') format('woff'),
        url('/fonts/vazir/Vazir-Bold.ttf') format('truetype');
        font-weight: bold;
        font-style: normal;
    }

    @font-face {
        font-family: Vazir;
        src: url('/fonts/vazir/Vazir-Black.eot');
        src: url('/fonts/vazir/Vazir-Black.eot?#iefix') format('embedded-opentype'),
        url('/fonts/vazir/Vazir-Black.woff2') format('woff2'),
        url('/fonts/vazir/Vazir-Black.woff') format('woff'),
        url('/fonts/vazir/Vazir-Black.ttf') format('truetype');
        font-weight: 900;
        font-style: normal;
    }

    @font-face {
        font-family: Vazir;
        src: url('/fonts/vazir/Vazir-Medium.eot');
        src: url('/fonts/vazir/Vazir-Medium.eot?#iefix') format('embedded-opentype'),
        url('/fonts/vazir/Vazir-Medium.woff2') format('woff2'),
        url('/fonts/vazir/Vazir-Medium.woff') format('woff'),
        url('/fonts/vazir/Vazir-Medium.ttf') format('truetype');
        font-weight: 500;
        font-style: normal;
    }

    @font-face {
        font-family: Vazir;
        src: url('/fonts/vazir/Vazir-Light.eot');
        src: url('/fonts/vazir/Vazir-Light.eot?#iefix') format('embedded-opentype'),
        url('/fonts/vazir/Vazir-Light.woff2') format('woff2'),
        url('/fonts/vazir/Vazir-Light.woff') format('woff'),
        url('/fonts/vazir/Vazir-Light.ttf') format('truetype');
        font-weight: 300;
        font-style: normal;
    }

    @font-face {
        font-family: Vazir;
        src: url('/fonts/vazir/Vazir-Thin.eot');
        src: url('/fonts/vazir/Vazir-Thin.eot?#iefix') format('embedded-opentype'),
        url('/fonts/vazir/Vazir-Thin.woff2') format('woff2'),
        url('/fonts/vazir/Vazir-Thin.woff') format('woff'),
        url('/fonts/vazir/Vazir-Thin.ttf') format('truetype');
        font-weight: 100;
        font-style: normal;
    }

    .fnt-vaz {
        font-family: Vazir, sans-serif;
    }

    .fnt-s-12{
        font-size: 12px;
        letter-spacing: normal;
    }

</style>