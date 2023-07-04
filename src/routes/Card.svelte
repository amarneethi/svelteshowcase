<style>
  .card {
    font-family: sans-serif;
    display: flex;
    flex-direction: column;
    background-color: #FFE27C;
    width: 200px;
  }

  .row {
    display: flex;
    flex-direction: row;
    flex: 1;
  }

  .column {
    display: flex;
    flex-direction: column;
    flex: 1;
  }

  .column.users {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }

  .imagestack{
    position: relative;
    width: 24px;
    border-radius: 24px;
    border: 2px solid #FFE27C ;
  }

  .imagestack:nth-child(1) {
    left:0px;
  }

  .imagestack:nth-child(2){
    left: -4px;

  }

  .imagestack:nth-child(3){
    left: -8px;
  }

  .imagestack:nth-child(4){
    left: -12px;
  }


</style>

<div class="card">
  <div class="row">
    <div class="column">
      <p>Design system</p>
      <p>Team Meeting</p>
    </div>
    <div class="column">
      <img src="./google-meets-icon.png" width="32px" alt="">
    </div>
  </div>
  <div class="row">
    <div class="column users">
        <!-- Column 1 -->
        <img class="imagestack" src="./user-1.jpeg" width="100%" alt="">
        <img class="imagestack" src="./user-2.jpeg" width="100%" alt="">
        <img class="imagestack" src="./user-3.jpeg" width="100%" alt="">
        <img class="imagestack" src="./user-4.jpeg" width="100%" alt="">
    </div>
    <div class="column">
      <!-- Column 2 -->
    </div>
  </div>
  <div class="row">
    <div class="column">
      <!-- Column 1 -->
    </div>
    <div class="column">
      <!-- Column 2 -->
    </div>
  </div>
</div>
