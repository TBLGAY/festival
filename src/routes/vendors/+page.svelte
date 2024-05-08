<script lang="ts">
    import IconButton from "$lib/LinkButton.svelte";
    import LinkButtonList from "$lib/LinkButtonList.svelte";
    import Navbar from "$lib/Navbar.svelte";
    import SplitContainer from "$lib/SplitContainer.svelte";
    import links_data from "$lib/assets/constitution.toml";
  
    const links = Object.values(links_data);
  </script>
  
  <svelte:head>
    <title>TBLGAY's Constitution</title>
  </svelte:head>
  
  <main>
    <h1>coming soon!</h1>
  
  </main>
  
  <style>
    main {
      display: flex;
      align-items: center;
      justify-content: center;
      min-height: 100%;
    }
  
    :global(html, body) {
      width: 100%;
      height: 70%;
    }
  
    h1 {
      font-size: 7em;
      filter: drop-shadow(rgb(242, 166, 166) 0.01em 0.01em 2px);
      font-family: 'Signika Negative', sans-serif;
    }
  </style>
  