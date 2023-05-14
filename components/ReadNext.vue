<script lang="ts" setup>

</script>

<template>
    <div class="read-next-header">
        <h6> Read Next </h6>
        <div class="page-item-list">
            <ul>
                <li>
                    <a href=""> <img src="~/assets/images/file.png" alt="file"/> IC-Project-Plan-Template-8538-V1.xlsx
                    </a>
                </li>
                <li>
                    <a href=""> <img src="~/assets/images/file.png" alt="file"/> Cracking the Coding Interview.pdf </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style scoped>

    div.read-next-header > h6{
        font-weight: 600;
        padding-bottom: 1rem;
    }

    div.page-item-list > ul {
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
    }

    div.page-item-list > ul > li {
        margin-bottom: 25px;
        font-size: 14px;
    }

    div.page-item-list ul li img {
        width: 20px;
        height: 20px;
        display: inline;
    }
</style>
