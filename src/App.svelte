<script lang="ts">
  import type { ItemInterface } from './models/items/Item.interface'
  import ItemListComponent from './components/items/ItemList.component.svelte'

  const items: ItemInterface[] = [
  {
    id: 1,
    name: 'Item 1',
    selected : false
  },
  {
    id: 2,
    name: 'Item 2',
    selected : false
  },
  {
    id: 3,
    name: 'Item 3',
    selected : false
  }
]
</script>

<main>
  <div class="home">
      <ItemListComponent items={items}/>
  </div>
</main>

<style>
</style>
