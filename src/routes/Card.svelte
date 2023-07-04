<script>
  export let meeting = {
    "subject": "Design system - Team meeting",
    "host": "Amarneethi R",
    "users": [
      "./user-1.jpeg",
      "./user-2.jpeg",
      "./user-3.jpeg",
      "./user-4.jpeg"
    ],
    "time": "10:15 - 12:15",
    "link": "https://example.com/meeting",
    "meetingIcon": "./google-meets-icon.png"

  }
</script>

<style>
  .card {
    font-family: sans-serif;
    display: flex;
    flex-direction: column;
    background-color: #FFE27C;
    width: 200px;
    padding: 12px;
    border-radius: 16px;
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
    flex: 3 1 auto;
    display: flex;
    flex-direction: row;
  }

  .imagestack{
    position: relative;
    width: 24px;
    height: 24px;
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

  .meetingSubject {
    flex: 4 1 auto;
    padding: 2px;
    font-size: 12px;
    font-weight: 600;
    color: #333;
  }

  .meetingHost {
    padding: 2px;
    font-size: 10px;
    font-weight: 400;
    color: #666;
  }

  p{
    margin: 0px;
  }


</style>

<div class="card">
  <div class="row meetingSubjectAndHost">
    <div class="column meetingSubject">
      <p>{meeting.subject}</p>
      <p class="meetingHost">{meeting.host}</p>
    </div>
    <div class="column meetingIcon">
      <img src={meeting.meetingIcon} width="32px" alt="">
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
      {meeting.time}
    </div>
  </div>
  <div class="row">
    <div class="column">
      <a href={meeting.link}>Join Meeting</a>
    </div>
    <div class="column">
      <!-- Column 2 -->
    </div>
  </div>
</div>
