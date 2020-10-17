<template>
    <div class="container-fluid">
        <div class="row-12 h-100 d-flex flex-column justify-content-center">
            <div class="col ml-md-5 ml-l-5 ml-sm-0 ml-xs-0 d-flex flex-column justify-content-center about-text">
                <h1>Hello, I'm Mahamed!</h1>
                <h2>A software developer</h2>
                
                <p>Who likes to code</p>
                <span>
                    <a href="#" class="btn">Get to know me</a>
                </span>
            </div>
        </div>
    </div>
</template>

<style scoped>
.about-text {
    margin-top: -23rem;
}

@media only screen and (max-width: 600px) {
  .about-text {
    margin-top: -15rem;
  }
}

h1 {
    font-weight: 300;
    font-size: 3.4rem;
}

h2 {
    font-weight: 300;
    font-size: 3rem;
}

p {
    font-weight: 200;
    font-size: 1.4rem;
}

a {
    border: 1px solid black;
}

</style>