<template>
    <div>
        <div>
<!--            <BreadCrumb/>-->
            <div class="content-body">
                <div v-html="rawHtml"></div>
            </div>
        </div>
    </div>
</template>

<script setup>
    import {ref} from 'vue';

    const rawHtml = ref("<p>&nbsp;</p>\n" +
        "\n" +
        "<p>&nbsp;</p>\n" +
        "\n" +
        "<p>&nbsp;</p>\n" +
        "\n" +
        "<ul>\n" +
        "\t<li><strong>WHO THE HELL ARE YOU?</strong><br />\n" +
        "\t<br />\n" +
        "\tWell since you asked. My name is Salami Kolawole, I am from Nigeria&nbsp;and I earn my daily bread through software development. Throughout my career, I have had the opportunity to work on various projects, ranging from open-source initiatives to enterprise solutions. As a leader, I have successfully guided teams of 5-10 members through one, two, three, four, five&nbsp;product launches, spanning various domains.<br />\n" +
        "\t&nbsp;</li>\n" +
        "\t<li><strong>HOW DID YOU BECOME A SOFTWARE ENGINEER?</strong><br />\n" +
        "\t<br />\n" +
        "\tIt all started in 2016, I was mandated to take a course in programming during my graduate program. While in the lecture room on a sunny Friday, the lecturer said 95% percent of you in this room will never end up as a programmer, just cram and pass the goddamn course. That statement really skyrocketed my interest in programming, I picked up my laptop days after, head to youtube, and search for FORTRAN FOR BEGINNERS. I never looked back afterward. A year later I picked up web development, so here I am.<br />\n" +
        "\t&nbsp;</li>\n" +
        "\t<li><strong>DO YOU HAVE A JOB AND WHAT DO YOU DO AT YOUR JOB?</strong><br />\n" +
        "\tSure, I do have an employer, I work at VALE. You can check us out @ <a href=\"https://vale.ng\">https://vale.ng</a><br />\n" +
        "\tI do wear many hats and they all fit. Most of the time you will find hacking away the backend side of things, I do dabble in front-end engineering too, but I do respect my boundaries. Catch me goofing around with DevOps-related tasks at odd hours too.<br />\n" +
        "\tArchitectural design? Yeah, I am always discussing trade-offs.</li>\n" +
        "</ul>\n" +
        "\n" +
        "<p>&nbsp;</p>\n" +
        "\n" +
        "<ul>\n" +
        "\t<li><strong>WHAT DO YOU LOVE ABOUT BEING A SOFTWARE DEVELOPER?</strong><br />\n" +
        "\t<br />\n" +
        "\tNothing actually, it&#39;s just a profession where you are a beginner at something new every 3 months.</li>\n" +
        "</ul>\n" +
        "\n" +
        "<p>&nbsp;</p>\n" +
        "\n" +
        "<ul>\n" +
        "\t<li><strong>WHAT DO YOU REGARD AS&nbsp;AN IDEAL SOFTWARE?</strong><br />\n" +
        "\t<br />\n" +
        "\tA software that does not exist is my ideal software.&nbsp; Hello World application comes a distant second.<br />\n" +
        "\t<br />\n" +
        "\tErmm sorry, I have to&nbsp;go now, there&#39;s a crash in production. I need to start taking testing seriously.&nbsp;</li>\n" +
        "</ul>");

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
