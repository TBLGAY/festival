<script>
  import IconButton from "$lib/LinkButton.svelte";
  import LinkButtonList from "$lib/LinkButtonList.svelte";
  import Navbar from "$lib/Navbar.svelte";
  import SplitContainer from "$lib/SplitContainer.svelte";
  import links_data from "$lib/assets/links.toml";

  const links = Object.values(links_data);
</script>

<svelte:head>
  <title>TBLGAY</title>
</svelte:head>

<SplitContainer>
  <div slot="left" class="left">
    <h1 style:font-family="'Signika Negative', sans-serif">TBLGAY's<br/> Queer Film Festival</h1>
    <h3
      style:font-family="'DM Sans', sans-serif"
      style:font-size="1.196em"
      style:margin-bottom="0.1em"
    >
      a showcase of student art & film
    </h3>
    <p
      style:font-family="'DM Sans', sans-serif"
      style:margin-top="0"
      style:font-size="1.02em"
    >
      TBLGAY, York University's queer community service, presents a showcase of film and art by and for queer students.
      <br />
      <br />
      <b>taking place on July 3rd, at [LOCATION TBD]</b>
    </p>
  </div>
  <hr />
  <div slot="right" class="right">
    <LinkButtonList {links} />
  </div>
</SplitContainer>

<style>
  .left {
    height: 100%;

    display: flex;
    flex-direction: column;
    /* align-items: center; */
    justify-content: flex-start;
  }

  .left h1 {
    margin-top: 0.2em;
    color: rgb(66, 59, 59);
    font-size: 3em;
    margin-bottom: 0;
    text-shadow: 1px 1px 2px rgb(211, 173, 173);
  }
</style>
