<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>دردشة عالمية</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #1e3c72, #2a5298);
      color: #fff;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }

    #welcome-screen, #chat-screen {
      display: none;
      text-align: center;
      padding: 20px;
      box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
      border-radius: 10px;
    }

    #welcome-screen {
      display: flex;
      flex-direction: column;
      align-items: center;
      background: #ffffff22;
      padding: 20px;
      border-radius: 10px;
    }

    #welcome-screen input {
      margin: 10px 0;
      padding: 10px;
      border: none;
      border-radius: 5px;
      width: 80%;
    }

    #welcome-screen button {
      padding: 10px 20px;
      background-color: #4caf50;
      border: none;
      border-radius: 5px;
      color: #fff;
      cursor: pointer;
      font-size: 16px;
    }

    #chat-screen {
      display: flex;
      flex-direction: column;
      background: #ffffff22;
      width: 90%;
      max-width: 800px;
      height: 90vh;
      border-radius: 20px;
      overflow: hidden;
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.5);
    }

    #chat-header {
      background: #1e3c72;
      padding: 10px;
      text-align: center;
      font-size: 24px;
      font-weight: bold;
      color: #ffcd3c;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
    }

    #chat-messages {
      flex-grow: 1;
      overflow-y: auto;
      padding: 20px;
      background: #ffffff33;
      border-radius: 20px;
    }

    .message {
      margin-bottom: 15px;
    }

    .message span {
      font-weight: bold;
      color: #ffcd3c;
    }

    #message-input {
      display: flex;
      padding: 10px;
      background: #1e3c72;
      border-top: 2px solid #ffffff33;
    }

    #message-input input {
      flex-grow: 1;
      padding: 10px;
      border: none;
      border-radius: 5px;
      font-size: 16px;
    }

    #message-input button {
      padding: 10px 20px;
      background-color: #4caf50;
      border: none;
      border-radius: 5px;
      color: #fff;
      cursor: pointer;
      font-size: 16px;
      margin-left: 10px;
    }

    @media (max-width: 600px) {
      #chat-screen {
        max-width: 100%;
      }
    }
  </style>
</head>
<body>
  <div id="welcome-screen">
    <h1>دردشة البودي</h1>
    <p>يرجى إدخال اسمك للبدء</p>
    <input type="text" id="username" placeholder="أدخل اسمك">
    <button onclick="startChat()">ابدأ</button>
  </div>

  <div id="chat-screen">
    <div id="chat-header">غرفة الدردشة</div>
    <div id="chat-messages"></div>
    <div id="message-input">
      <input type="text" id="message" placeholder="أدخل رسالتك">
      <button onclick="sendMessage()">إرسال</button>
    </div>
  </div>

  <script>
    let username = "";
    const apiUrl = "https://hpppppplgog.tiiny.io/";

    // بدء الدردشة
    function startChat() {
      username = document.getElementById("username").value.trim();
      if (!username) {
        alert("يرجى إدخال اسمك");
        return;
      }
      document.getElementById("welcome-screen").style.display = "none";
      document.getElementById("chat-screen").style.display = "flex";
      fetchMessages();
    }

    // تحميل الرسائل
    async function fetchMessages() {
      try {
        const response = await fetch(apiUrl);
        if (!response.ok) throw new Error("تعذر جلب الرسائل");

        const data = await response.json();
        if (data.status === "success") {
          const messagesDiv = document.getElementById("chat-messages");
          messagesDiv.innerHTML = ""; // مسح الرسائل القديمة
          data.messages.forEach((msg) => {
            const messageEl = document.createElement("div");
            messageEl.classList.add("message");
            messageEl.innerHTML = `<span>${msg.sender}:</span> ${msg.message}`;
            messagesDiv.appendChild(messageEl);
          });
          messagesDiv.scrollTop = messagesDiv.scrollHeight; // التمرير لأسفل
        } else {
          console.error("لم يتم استرجاع الرسائل بنجاح.");
        }
      } catch (error) {
        console.error("خطأ في جلب الرسائل:", error);
      }
      setTimeout(fetchMessages, 2000); // التحديث كل 2 ثانية
    }

    // إرسال رسالة
    async function sendMessage() {
      const messageInput = document.getElementById("message");
      const message = messageInput.value.trim();
      if (!message) return;

      console.log("إرسال رسالة إلى API:", message);  // إضافة سجل للتأكد من إرسال الرسالة

      try {
        const response = await fetch(apiUrl, {
          method: "POST",
          headers: { "Content-Type": "application/json" },
          body: JSON.stringify({ sender: username, message: message }),
        });

        if (response.ok) {
          messageInput.value = "";
          fetchMessages();
        } else {
          console.error("فشل إرسال الرسالة");
        }
      } catch (error) {
        console.error("خطأ في إرسال الرسالة:", error);
      }
    }
  </script>
</body>
</html>
