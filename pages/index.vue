<script lang="ts" setup></script>

<template>
    <div>
        <div>
            <div class="flex-main-content">
                <div class="flex-folder-parent">
                    <div class="flex-folder">
                        <nuxt-link to="/"><img src="~/assets/images/grey-fold.png"/> Online Solution</nuxt-link>
                        <nuxt-link to="/"><img src="~/assets/images/grey-fold.png"/> Packages</nuxt-link>
                        <nuxt-link to="/"><img src="~/assets/images/grey-fold.png"/> Projects</nuxt-link>
                        <nuxt-link to="/"><img src="~/assets/images/grey-fold.png"/> Concepts</nuxt-link>
                        <nuxt-link to="/"><img src="~/assets/images/grey-fold.png"/> Tutorials</nuxt-link>
                        <nuxt-link to="/about-salami-kolawole"><img class="img-file" src="~/assets/images/web-file.png"
                                                                    alt="file"/> About.html
                        </nuxt-link>
                    </div>
                </div>
                <div class="flex-about">
                    <img class="profile-pic" src="~/assets/images/salami-kolawole.png" alt="salami kolawole"/>
                    <p class="about-note"> Clean design merchant but not a software purist. || Building cool stuff @
                        Vale (Formerly
                        Fundbae) </p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>


    ul {
        list-style-image: url("~/assets/images/folder.png");
    }

    div.flex-main-content {
        display: flex;
        justify-content: center
    }

    div.main-content {
        margin: 0 auto;
        width: 80%;
        max-width: 1440px;
    }

    div.main-content > div {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
    }

    ul {
        display: inline;
    }

    ul.folder-list > li {
        display: inline;
        list-style: url("~/assets/images/folder.png");
    }

    a > img {
        width: 50px;
        height: 50px;
    }

    .flex-folder {
        display: flex;
        flex-wrap: wrap;
        justify-content: left;
    }

    div.flex-folder > a {
        margin: 10px;
        flex-grow: 0;
        flex-basis: 0;
        min-width: 90px;
    }

    .flex-folder-parent {
        max-width: 500px;
    }

    div.flex-about img {
        width: 200px;
        height: 200px;
        border-radius: 100px;
    }

    div.flex-about {
        text-align: center;
    }

    p.about-note {
        max-width: 200px;
    }

    img.img-file {
        width: 50px;
        height: 50px;
    }

    @media only screen and (max-width: 600px) {

        div.flex-main-content {
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        p.about-note {
            max-width: 100%;
        }

        img.profile-pic {
            display: inline;
        }

        div.flex-folder > a {
            margin: 10px;
            flex-grow: 1;
            flex-basis: 0;
            min-width: 70px;
        }
    }
</style>
