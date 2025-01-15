<template>
  <div class="calculator-container">
    <header class="calculator-header">Calculadora</header>
    <div class="display">
      <div class="expression">{{ expression }}</div>
      <div class="result">{{ result || '0' }}</div>
    </div>
    <div class="buttons">
      <button v-for="btn in buttons" :key="btn" :class="'btn-' + btn" @click="handleClick(btn)">{{ btn }}</button>
    </div>
    <div class="history">
      <h3>Historial</h3>
      <ul>
        <li v-for="(entry, index) in history" :key="index">{{ entry }}</li>
      </ul>
      <button class="clear-history" @click="clearHistory">Limpiar Historial</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      expression: '',
      result: '',
      history: [],
      buttons: [
        '7', '8', '9', '/',
        '4', '5', '6', '*',
        '1', '2', '3', '-',
        '0', '.', '=', '+',
        'C', '%', 'AC'
      ],
    };
  },
  methods: {
    handleClick(btn) {
      if (btn === 'C') {
        this.expression = '';
      } else if (btn === 'AC') {
        this.expression = '';
        this.result = '';
        this.history = [];
      } else if (btn === '=') {
        try {
          const evaluated = eval(this.expression.replace(/%/, '/100')); 
          
          this.result = evaluated;
          this.history.unshift(`${this.expression} = ${evaluated}`);
          //this.expression = this.result;
        } catch (e) {
          this.result = 'Error';
        }
      } else {
        this.expression += btn;
      }
    },
    clearHistory() {
      this.history = [];
    }
  }
};
</script>

<style>

</style>