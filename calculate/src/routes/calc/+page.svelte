<h1>Простой Калькулятор</h1>
<script>
  let num1 = 0;
  let num2 = 0;
  let result = 0;
  
  function add() {
    result = num1 + num2;
  }
  
  function subtract() {
    result = num1 - num2;
  }
  
  function multiply() {
    result = num1 * num2;
  }
  
  function divide() {
    result = num1 / num2;
  }
</script>

<input type="number" bind:value={num1}>
<input type="number" bind:value={num2}>

<button on:click={add}>+</button>
<button on:click={subtract}>-</button>
<button on:click={multiply}>*</button>
<button on:click={divide}>/</button>

<p>Результат: {result}</p>