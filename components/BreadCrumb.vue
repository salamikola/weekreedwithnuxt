<template>
    <div class="breadcrumb">
        <ul>
            <li><a href=""> Home </a></li>
            <li><a href=""> Page Section </a></li>
            <li><a href=""> Page Details </a></li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: "BreadCrumb"
    }
</script>

<style scoped>

    div.breadcrumb {
        padding-bottom: 1.5rem;
    }

    div.breadcrumb ul li {
        display: inline;
        margin-right: 5px;
        color: cornflowerblue;
    }

    div.breadcrumb ul li:after {
        content: '>';
        font-weight: 900;
    }

    div.breadcrumb ul li:last-child {
        color: #EBEBE4
    }

    div.breadcrumb ul li:last-child:after {
        content: '';
    }
</style>
