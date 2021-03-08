<template>
  <div class="expression-exercises container">
    <div class="row">
      <div class="col-12">

        <h1>Test???????</h1>

        <h1>Exercises</h1>
        <div class="border p-1">
          <p>
            Write a math equation Vue can evaluate, inside of the curly braces
            below:
          </p>

          <p>{{2+2 * 2 /2}}</p>
        </div>
        <div class="border p-1">
          <p>
            Use interpolation to get the customary Hello, World! to display on
            the screen. Don't forget your quotes
          </p>
          <p>{{phrase}}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import { reactive, toRefs } from "vue";
  export default {
    name: "ExpressionsExcercises",
    setup() {
      const output = reactive({phrase: 'Hello World!'})

      return toRefs(output)
    }
  }
</script>