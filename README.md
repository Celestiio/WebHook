webhook.edit({
	name: 'VVickedNoob',
	avatar: 'https://ibb.co/LNMdrPm',
})

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Discord Webhook Tutorial</title>
  </head>
  <body>
    <button onclick="sendMessage()">Send</button>
  </body>

  <script>
    function sendMessage() {
      var request = new XMLHttpRequest();
      request.open("POST", "https://discord.com/api/webhooks/731897659685863434/cdSYPL_m-ZwimYUqXv7o319WguFofvruRn2HcdTSemvD6p158b0oDYeLRMl4n4YmTjZa");

      request.setRequestHeader('Content-type', 'application/json');

      var params = {
        username: "VVickedNoob",
        avatar_url: "https://ibb.co/LNMdrPm",
        content: "<@454363608793612288> https://cdn.discordapp.com/attachments/710162007650992218/714984326424690739/image0.png"
      }

      request.send(JSON.stringify(params));
    }
  </script>
</html>
