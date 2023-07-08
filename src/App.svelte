<script lang="ts">
  import ItemListComponent from './components/items/itemList.component.svelte'
  const items: any[] = [{
    id: 1,
    name: 'Item 1'
  },
  {
    id: 2,
    name: 'Item 2'
  },
  {
    id: 3,
    name: 'Item 3'
  }]
</script>

<main>
  <div class="home">
    <ItemListComponent items={items} /> 
  </div>
</main>

