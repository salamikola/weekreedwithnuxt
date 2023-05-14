<template>
    <div class="content-header">
        <div class="content-title">
            <h3> Database SQL to Laravel Migration </h3>
            <p> A 3 minutes read</p>
        </div>
        <div class="content-author">
            <img class="profile-pic" src="~/assets/images/salami-kolawole.png" alt="profile-pic"/>
            <div class="author-text">
                <h6> Salami Kolawole</h6>
                <p> Clean design merchant but not a software purist. || Building cool stuff @ Vale (Formerly
                    Fundbae) </p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "ContentHeader"
    }
</script>

<style scoped>

    .profile-pic {
        width: 50px;
        height: 50px;
        border-radius: 50px;
        margin-right: 5px;
    }

    div.content-header {
        padding-bottom: 1.5rem;
    }

    div.content-title {
        padding-bottom: 1.5rem;
    }

    div.content-header h3 {
        font-style: normal;
        text-transform: uppercase;
        text-align: center;
        font-weight: 600;
        font-size: 24px;
    }

    div.content-title > p {
        text-transform: uppercase;
        font-size: 10px;
        text-align: center;
        font-style: italic;
    }

    .content-author {
        display: flex;
        justify-content: flex-start;
    }

    @media (min-width: 1025px) {
        .content-author {
            display: flex;
            justify-content: flex-end;
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

    .author-text {
        flex-basis: 70%;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
    }

    .author-text h6 {
        font-weight: 500;
    }

    .author-text p {
        font-size: 12px;
    }
</style>
