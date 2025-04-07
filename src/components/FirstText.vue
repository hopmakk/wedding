<template>
    <div class="text-container">
      <p class="styled-paragraph">
        Рассадка появится немного позже...
      </p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'StyledTextBlock'
  }
  </script>
  
  <style scoped>
  .text-container {
    margin: 0 auto; /* Центрирование контейнера */
    max-width: 1200px; /* Максимальная ширина для больших экранов */
    /* box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    border-radius: 15px; */
  }
  
  .styled-paragraph {
    padding: 20px;
    color: rgb(255, 43, 63); /* Указанный цвет */
    font-family: 'Caveat', cursive;
    font-weight: 700; /* Более жирное начертание */
    line-height: 1.5; /* Межстрочный интервал */
  }
  </style>