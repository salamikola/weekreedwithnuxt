<template>
    <div>
        <BreadCrumb/>
        <ContentHeader/>
        <OnlineDescription/>

        <div class="boxes">

            <div class="json-box">
                <label for="json">JSON:</label>
                <textarea id="json" name="json" class="json" rows="10" cols="50"> </textarea>
                <button> Generate</button>
            </div>


            <div class="typehint-box">
                <label for="typehint">PHP TYPEHINT PROPERTY:</label>
                <textarea id="typehint" name="typehint" class="typehint" rows="10" cols="50"> </textarea>
            </div>

        </div>
    </div>
</template>

<script setup>
</script>

<style scoped>

    textarea.json, textarea.typehint {
        border: 1px solid #EBEBE4;
        width: 100%;
        border-radius: 5px;
    }

    .boxes {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
    }


    .json-box button {
        background: #EBEBE4;
        padding: 5px;
        border-radius: 2px;
        text-align: right;
        float: right;
        color: #696969;
    }

    .typehint-box button {
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
