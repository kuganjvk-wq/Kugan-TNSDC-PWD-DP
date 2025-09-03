/* General Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(270deg, #00b4db, #0083b0);
  background-size: 400% 400%;
  animation: backgroundShift 15s ease infinite;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

/* Container styling */
.container {
  text-align: center;
  color: white;
}

/* Headline animation */
.headline {
  font-size: 2.5rem;
  animation: fadeInSlide 2s ease-out forwards;
  opacity: 0;
  transform: translateY(-20px);
  margin-bottom: 2rem;
}

/* Button with hover animation */
.animated-button {
  padding: 1rem 2rem;
  font-size: 1.2rem;
  background-color: #ffffff;
  color: #0083b0;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  transition: transform 0.3s ease, background-color 0.3s ease;
}

.animated-button:hover {
  background-color: #00b4db;
  color: white;
  transform: scale(1.1);
}

/* Keyframes */
@keyframes fadeInSlide {
  0% {
    opacity: 0;
    transform: translateY(-30px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes backgroundShift {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}
