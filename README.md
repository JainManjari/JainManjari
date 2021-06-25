<link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css"
/>

<style>
    @import url('https://fonts.googleapis.com/css2?family=EB+Garamond&display=swap');

    :root
    {
        --animate-duration: 2.2s;
        --animate-delay: 1.2s;
    }

    .body
    {
        background: linear-gradient(to bottom,#F08331,#88D06D);
        height:inherit;
        min-height:500px;
        width:100%;
        padding:10px 5px 10px;
        color:snow;
    }
    .header
    {
        text-align:center;
        display:block;
        margin-bottom:15px;
        font-family: 'EB Garamond', serif;
        
    }
    .header a
    {
        color:darkslategrey;
        background:lightgreen;
        border:1.8px solid slategrey;
        padding:4px;
        border-radius:13px 0px 13px 0px;
        font-size:19px;
        transition:all ease-in 0.6s;
    }
    .header a:hover
    {
        text-decoration:none;
        color:black;
        border-color:darkslategrey;
    }

    .intro
    {
        display:flex;
        justify-content:space-between;
        min-height:300px;
        border:1px solid;
        margin:0px auto 10px;
        flex-wrap:wrap;
        width:85%;
    }

    .intro .img-container
    {
        width:250px;
        min-height:100%;
        border:1px solid;
        display:flex;
        justify-content:center;
        align-items:center;
    }
    .intro .img-container img
    {
        width:200px;
        height:300px;
    }
</style>


<div class="body">
     <h2 class="header animate__animated  animate__fadeInDown">
            Namaste! I am Manjari Jain <span style="font-family:serif;">-</span> <a href="http://www.thehindflora.com">TheHindFlora</a>
    </h2>
    <div class="intro">
       <div>
       </div>
       <div class="img-container">
           <img src="designer.gif">
       </div>
    </div>
    <div>
        <a href="https://github.com/JainManjari">
            <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=JainManjari&layout=compact&show_icons=true&theme=buefy" />
        </a>
        <a href="https://github.com/JainManjari">
            <img src="https://github-readme-stats.vercel.app/api?username=JainManjari&hide=prs&layout=compact&show_icons=true&theme=buefy" />
        </a>
    </div>
</div>