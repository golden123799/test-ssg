<script lang="ts">
    import { Svroller } from 'svrollbar'
  
    const items = Array.from({ length: 50 }).map((_, i) => `item ${i}`)
  </script>
  
  <Svroller width="10rem" height="10rem">
    <!-- <div style="height:100px; overflow: scroll;"> -->

        {#each items as item (item)}
          <div>{item}</div>
        {/each}
    <!-- </div> -->
  </Svroller>