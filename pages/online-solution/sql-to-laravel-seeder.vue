<template>
    <div>
        <BreadCrumb/>
        <ContentHeader/>
        <OnlineDescription/>

        <div class="boxes">

            <div class="sql-box">
                <label for="sql">SQL:</label>
                <textarea id="sql" name="sql" class="sql" rows="10" cols="50"> </textarea>
                <button> Generate</button>
            </div>


            <div class="migration-box">
                <label for="migration">Seeder:</label>
                <textarea id="migration" name="migration" class="migration" rows="10" cols="50"> </textarea>
                <button> Download</button>
            </div>

        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>

    textarea.sql, textarea.migration {
        border: 1px solid #EBEBE4;
        width: 100%;
        border-radius: 5px;
    }

    .boxes {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
    }


    .sql-box button {
        background: #EBEBE4;
        padding: 5px;
        border-radius: 2px;
        text-align: right;
        float: right;
        color: #696969;
    }

    .migration-box button {
        background: cornflowerblue;
        padding: 5px;
        border-radius: 2px;
        text-align: right;
        float: right;
        color: #fff;
    }

    @media (min-width: 1025px) {
        .boxes {
            flex-direction: row;
            justify-content: space-between;
        }

        .boxes > div {
            flex-basis: 48%;
        }

    }

</style>
