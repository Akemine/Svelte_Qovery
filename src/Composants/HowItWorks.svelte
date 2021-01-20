<script></script>

<main>
    <div class="myDiv">
    <h1 style="color: #454658" >How does it work?</h1>
    <p class="textWidth" style="color: #454658">Qovery Engine is an open-source abstraction layer product that 
            turns easy apps deployment on AWS, GCP, Azure and others Cloud providers. The Qovery Engine is 
            coded in Rust and takes advantage of Terraform, Helm, Kubectl, Docker to manage resources.</p>
    <img class="img" src="img/policies.svg" alt="illustration">
    </div>
</main>

<style>

    @media screen and (max-width: 2200px) {

        .img{
            width: 74%; 
        }
        .myDiv{
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .textWidth{
            width:45%;
        }

        main{
           background-color: whitesmoke;
       }
    }

   @media screen and (max-width: 800px) {
    main{
           background-color: green;
       }
    }
</style>