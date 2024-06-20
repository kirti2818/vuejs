  <template>
    <div>
      <h1>Parent Component</h1>
      <ChildComponent>
        <template v-slot:header>
          <h1>Kirti Gupta</h1>
        </template>
        <template v-slot:content>
          <button>Buy Now</button>
        </template>
        <template v-slot:footer>
          <h2>Age is 21</h2>
        </template>
      </ChildComponent>
      <ChildComponent :isbtndisabled="isbtndisabled" :update="(val) => {
        isbtndisabled = val
      }">
        <template v-slot:header>
          <h1>Sakshi Gupta</h1>
        </template>
        <template v-slot:content>
          <button>Buy Now</button>
        </template>
        <template v-slot:footer>
          <h2>Age is 22</h2>
        </template>
      </ChildComponent>
      <!-- <ChildComponent></ChildComponent> -->
    </div>
  </template>
<script>
import ChildComponent from './ChildComponent.vue'
export default {
  name: "ParentComponent",
  components: {
    ChildComponent
  },
  data() {
    return {
      isbtndisabled: false
    }
  },
  watch: {
    isbtndisabled(newVal) {
      console.log("idbtndisabled", newVal)
    }
  },
  // methods: {
  //   updateIsBtnDisabled(val) {
  //     this.isbtndisabled = val;
  //   }
  // }
}
</script>