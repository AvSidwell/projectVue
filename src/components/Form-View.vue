<template>
    <div>
        <h2>Text Input</h2>
        <input type="text" src="" alt="" v-model="text" />{{ text }}
        <input type="image" src="" alt="" v-model="text" />{{ text }}
        <input type="checkbox" name="" id="checkbox" v-model="checked" />
        <label for="checkbox">Checked: {{ checked }}</label>
    </div>
    <div>
        <h2>Multi Checkbox</h2>
        <input type="checkbox" name="" id="Ches" v-model="checkedNames" value="Ches"/>
        <label for="Ches">Ches</label>
        <input type="checkbox" name="" id="Luke" v-model="checkedNames" value="Luke" />
        <label for="Luke">Luke</label>
        <p>
          <pre>{{ checkedNames }}</pre>
        </p>
    </div>
    <div>

        <h2>Radio</h2>
        <input type="radio" value="one" id="one" name="" v-model="picked">
        <label for="one">One</label>
        <br>
        <input type="radio" value="two" id="two" name="" v-model="picked">
        <label for="two">Two</label>
        <br>
        <span>Picked: {{ picked }}</span>
    </div>
    <div>
        <h2>Multi-Selector</h2>
        <select name="" id="" v-model="multiSelected" multiple style="width: 5rem">
        <option value="A">A</option>
        <option value="B">B</option>
        <option value="C">C</option>
    </select>
    <span>{{ multiSelected }}</span>
    </div>
</template>
<script>
export default {
  data() {
    return {
      text: "",
      checked: true,
      checkedNames: ['Ches'],
      picked: 'one',
      multiSelected: ['A']
    };
  },
};
</script>
