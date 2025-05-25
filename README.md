<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Hadiah Untukmu</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background-color: #000;
      color: #ddd;
      font-family: Arial, sans-serif;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
      overflow: hidden;
    }

    h1 {
      font-size: 2.2em;
      animation: blink 2s infinite;
    }

    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.3; }
    }

    button {
      background-color: #222;
      color: #0f0;
      border: 2px solid #0f0;
      padding: 15px 30px;
      font-size: 1.5em;
      cursor: pointer;
      border-radius: 8px;
      transition: 0.3s ease;
    }

    button:hover {
      background-color: #0f0;
      color: black;
    }

    #jumpscare {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background: black;
      display: none;
      justify-content: center;
      align-items: center;
      z-index: 9999;
    }

    #jumpscare img {
      width: 100vw;
      height: 100vh;
      object-fit: cover;
      animation: shake 0.2s infinite;
    }

    @keyframes shake {
      0% { transform: translate(0, 0); }
      25% { transform: translate(-20px, 15px); }
      50% { transform: translate(20px, -15px); }
      75% { transform: translate(-20px, -15px); }
      100% { transform
