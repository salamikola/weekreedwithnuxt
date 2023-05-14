<template>
    <div>
        <div class="page-item-list">
            <ul>
                <li>
                    <a href=""> <img src="~/assets/images/file.png" alt="file"/>  IC-Project-Plan-Template-8538-V1.xlsx
                    </a>
                </li>
                <li>
                    <a href=""> <img src="~/assets/images/file.png" alt="file"/> Cracking the Coding Interview.pdf </a>
                </li>
                <li>
                    <a href=""> <img src="~/assets/images/file.png" alt="file"/>
                        Black-LinkedIn-icon-in-flat-design-on-transparent-PNG.png </a>
                </li>
                <li>
                    <a href=""> <img src="~/assets/images/file.png" alt="file"/> IC-Project-Plan-Template-8538-V1.xlsx
                    </a>
                </li>
                <li>
                    <a href=""> <img src="~/assets/images/file.png" alt="file"/> IC-Project-Plan-Template-8538-V1.xlsx
                    </a>
                </li>
                <li>
                    <a href=""> <img src="~/assets/images/file.png" alt="file"/> IC-Project-Plan-Template-8538-V1.xlsx
                    </a>
                </li>
                <li>
                    <a href=""> <img src="~/assets/images/file.png" alt="file"/> IC-Project-Plan-Template-8538-V1.xlsx
                    </a>
                </li>
            </ul>
        </div>
        <div class="pagination">
            <button>  Load More </button>
        </div>
    </div>
</template>

<script>
    export default {
        name: "[slug]"
    }
</script>

<style scoped>
    div.page-item-list > ul {
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
    }

    div.page-item-list > ul > li {
        margin-bottom: 25px;
    }

    div.page-item-list ul li img {
        width: 40px;
        height: 40px;
        display: inline;
    }

    div.page-item-list ul li a span {
        width: 40px;
    }

    div.pagination{
        display: flex;
        justify-content: center;
    }
    div.pagination button{
        box-sizing: content-box;
        padding: 5px;
        border: 1px solid black;
    }

    @media (min-width: 1025px){
        div.page-item-list > ul {
            display: flex;
            flex-wrap: wrap;
            flex-direction: row;
            justify-content: flex-start;
        }

        div.page-item-list > ul > li {
            width: 33%;
        }
    }


</style>
