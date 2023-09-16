
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&display=swap');

  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    scroll-behavior: smooth;
    font-family: 'Poppins', sans-serif;
  }

  :root{
    --bg-color: #1c1c1c;
    --second-bg-color: #101010;
    --text-color: #ededed;
    --main-color: #00ff7f;

}

html {
font-size: 62.5%;

}

body{
    background-color: var(--bg-color);
    color: var(--text-color);

}

.header{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 2rem 9%;
    display: flex;
    background-color: transparent;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}

.logo{
    font-size: 2.5rem;
    color: var(--text-color);
    font-weight: 600;
}

.navbar a {
    font-size: 1.7rem;
    color: var(--text-color);
    font-weight: 500;
    margin-left: 3.5rem;
    transition: .3s ease-in-out;
}

.navbar a:hover, .navbar a.active {
    color: var(--main-color);
}

#menu-icon{
    font-size: 3.6rem;
    color: var(--text-color);
    cursor: pointer;
    display: none;
}

section{
    min-height: 100vh;
    padding: 10rem 9% 2rem;
}

.home{
    display: flex;
    align-items: center;
    padding:0 9%;

}

.home-content{
    max-width: 60rem;
}

.home-content h1{
font-size: 5.6rem;
font-weight: 700;
line-height: 1.3;
}

.home-content .text-animate{
    position: relative;
    width: 43rem;
}

.home-content .text-animate h3{
    font-size: 3.2rem;
    font-weight: 700;
    color: transparent;
    -webkit-text-stroke: .7px var(--main-color);
}

.home-content p{
    font-size: 1.6rem;
    margin: 2rem 0 4rem;
    max-width: 50rem;
    width: 80%; 
    text-align: justify; 
    text-justify: inter-word;
}

.btn-box{
    position: relative;
    display: flex;
    justify-content: space-between;
    width: 34.5rem;
    height: 5rem;
}

.btn-box a{
    font-size: 1.3rem;
}

.btn-box .btn{
    position: relative;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 15rem;
    height: 100%;
    background: var(--main-color);
    border-radius: 0.8rem;
    font-weight: 600;
    letter-spacing: 0.1rem;
    color: var(--bg-color);
    z-index: 1;
    overflow: hidden;
    transition: .5s;
}

.btn-box .btn:hover{
color: var(--main-color);
}

.btn-box .btn::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background: var(--bg-color);
    z-index: -1;
    transition: .5s;
}

.btn-box .btn:nth-child(2){
    background-color: transparent;
    color: var(--main-color);
}
.btn-box .btn:nth-child(2):hover{
    color: var(--bg-color);
}

.btn-box .btn:nth-child(2)::before{
    background: var(--main-color);
}

.btn-box .btn:hover::before{
    width: 100%;

}

.home-sci{
    position: absolute;
    bottom: 4rem;
    width: 170px;
    display: flex;
    justify-content: space-between;
}

.home-sci a{
    position: relative;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 40px;
    height: 40px;
    background: transparent;
    border: .2rem solid var(--main-color);
    border-radius: 50%;
    font-size: 20px;
    color: var(--main-color);
    z-index: 1;
    overflow: hidden;
    transition: background 0.3s ease-in-out;
}



.home-sci a::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;

    z-index: -1;
    transition: .5s;
}

.home-sci a:hover{

    background: var(--second-bg-color);
}

.home-sci a:hover::before{
width: 100%;
}

.home-imgHover {
    position: absolute;
    top: 0;
    right: 0;
    width: 45%;
    height: 100%;
    background: transparent;
    transition: .5s;
}

.home-imgHover:hover {
    background-color: var(--bg-color);
    opacity: .8;
}

.about{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 2rem;
    background-color: var(--second-bg-color);
    padding-bottom: 6rem;
}

.heading{
    font-size: 4rem;
    margin-bottom: 3rem;
    text-align: center;
}

span{
 color: var(--main-color);
}

.about-img {
    position: relative;
    width: 20rem;
    height: 20rem;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.about-img img{
    width: 90%;
    border-radius: 50%;
    border: .2rem solid var(--main-color);
}

.about-img .circle-spin{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%) rotate(0);
    width: 100%;
    height: 100%;
    border-radius: 50%;
    border-top: .2rem solid var(--second-bg-color);
    border-bottom: .2rem solid var(--second-bg-color);
    border-left: .2rem solid var(--main-color);
    border-right: .2rem solid var(--main-color);
}

.about-content{
    text-align: center;
}

