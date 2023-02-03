<script lang="ts">
</script>

<main>
  <h1>JS Clickjacking Demo</h1>

  <p>
    Check out <a href="https://google.com" target="_blank" rel="noreferrer"
    on:click={(evt) => {
      evt.preventDefault()
      window.location.href = "https://bing.com"
    }}>this link</a>, it goes to Google!
  </p>

  <p class="note">
    Always check your link sources, and never trust prompts!
  </p>
</main>

<style>
  .note {
    color: #888;
  }
</style>