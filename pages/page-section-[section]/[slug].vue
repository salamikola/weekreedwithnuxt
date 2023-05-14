<template>
    <div>
        <div>
            <BreadCrumb/>
            <ContentHeader/>
            <div class="content-body">
                <div v-html="rawHtml"></div>
            </div>
            <div class="content-tags">
                <h6> Tags </h6>
                <span> #software development </span> <span> #cyber security </span> <span> #web </span>
            </div>
            <div class="content-divider">
                <hr/>
            </div>
            <div>
                <ReadNext/>
            </div>
        </div>
    </div>
</template>

<script setup>
    import {ref} from 'vue';

    const rawHtml = ref("<p>&nbsp;</p>\n" +
        "\n" +
        "<p>Media Query is a popular technique that enables to deliver a style sheet to different devices which have different screen sizes and resolutions respectively. They are used to customize the appearance of a website on multiple devices. A media query consist of a media type that can contain one or more expression which can be either true or false. The result of the query is true if the specified media matches the type of device the document is displayed on. If the media query is true then the style sheet is applied.</p>\n" +
        "\n" +
        "<p>The screen resolutions of different devices are listed below:</p>\n" +
        "\n" +
        "<ul>\n" +
        "\t<li>Mobile (Smartphone) max-width: 480px</li>\n" +
        "\t<li>Low Resolution Tablets and ipads max-width: 767px</li>\n" +
        "\t<li>Tablets Ipads portrait mode max-width:1024px</li>\n" +
        "\t<li>Desktops max-width:1280px</li>\n" +
        "\t<li>Huge size (Larger screen) max-width: 1281px and greater</li>\n" +
        "</ul>\n" +
        "\n" +
        "<p>&nbsp;</p>\n" +
        "\n" +
        "<p><a href=\"https://www.tiny.cloud/images/homepage/features/wow/media@1x.png\"><img alt=\"\" src=\"https://www.tiny.cloud/images/homepage/features/wow/media@1x.png\" style=\"height:286px; width:454px\" /></a></p>\n" +
        "\n" +
        "<p>&nbsp;</p>");

</script>

<style scoped>

    div.content-divider {
        padding-bottom: 2rem;
    }

    div.content-tags {
        display: flex;
        justify-content: flex-start;
        flex-wrap: wrap;
        padding-bottom: 2rem;
    }

    div.content-tags h6 {
        flex-basis: 100%;
        font-weight: 600;
    }

    div.content-tags span {
        margin-right: 10px;
        font-size: 14px;
    }


    @media (min-width: 1025px) {

        div.content-tags {
            display: flex;
            justify-content: flex-end;
            flex-wrap: wrap;
        }

        div.content-tags h6 {
            flex-basis: 100%;
            text-align: end;
        }

        div.content-tags span {
            margin-right: 0;
            margin-left: 10px;
        }

    }

</style>
