<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Salmon Paul's Creative Portfolio</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    :root {
      --primary: #0052cc;
      --secondary: #4a6fa5;
      --accent: #ff6b6b;
      --light: #f8f9fa;
      --dark: #212529;
      --gray: #6c757d;
      --border-radius: 18px;
      --box-shadow: 0 12px 30px rgba(0,0,0,0.08);
      --transition: all 0.3s ease;
    }
    
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    
    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
      background: linear-gradient(135deg, #f8fafc 0%, #e6f0ff 100%);
      color: var(--dark);
      line-height: 1.6;
      min-height: 100vh;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    
    .container {
      width: 100%;
      max-width: 900px;
      margin: 40px auto;
      background: #fff;
      border-radius: var(--border-radius);
      box-shadow: var(--box-shadow);
      padding: 50px;
      position: relative;
      overflow: hidden;
    }
    
    .container::before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 8px;
      background: linear-gradient(90deg, var(--primary), var(--accent));
    }
    
    header {
      text-align: center;
      margin-bottom: 40px;
    }
    
    h1 {
      color: var(--primary);
      margin-bottom: 15px;
      font-weight: 800;
      font-size: 2.8rem;
      letter-spacing: -0.5px;
      position: relative;
      padding-bottom: 15px;
    }
    
    h1::after {
      content: "";
      position: absolute;
      bottom: 0;
      left: 50%;
      transform: translateX(-50%);
      width: 100px;
      height: 5px;
      background: var(--accent);
      border-radius: 3px;
    }
    
    .tagline {
      font-size: 1.3rem;
      color: var(--secondary);
      font-weight: 500;
      margin-bottom: 20px;
    }
    
    .intro {
      text-align: center;
      font-size: 1.15rem;
      margin-bottom: 40px;
      color: var(--gray);
      font-weight: 500;
      max-width: 700px;
      margin: 0 auto 40px;
      line-height: 1.8;
    }
    
    .profile-link {
      text-align: center;
      margin-bottom: 50px;
    }
    
    .profile-link a {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      color: var(--primary);
      font-weight: 700;
      font-size: 1.25rem;
      text-decoration: none;
      padding: 14px 28px;
      border-radius: 50px;
      transition: var(--transition);
      background: rgba(0, 82, 204, 0.05);
      border: 2px solid rgba(0, 82, 204, 0.1);
    }
    
    .profile-link a:hover {
      background: rgba(0, 82, 204, 0.1);
      transform: translateY(-3px);
      box-shadow: 0 6px 15px rgba(0,0,0,0.1);
    }
    
    section {
      margin-bottom: 60px;
      position: relative;
    }
    
    section h2 {
      color: var(--secondary);
      font-size: 1.9rem;
      font-weight: 700;
      margin-bottom: 30px;
      display: flex;
      align-items: center;
      gap: 15px;
      padding-bottom: 15px;
      border-bottom: 2px solid rgba(0, 82, 204, 0.1);
    }
    
    section h2 i {
      color: var(--accent);
      width: 40px;
      height: 40px;
      background: rgba(0, 82, 204, 0.05);
      border-radius: 50%;
      display: inline-flex;
      align-items: center;
      justify-content: center;
    }
    
    .embeds-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
      gap: 30px;
    }
    
    .embed-card {
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 6px 15px rgba(0,0,0,0.08);
      transition: var(--transition);
      background: #fff;
    }
    
    .embed-card:hover {
      transform: translateY
