<script lang="ts">
  import { IMainProps } from "../api/types.ts";


  export let pageData: IMainProps

  const {
    test, title
  } = pageData

  const toggle = (e: MouseEvent) => {
    console.log('click::', e);
  }

</script>

<main class='main'>
  <p>{test}</p>
  <p>{title}</p>
  <button style="padding: 10px 20px;" on:click={toggle}>Click me.</button>

</main>
