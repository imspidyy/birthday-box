// script.js
document.getElementById("wishBox").addEventListener("click", function() {
  const messageElement = document.querySelector(".message");

  // Change the message to a birthday wish
  messageElement.textContent = "Happy Birthday, jaan! 🎂💖";
  messageElement.style.fontSize = "24px";
  messageElement.style.color = "#ff69b4";
  
  // Add a hidden class to fade the old message
  setTimeout(() => {
    messageElement.classList.add("hidden");
  }, 1000);  // Hide the original message after 1 second

  // Show the birthday wish with some animation
  setTimeout(() => {
    messageElement.classList.remove("hidden");
  }, 1500);  // Show the new message after 1.5 seconds
});
