<template>
    <div class="intro">
        <div id="content" class="media">
            <div class="media-content" id="wrap-text">
                <p id="headingOne" class="is-size-4">
                    SKILLS
                </p>
                <br>
                <br>
                <div class="columns">
                    <div class="column">
                        <p class="is-size-6">
                            <strong>LANGUAGES</strong>
                        </p>
                        <p id="languagelist" class="is-size-6">
                            Javascript
                        </p>
                        <p id="languagelist" class="is-size-6">
                            HTML
                        </p>
                        <p id="languagelist" class="is-size-6">
                            CSS
                        </p>
                        <p id="languagelist" class="is-size-6">
                            Java
                        </p>
                        <p id="languagelist" class="is-size-6">
                            Python
                        </p>
                    </div>
                    <div class="column">
                        <p class="is-size-6">
                            <strong>FRAMEWORKS</strong>
                        </p>
                        <p id="languagelist" class="is-size-6">
                            Vue
                        </p>
                        <p id="languagelist" class="is-size-6">
                            React
                        </p>
                        <p id="languagelist" class="is-size-6">
                            React Native
                        </p>
                        <p id="languagelist" class="is-size-6">
                            Node
                        </p>
                        <p id="languagelist" class="is-size-6">
                            Express
                        </p>
                    </div>
                    <div class="column">
                        <p class="is-size-6">
                            <strong>TECHNOLOGIES</strong>
                        </p>
                        <p id="languagelist" class="is-size-6">
                            Git & Github
                        </p>
                        <p id="languagelist" class="is-size-6">
                            MongoDB
                        </p>
                        <p id="languagelist" class="is-size-6">
                            Postman
                        </p>
                        <p id="languagelist" class="is-size-6">
                            Bash
                        </p>

                    </div>
                    <div class="column">

                    </div>
                </div>
                <br>
                <br>

                <br>

            </div>

            <div class="media-right">
                <img id="emoji" src="../assets/mac.jpeg" />
            </div>
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
