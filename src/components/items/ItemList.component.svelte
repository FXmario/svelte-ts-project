<script lang="ts">
  import type { ItemInterface } from '../../models/items/Item.interface'
  export let items: ItemInterface[] = []
</script>

<div>
  <h3>Items:</h3>
  <ul>
    {#each items as item}
      <li>
        {item.name}
      </li>
    {/each}
  </ul>
</div>

