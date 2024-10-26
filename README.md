# Hi... I'm Dmitrii 👋

I will be a Developer.

- Open to project collaborations
- You can reach me through:

<div align="left">
    <a href="https://github.com/qavelkii/">
        <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
    </a>
    <a href="mailto:qavelkii@gmail.com">
        <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
    </a>
    <a href="https://wa.me/17868346332">
        <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
    </a>
    <a href="https://www.linkedin.com/in/dmitrii-velikii/">
        <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
    </a>
</div>

**NOTE**: Let's help each other 🤝
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Running Mario Animation</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #87ceeb;
      overflow: hidden;
      margin: 0;
    }
    
    .scene {
      position: relative;
      width: 100%;
      height: 200px;
      overflow: hidden;
    }

    .ground {
      position: absolute;
      bottom: 0;
      width: 100%;
      height: 50px;
      background: #654321;
    }

    .mario {
      position: absolute;
      bottom: 50px;
      width: 50px;
      height: 50px;
      background: url('https://www.spriters-resource.com/resources/sheets/44/47359.png?updated=1670588656') -40px -40px;
      background-size: 200%;
      animation: run 0.5s steps(4) infinite, jump 3s ease-in-out infinite;
    }

    @keyframes run {
      0% { transform: translateX(0); }
      100% { transform: translateX(1000px); }
    }

    @keyframes jump {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-100px); }
    }
  </style>
</head>
<body>
  <div class="scene">
    <div class="ground"></div>
    <div class="mario"></div>
  </div>
</body>
</html>
