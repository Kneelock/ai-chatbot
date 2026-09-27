# ai-chatbot
trying this out
my-ai-chatbot/
│
├── index.html
├── style.css
├── script.js
└── README.md
<!DOCTYPE html>
<html>
<head>
  <title>My AI Chatbot</title>
  <link rel="stylesheet" href="style.css">
</head>

<body>

  <h1>My AI Assistant</h1>

  <div id="chat"></div>

  <input id="message" placeholder="Ask something...">
  <button onclick="sendMessage()">Send</button>

  <script src="script.js"></script>

</body>
</html>
body {
  font-family: Arial;
  max-width: 700px;
  margin: 50px auto;
}

#chat {
  min-height: 400px;
  border: 1px solid #ddd;
  padding: 20px;
  margin-bottom: 20px;
}

input {
  width: 70%;
  padding: 10px;
}
function sendMessage() {
  const message = document.getElementById("message").value;

  document.getElementById("chat").innerHTML +=
    `<p><b>You:</b> ${message}</p>`;

  document.getElementById("message").value = "";
}
button {
  padding: 10px 20px;
}
