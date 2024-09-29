<template>
    <div>
      <div id="date-x">{{ formattedDate }}</div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        formattedDate: ''
      };
    },
    methods: {
      updateDate() {
        const now = new Date();
        const options = { 
          year: 'numeric', 
          month: 'short', 
          day: 'numeric', 
          hour12: false 
        };
        this.formattedDate = now.toLocaleString('en-GB', options);
      }
    },
    mounted() {
      this.updateDate(); // Initial call to set the date immediately
      setInterval(this.updateDate, 1000); // Update the date every second
    },
    beforeDestroy() {
      clearInterval(this.interval); // Clear the interval to prevent memory leaks
    }
  };
  </script>
  
  <style scoped>
  #date-x {
    font-family: 'Poppins',sans-serif;
    opacity: 35%;
    font-size: small;
    text-align: center;
  }
  </style>