.about-content h3{
    font-size: 2.6rem;
    margin: 1rem 0 2rem;
    
}

.about-content p{ 
    width: 100%; 
    text-align: justify; 
    text-justify: inter-word;
    font-size: 1.4rem;
    margin-bottom: 1.5rem;
}

.btn-box.btns{
    display: inline-block;
    width: 15rem;
}

.btn-box.btns a::before{
    background-color: var(--bg-color);
}

.education{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    min-height: auto;
    padding-bottom: 5rem;
}

.education .education-row{
    display: flex;
    flex-wrap: wrap;
    gap: 5rem;
}

.education-row .education-column{
    flex: 1 1 40rem;
}

.education-column .title{
    font-size: 2.5rem;
    margin: 0 0 1.5rem 2rem;
}

.education-column .education-box{
    border-left: .2rem solid var(--main-color);
}

.education-box .education-content{
    position: relative;
    padding-left: 2rem;
}

.education-box .education-content::before{
    content: '';
    position: absolute;
    top: 0;
    left: -1.1rem;
    width: 2rem;
    height: 2rem;
    background: var(--main-color);
    border-radius: 50%;
}

.education-content .content::before{
content: "";
position: absolute;
top: 0;
left: 0;
width: 0;
height: 100%;
background-color: var(--main-color);
z-index: -1;
transition: .5s;
}

.education-content .content:hover::before{

    width: 100%;
}

.education-content .content{
    position: relative;
    padding: 1.5rem;
    border: .2rem solid var(--main-color);
    border-radius: .6rem;
    margin-bottom: 2rem;
}

.education-content .content .year i{

    padding-right: 0.5rem;

}

.education-content .content h3{
    font-size: 1.5rem;
}

.education .content p{
    font-size: 1.2rem;
    padding-top: .5rem;
}

.skills{
    min-height: auto;
    padding-bottom: 7rem;
    background: var(--second-bg-color);
}

.skills .skills-row{
    display: flex;
    flex-wrap: wrap;
    gap: 5rem;
}

.skills-row .skills-column{
   flex: 1 1 40rem;
}

.skills-column .title{
    font-size: 2.5rem;
    margin: 0 0 1.5rem;
}

.skills-box .skills-content{
    position: relative;
    border: .2rem solid var(--main-color);
    border-radius: .6rem;
    padding: .5rem 1.5rem;
    z-index: 1;
    overflow: hidden;
}

.skills-box .skills-content::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background: var(--bg-color);
    z-index: -1;
    transition: .5s;
}

.skills-box .skills-content:hover::before{
    width: 100%;
}

.skills-content .progress{
    padding: 1rem 0;
}
.skills-content .progress h3{
    font-size: 1.7rem;
    display: flex;
    justify-content: space-between;
}

.skills-content .progress h3 span{
    color: var(--text-color);
}

.skills-content .progress .bar{
    height: 2.5rem;
    border-radius: .6rem;
    border: .2rem solid var(--main-color);
    padding: .5rem;
    margin: 1rem 0;
}


.skills-content .progress .bar span{
    display: block;
    height: 100%;
    border-radius: .3rem;
    background: var(--main-color);
}

.skills-column:nth-child(1) .skills-content .progress:nth-child(1) .bar span{
    width: 90%;
}

.skills-column:nth-child(1) .skills-content .progress:nth-child(2) .bar span{
    width: 80%;
}

.skills-column:nth-child(1) .skills-content .progress:nth-child(3) .bar span{
    width: 60%;
}

.skills-column:nth-child(1) .skills-content .progress:nth-child(4) .bar span{
    width: 75%;
}

.skills-column:nth-child(2) .skills-content .progress:nth-child(1) .bar span{
    width: 80%;
}

.skills-column:nth-child(2) .skills-content .progress:nth-child(2) .bar span{
    width: 50%;
}

.skills-column:nth-child(2) .skills-content .progress:nth-child(3) .bar span{
    width: 85%;
}

.skills-column:nth-child(2) .skills-content .progress:nth-child(4) .bar span{
    width: 65%;
}

.contact{
    min-height: auto;
    padding-bottom: 7rem;
}

.contact form{
    max-width: 70rem;
    margin: 0 auto;
    text-align: center;
}

