<script lang="ts">
  import ChildComponent from './ChildComponent.vue'
  import type { MyChildProps } from './ChildComponent.vue'
  
  type ChildComponentWithGenerics = new <T>(props: MyChildProps<T>) => {
    $props: MyChildProps<T>
  }
  
  export default ChildComponent as ChildComponentWithGenerics
  </script>