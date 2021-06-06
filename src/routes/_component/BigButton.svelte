<script>
  import { createEventDispatcher } from 'svelte';

  export let title = 'Button Title';
  export let color = 'white';

  const dispatch = createEventDispatcher();

  const submit = () => dispatch('submit');
</script>
<style>
    button {
        height: 120px;
        width: 120px;
        border-radius: 100%;
        background: var(--orange-color);
        border: 1px solid var(--text-color);
        cursor: pointer;
        transition: background-color 200ms ease-out;
    }

    button:hover {
        background: transparent;

    }

    .orange {
        background: var(--orange-color);

    }

    .red {
        background-color: var(--red-color);

    }


    .blue {
        background-color: var(--blue-color);

    }

    h2 {
        font-size: 20;
        font-weight: 500;
    }
</style>

<button class='{color}' on:click={submit}>
    <h2>
        {title}
    </h2>
</button>