.contact form .input-box{
    position: relative;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.contact form .input-box .input-field{
    position: relative;
    width: 49%;
    margin: .8rem 0;
}

.contact form .input-box .input-field input,
.contact form .textarea-field textarea{
    width: 100%;
    height: 100%;
    padding: 1.5rem;
    font-size: 1.6rem;
    color: var(--text-color);
    background: transparent;
    border-radius: .6rem;
    border: .2rem solid var(--main-color);
}


.contact form .input-box .input-field input::placeholder,
.contact form .textarea-field textarea::placeholder{
    color: var(--text-color);
}

.contact form .focus{
    position: absolute;
    top: 0;
    left: 0;
    width: 0%;
    height: 100%;
    background: var(--second-bg-color);
    border-radius: .6rem;
    z-index: -1;
    transition: .5s;
}

.contact form .input-box .input-field input:focus~.focus,
.contact form .input-box .input-field input:valid~.focus,
.contact form .textarea-field textarea:focus~.focus,
.contact form .textarea-field textarea:valid~.focus{
    width: 100%;
}

.contact form .textarea-field {
    position: relative;
    margin: .8rem 0 2.7rem;
    display: flex;
}

.contact form .textarea-field textarea {
    resize: none;
}

.contact form .btn-box.btns .btn{
    cursor: pointer;
}

/// 
HTML

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
    <link
      href="https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css"
      rel="stylesheet"
    />

    <title>Document</title>
  </head>
  <body>
    <header class="header">
      <a href="#" class="logo">Gabriel Ferreira.</a>

      <div class="bx bx-menu" id="menu-icon"></div>

      <nav class="navbar">
        <a href="#home" class="active">Inicio</a>
        <a href="#about">Sobre Mim</a>
        <a href="#education">Curriculo</a>
        <a href="#skills">Habilidades</a>
        <a href="#contact">Contato</a>
      </nav>
    </header>

    <main>
      <section class="home" id="home">
        <div class="home-content">
          <h1>Olá, eu sou <span>Gabriel</span></h1>
          <div class="text-animate">
            <h3>Desenvolvedor Front-end</h3>
          </div>
          <p>
            sou Gabriel, um desenvolvedor front-end com uma visão abrangente do
            back-end. Minha jornada no mundo do desenvolvimento web tem sido
            marcada por um compromisso constante com a excelência e a inovação.
            Estou ansioso para enfrentar novos desafios e contribuir para
            projetos empolgantes no futuro.
          </p>
          <div class="btn-box">
            <a href="#" class="btn">Contate-me</a>
            <a href="#" class="btn">Fale comigo</a>
          </div>
        </div>

        <div class="home-sci">
          <a href="#"><i class="bx bxl-linkedin"></i></a>
          <a href="#"><i class="bx bxl-instagram"></i></a>
          <a href="#"><i class="bx bxl-github"></i></a>
        </div>

        <!-- <div class="home-imgHover"></div> -->
      </section>

      <section class="about" id="about">

        <h2 class="heading">Sobre <span>Mim</span></h2>

        <div class="about-img">
          <img src="assets/about.jpg" />
          <span class="circle-spin"></span>
        </div>

        <div class="about-content">
          <h3>Desenvolvedor Front-end</h3>
          <p>
            Aos 15 anos, ingressei na Etec de Cândido Mota, onde cursei
            Informática para Internet integrado ao ensino médio. Nesse período,
            aprendi HTML, CSS, PHP e JavaScript, consolidando uma base sólida em
            programação web. Essa experiência foi mais do que uma preparação
            para o mercado de trabalho; foi o início de uma paixão que continua
            a guiar minha trajetória profissional. Estou ansioso para explorar
            novas tecnologias e contribuir com soluções criativas e inovadoras
            na programação. Cada linha de código é uma oportunidade de
            transformar ideias em realidade, e estou determinado a fazer cada
            uma delas contar.
          </p>

          <div class="btn-box btns">
            <a href="#" class="btn">Leia Mais</a>
          </div>
        </div>
      </section>

  
      <section class="education" id="education">
    
        <h2 class="heading">Minha <span>Carreira</span></h2>

        <div class="education-row">
            <div class="education-column">
                <h3 class="title">Curriculo</h3>
                <div class="education-box">


                    <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar'></i>2021 - 2023</div>
                            <h3>Curso Técnico integrado ao ensino médio - Etec </h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam maxime vero facere cupiditate quisquam, quasi iure temporibus ea porro aspernatur officiis libero quod quibusdam ad quae odit quas aut reprehenderit?</p>
                        </div>
                    </div>

                <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar'></i>2021 - 2023</div>
                            <h3>Curso Técnico integrado ao ensino médio - Etec </h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam maxime vero facere cupiditate quisquam, quasi iure temporibus ea porro aspernatur officiis libero quod quibusdam ad quae odit quas aut reprehenderit?</p>
                        </div>
                    </div>

                <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar'></i>2021 - 2023</div>
                            <h3>Curso Técnico integrado ao ensino médio - Etec </h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam maxime vero facere cupiditate quisquam, quasi iure temporibus ea porro aspernatur officiis libero quod quibusdam ad quae odit quas aut reprehenderit?</p>
                        </div>
                    </div>

                </div>
            </div>

             <div class="education-column">
                <h3 class="title">Experiência</h3>
                <div class="education-box">


                    <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar'></i>2023</div>
                            <h3>Curso Front-end - ADA TECH</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam maxime vero facere cupiditate quisquam, quasi iure temporibus ea porro aspernatur officiis libero quod quibusdam ad quae odit quas aut reprehenderit?</p>
                        </div>
                    </div>

                <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar'></i>2023</div>
                            <h3>Curso Front-end - ADA TECH</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam maxime vero facere cupiditate quisquam, quasi iure temporibus ea porro aspernatur officiis libero quod quibusdam ad quae odit quas aut reprehenderit?</p>
                        </div>
                    </div>

                <div class="education-content">
                        <div class="content">
                            <div class="year"><i class='bx bxs-calendar'></i>2023</div>
                            <h3>Curso Front-end - ADA TECH</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam maxime vero facere cupiditate quisquam, quasi iure temporibus ea porro aspernatur officiis libero quod quibusdam ad quae odit quas aut reprehenderit?</p>
                        </div>
                    </div>

                </div>
            </div>


        </div>
      </section>

      <section class="skills" id="skills">
        <h2 class="heading">Minhas <span>Habilidades</span></h2>

        <div class="skills-row">
            <div class="skills-column">
                <h3 class="title">Habilidades de Programação</h3>

              <div class="skills-box">
                <div class="skills-content">
                    <div class="progress">
                        <h3>HTML <span>90%</span></h3>
                        <div class="bar"><span></span></div>
                    </div>

                        <div class="progress">
                        <h3>CSS <span>80%</span></h3>
                        <div class="bar"><span></span></div>
                    </div>

                        <div class="progress">
                        <h3>JavaScript <span>60%</span></h3>
                        <div class="bar"><span></span></div>
                    </div>

                        <div class="progress">
                        <h3>PHP <span>75%</span></h3>
                        <div class="bar"><span></span></div>
                    </div>
                </div>
              </div>  
            </div>

             <div class="skills-column">
                <h3 class="title">Habilidades Profissionais</h3>

              <div class="skills-box">
                <div class="skills-content">
                    <div class="progress">
                        <h3> Trabalho em Equipe <span>80%</span></h3>
                        <div class="bar"><span></span></div>
                    </div>

                        <div class="progress">
                        <h3> Comunicação <span>50%</span></h3>
                        <div class="bar"><span></span></div>
                    </div>

                        <div class="progress">
                        <h3> Resolução de Problemas <span>85%</span></h3>
                        <div class="bar"><span></span></div>
                    </div>

                        <div class="progress">
                        <h3> Gestão de Equipe <span>65%</span></h3>
                        <div class="bar"><span></span></div>
                    </div>
                </div>
              </div>  
            </div>


        </div>
      </section>

      <section class="contact" id="contact">

        <h2 class="heading">Contate - <span>me!</span></h2>

        <form action="">
          <div class="input-box">
            <div class="input-field">
              <input type="text" placeholder="Nome completo" required>
              <span class="focus"></span>
            </div>
                 <div class="input-field">
              <input type="text" placeholder="Email" required>
              <span class="focus"></span>
            </div>
          </div>

           <div class="input-box">
            <div class="input-field">
              <input type="number" placeholder="Número de telefone" required>
              <span class="focus"></span>
            </div>
                 <div class="input-field">
              <input type="text" placeholder="Assunto do email" required>
              <span class="focus"></span>
            </div>
          </div>

          <div class="textarea-field">
            <textarea name="" id="" cols="30" rows="10" placeholder="Sua mensagem" required></textarea>
            <span class="focus"></span>
          </div>

          <div class="btn-box btns">
            <button type="submit" class="btn">Enviar</button>
          </div>
        </form>
      </section>

    </main>

    <footer></footer>
    <script src="scripts.js"></script>
  </body>
</html>
