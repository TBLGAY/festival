<script>
  import SplitContainer from "$lib/SplitContainer.svelte";
  import space from "$lib/assets/space.toml";
</script>

<svelte:head>
  <title>tblgay | about</title>
</svelte:head>

<SplitContainer>
  <div slot="left" class="left">
    <h1 style:font-family="'Signika Negative', sans-serif">about</h1>
    <p>
      The TBLGAY Queer Film Festival is an outdoors showcase of student film and art, hosted by Trans, Bisexual, Lesbian, Gay, Asexual at York.
    </p>
    <p>
      It is open to community members from across Toronto, no matter what university or institution they study at!
    </p>
  </div>
  <hr />
  <div slot="right" class="right">
    <h3>Details</h3>
    {#each Object.values(space.open) as times}
      <h4>{times.term}</h4>
      <p>{times.hours}</p>
    {/each}
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
    font-size: 4em;
    margin-bottom: 0;
    text-shadow: 1px 1px 2px rgb(211, 173, 173);
  }


  p {
    font-family: "DM Sans", sans-serif;
    margin-top: 0;
    font-size: 1.25em;
  }

  h3 {
    font-size: 1.4em;
  }

  h3,
  h4 {
    font-family: "DM Sans", sans-serif;
    margin-bottom: 0.1em;
  }

  h4 {
    font-size: 1.25em;
  }

  a {
    color: #db1225;
  }

  a:hover {
    color: #9b0b19;
  }
</style>
