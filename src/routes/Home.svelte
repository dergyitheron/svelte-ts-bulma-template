<script>
	import { fade } from 'svelte/transition';
</script>

<main in:fade="{{duration: 400}}">
  <div class="hero-body">
    <div class="container has-text-centered">
      <div class="column is-6 is-offset-3">
        <h1 class="title">
            Home page
        </h1>
        <h2 class="subtitle">
            This is the best template
        </h2>
        <div class="box">
          <div class="field is-grouped">
            <p class="control is-expanded">
              <input class="input" type="text" placeholder="Enter your email">
            </p>
            <p class="control">
              <a class="button is-info" disabled>
                This is disabled
              </a>
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</main>

<style>

</style>
