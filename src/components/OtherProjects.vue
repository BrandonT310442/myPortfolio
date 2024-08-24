<template>
    <div class="intro" id="wrap-text">
        <p id="headingOne" class="is-size-4">
            OTHER NOTEWORTHY PROJECTS
        </p>
    </div>
    <br>
    <br>

    <div class="columns is-variable is-4">
        <div class="column is-one-third">
            <div class="card custom-card">
                <div class="card-content">
                    <div class="content">
                        Lorem ipsum leo risus, porta ac consectetur ac, vestibulum at eros. Donec
                        id elit non mi porta gravida at eget metus. Cum sociis natoque penatibus
                        et magnis dis parturient montes, nascetur ridiculus mus. Cras mattis
                        consectetur purus sit amet fermentum.
                    </div>
                </div>
            </div>
        </div>
        <div class="column is-one-third">
            <div class="card custom-card">
                <div class="card-content">
                    <div class="content">
                        Lorem ipsum leo risus, porta ac consectetur ac, vestibulum at eros. Donec
                        id elit non mi porta gravida at eget metus. Cum sociis natoque penatibus
                        et magnis dis parturient montes, nascetur ridiculus mus. Cras mattis
                        consectetur purus sit amet fermentum.
                    </div>
                </div>
            </div>
        </div>

        <div class="column is-one-third">
            <div class="card custom-card">
                <div class="card-content">
                    <div class="content">
                        Lorem ipsum leo risus, porta ac consectetur ac, vestibulum at eros. Donec
                        id elit non mi porta gravida at eget metus. Cum sociis natoque penatibus
                        et magnis dis parturient montes, nascetur ridiculus mus. Cras mattis
                        consectetur purus sit amet fermentum.
                    </div>
                </div>
            </div>
        </div>
    </div>
    <br>
    <br>

    <br>
    <br>

    <br>
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

.card {
    background-color: transparent;
    color: #007bff;
    border: 1.5px solid #007bff;

}

#wrap-text {
    margin-top: 100px;
    margin-right: 50px;
    z-index: 1.0;
    transform: translateX(10%);
}

.custom-card {
    max-width: 300px;
    margin: 0 auto;
}

.columns {
    margin: 0 20px;
}
</style>
