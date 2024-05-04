<script>
    import Hero from "$lib/Hero.svelte";
  </script>
  
  <Hero/>
  <section class="section flow">
    <h2>Art Show Events</h2>
  <div class="boxes">
    
    <div class="flow">
        <img src="https://picsum.photos/300?random1" alt="placeholder">
        <div>
            <h3>Featured Artists</h3>
        <div class="subheading">May 2024</div>
    </div>
     <p>Complete the form to request an application to exhibit</p>
     <a href="/blog" class="button">Application</a>
    </div>
  
    <div class="flow">
        <img src="https://picsum.photos/300?random2" alt="placeholder">
        <div><h3>Contributors</h3>
        <div class="subheading">May 2024</div>
        </div>
     <p>Complete the form to contribute to the event</p>
     <a href="/contact" class="button">Contribute</a>
    </div>
  </div>
  </section>
  <style>
    section{
        padding: 3rem;
        background-color: rgb(216, 185, 241);
        border-radius: 1rem;
    }
  .boxes {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(14rem, 1fr));
  gap: 3rem;
  }
  
  .subheading {
    text-transform: uppercase;
    font-size: 0.8rem;
    letter-spacing: 1px;
  }
  
  .button {
    display: inline-block;
    padding-inline: 1rem;
  }
  </style>