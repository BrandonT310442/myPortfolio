<template>
    <div class="intro">
        <div id="content" class="media">
            <div class="media-content" id="wrap-text">
                <p id="headingOne" class="is-size-4">
                    SKILLS
                </p>
                <br>
                <br>

            </div>
            <br>
            <br>

            <br>

        </div>

        <div class="media-right">
            <img id="emoji" src="../assets/mac.jpeg" />
        </div>
    </div>
</template>

<script>
export default {

}
</script>
<style scoped>
#headingOne {
    color: #007bff;
    font-family: "Work Sans", sans-serif;
    font-weight: 600;
    letter-spacing: .2rem;
    text-decoration: underline;
    text-underline-offset: 10px;
}



#wrap-text {
    margin-top: 100px;
    margin-right: 50px;
    z-index: 1.0;
    transform: translateX(10%);
}

#emoji {
    width: 300px;
    height: 300px;
    margin-top: 50px;
    position: absolute;
    right: 5px;
    z-index: 1;

}

#languagelist {
    margin-top: 10px;
}
</style>
