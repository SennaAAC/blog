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
            max-width: 1080px;
            margin: 20px auto;
        }

    @media (min-width: 320px) and (max-width: 769px) {
      main {
        max-width: 300px;
        margin: 20px auto;
        font-size: 10px;
      }
    }
  
  </style>