<script>
  import Card from './Card.svelte'
  const meeting = {
    subject: 'Meeting Subject',
    host: 'Meeting Host',
    meetingIcon: './google-meets-icon.png',
    time: 'Meeting Time',
    link: 'Meeting Link',
    users: [
      './user-1.jpeg',
      './user-2.jpeg',
      './user-3.jpeg',
      './user-4.jpeg'
    ]
  }
</script>

<Card {meeting} />