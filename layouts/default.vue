<script lang="ts" setup></script>

<template>
    <div>
        <div class="main">
            <div class="text-center p-10 font-cursive">
                <span class="text-[36px]">  WeekReed  </span>
            </div>
            <div id="content-wrap">
                <slot/>
            </div>
            <footer class="absolute bottom-0 w-full footer">
                <div>
                    <div>
                        <div class="mb-10 flex items-center justify-center w-full">
                            <hr class="w-[40%]"/>
                            <p class="mr-5 ml-5"> weekreed </p>
                            <hr class="w-[40%]"/>
                        </div>
                        <div class="flex justify-around flex-wrapper">
                            <div class="flex-none toggle">
                                    <input type="checkbox" id="toggle"  >
                                    <label for="toggle"></label>
                                    <span class="slider round"></span>
                                <span> © 2022 WeekReed </span>
                            </div>
                            <div class="flex-initial flex-list">
                                <ul class="footer-list">
                                    <li> Tutorials</li>
                                    <li> Online Solutions</li>
                                    <li> Articles</li>
                                    <li> Packages</li>
                                    <li> Projects</li>
                                </ul>
                            </div>
                            <div class="flex-initial flex-initial-icon">
                                <img src="~/assets/images/socials/twitter.png" alt="twitter"/>
                                <img src="~/assets/images/socials/linkedin.png" alt="linked"/>
                                <img src="~/assets/images/socials/github.png" alt="facebook"/>
                            </div>
                        </div>
                    </div>
                </div>
            </footer>
        </div>
    </div>
</template>

<style scoped>

    #content-wrap {
        padding-bottom: 10.5rem;
    }

    .footer{
        height: 8.5rem;
    }
    .main {
        min-height: 100vh;
        margin: 0 auto;
        width: 80%;
        max-width: 1440px;
        position: relative;
    }

    .flex-list {
        width: 45%
    }

    .footer-list > li {
        display: inline;
        margin-right: 5px;
    }

    .flex-wrapper {
        display: flex;
        flex-wrap: wrap;
        padding-bottom: 10px;
    }

    div.flex-initial-icon {
        display: flex;
    }

    div.flex-initial-icon img {
        width: 20px;
        height: 20px;
        margin-right: 10px;
    }

    .toggle input[type=checkbox] {
        display: none;
    }

    .toggle label {
        background-color: #777;
        border: 2px solid #555;
        border-radius: 50px;
        cursor: pointer;
        display: inline-block;
        position: relative;
        transition: all ease-in-out 0.3s;
        width: 50px;
        height: 20px;
    }

    .toggle label::after {
        background-color: #555;
        border-radius: 50%;
        content: ' ';
        cursor: pointer;
        display: inline-block;
        position: absolute;
        left: -17px;
        top: 2px;
        transition: all ease-in-out 0.3s;
        width: 12px;
        height: 12px;
    }

    .toggle label::before {
        border-radius: 50%;
        content: ' ';
        cursor: pointer;
        display: inline-block;
        position: absolute;
        left: 2px;
        top: 2px;
        transition: all ease-in-out 0.3s;
        width: 12px;
        height: 12px;
    }

    .toggle input[type=checkbox]:checked ~ label {
        background-color: #00a0fc;
        border-color: #006dc9;
    }

    .toggle input[type=checkbox]:checked ~ label::after {
        background-color: #0054B0;
        transform: translateX(50px);
    }

    @media only screen and (max-width: 600px) {
        div.flex-list {
            width: 100%;
        }
    }


</style>
