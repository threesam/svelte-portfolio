<style>
  section {
    display: grid;
    position: relative;
    width: 100%;
    font-weight: 600;
    color: var(--black);
    z-index: 10;
  }
  div {
    padding: 2rem;

    transition: all 0.2s ease-in;
  }
  a {
    color: var(--yellow);
  }
  a:hover {
    color: var(--light-grey);
    font-weight: 900;
  }
  p {
    color: var(--white);
  }
  @media (max-width: 799px) {
    section {
      grid-template-columns: 1fr;
    }
  }
  @media (min-width: 800px) {
    section {
      grid-template-columns: repeat(4, 1fr);
      gap: 1rem;
      padding: 1rem;
      font-size: 1.2rem;
      height: 100vh;
    }
    div {
      border-radius: 10px;
      display: grid;
      place-content: center;
      overflow: hidden;
    }
  }
</style>

<section>
  <div class="bg">
    <p>
      My name is Salvatore D'Angelo III but everyone calls me
      <b>Sam</b>
    </p>
  </div>
  <div class="bg">
    <p>I grew up in Trenton, NJ.</p>
  </div>
  <div class="bg">
    <p>
      Graduated with a double major in PolySci and Global Studies from
      <a href="https://rider.edu" target="_blank" rel="noopener noreferrer">
        Rider
      </a>
      just in time to realize that I liked the theory of politics a lot more
      than the practice
    </p>
  </div>
  <div class="bg">
    <p>
      so I thought...
      <em>Might as well go play some music</em>
    </p>
  </div>
  <div class="bg">
    <p>
      My friend convinced me to check out a “really cool” open mic at a local
      <a
        href="https://www.facebook.com/trentonsocial"
        target="_blank"
        rel="noopener noreferrer">
        bar
      </a>
      in my hometown
    </p>
  </div>
  <div class="bg">
    <p>
      It was and I went every week, started waiting tables, making drinks,
      became a part of a beautifully underground arts community, co-founded a
      production
      <a
        href="https://sixtomidnight.productions"
        target="_blank"
        rel="noopener noreferrer">
        company
      </a>
      , and met my
      <a
        href="https://dianadangelo.com"
        target="_blank"
        rel="noopener noreferrer">
        wife
      </a>
    </p>
  </div>
  <div class="bg">
    <p>We had two lovely little girls, Phoenix and Juniper</p>
  </div>
  <div class="bg">
    <p>Our dog, Koda, is grumpily protective of each new addition</p>
  </div>
  <div class="bg">
    <p>
      Inspired by #generativeart and looking to evolve my company, I came upon
      <a
        href="https://processing.org"
        target="_blank"
        rel="noopener noreferrer">
        The Processing Foundation
      </a>
      , started slow and kept iterating daily until programming became an
      insatiable pursuit
    </p>
  </div>
  <div class="bg">
    <p>
      Coupling art and code led to an interest in web design and development
    </p>
  </div>
  <div class="bg">
    <p>
      I’m now obsessed with solving my clients’ problems and designing
      responsive solutions that scale
    </p>
  </div>
  <div class="bg">
    <p>
      For more info, here's my
      <a
        href="./salvatore-dangelo-resume.PDF"
        target="_blank"
        rel="noopener noreferrer">
        resume
      </a>
    </p>
  </div>
</section>

<!-- /* background with lowered opacity, text with full */
@media(max-width: 799px) {
    .bg {
        background-color: rgba(var(--rgb-dark-grey), 0.9);
    }
}

@media(min-width: 800px) {
    .bg {
        position: relative;
        z-index: 1;
    }
    
    .bg::before {
        content: "";
        position: absolute;
        top: 0; 
        left: 0;
        width: 100%; 
        height: 100%;  
        opacity: 0.85; 
        z-index: -1;
        background-color: unset;
        background-image: url('images/portfolioBG_BW.png');
        background-size: cover;
        background-attachment: fixed;
      }

    .bg:nth-of-type(3),
    .bg:nth-of-type(6),
    .bg:nth-of-type(9),
    .bg:nth-of-type(11) {
        grid-column: span 2;
    }
} -->
