<script lang="ts">
  import type { ItemInterface } from '../../models/items/Item.interface'
  export let items: ItemInterface[] = []

  const handleClick = (item: ItemInterface) => {
    item.selected = !item.selected
    items = items
    console.log('handleItemClick', item.id, item.selected)
  }
</script>

<div>
  <h3>Items:</h3>
  <ul>
    {#each items as item}
      <li on:click={() => handleClick(item)}>
        {item.name} [{item.selected}]
      </li>
    {/each}
  </ul>
</div>

