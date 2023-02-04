<svelte:head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/prism-themes/1.9.0/prism-coldark-dark.min.css" integrity="sha512-UE88w575S5hQlj3QhY249ZKOe9noZYPtmKL6DwZnKQtTFRCw2dkRfUdp6GwxeV/mig7Q9G7H3vcX8ETVRDRrTg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
  <link rel="stylesheet" href="/pico.css">
  <link rel="stylesheet" href="/global.css">
</svelte:head>

<script>
    import Header from "$lib/Header.svelte";
    import Footer from "$lib/Footer.svelte";
  </script>
  
  <Header/>
  
  <main>
    <slot></slot>
  </main>
  
  <Footer/>
  
  <style>
  
    main {
        padding-top: 50px;
    }

    @media (min-width:320px){
      main {
        max-width: 280px;
        margin: 10px auto;
      }
    }
    @media (min-width:481px){
      main {
        max-width: 400px;
        margin: 10px auto;
      }
    }
    @media (min-width:641px) {
      main {
        max-width: 560px;
        margin: 10px auto;
      }
    }
    @media (min-width:961px) {
      main {
        max-width: 750px;
        margin: 10px auto;
      }
    }
    @media (min-width:1025px) {
      main {
        max-width: 900px;
        margin: 10px auto;
      }
    }
    @media (min-width:1281px) {
      main {
        max-width: 1100;
        margin: 10px auto;
      }
    }

    /* @media (min-width: 320px) and (max-width: 769px) {
      main {
        max-width: 400px;
        margin: 10px auto;
      }
    } */
  
  </style>