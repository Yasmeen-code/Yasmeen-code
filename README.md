
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Yasmeen - Backend Developer</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');

  body {
    font-family: 'Poppins', sans-serif;
    background: #0f172a;
    color: #e2e8f0;
    margin: 0;
    padding: 40px 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
  }

  .card {
    background: #1e293b;
    border-radius: 24px;
    padding: 40px;
    max-width: 800px;
    width: 100%;
    box-shadow: 0 20px 50px rgba(0,0,0,0.5);
    text-align: center;
    border: 1px solid #334155;
    position: relative;
    overflow: hidden;
  }

  .card::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(99,102,241,0.1) 0%, transparent 70%);
    animation: rotate 20s linear infinite;
    z-index: 0;
  }

  @keyframes rotate {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }

  .content {
    position: relative;
    z-index: 1;
  }

  .avatar {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    background: linear-gradient(135deg, #6366f1, #a855f7);
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 20px;
    font-size: 48px;
    box-shadow: 0 0 30px rgba(168, 85, 247, 0.4);
  }

  h1 {
    font-size: 2.5rem;
    margin: 0 0 10px;
    background: linear-gradient(90deg, #818cf8, #c084fc);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  h3 {
    font-weight: 300;
    color: #94a3b8;
    margin: 0 0 30px;
    font-size: 1.2rem;
  }

  .project-link {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    background: #334155;
    color: #e2e8f0;
    padding: 10px 20px;
    border-radius: 50px;
    text-decoration: none;
    font-size: 0.95rem;
    transition: all 0.3s ease;
    margin-bottom: 30px;
  }

  .project-link:hover {
    background: #475569;
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.3);
  }

  .section-title {
    font-size: 1.1rem;
    color: #94a3b8;
    margin: 30px 0 15px;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 600;
  }

  .tools {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
    margin-top: 10px;
  }

  .tool {
    background: #0f172a;
    border: 1px solid #334155;
    border-radius: 12px;
    padding: 12px;
    width: 60px;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: all 0.3s ease;
    cursor: pointer;
  }

  .tool:hover {
    border-color: #818cf8;
    transform: translateY(-5px) scale(1.1);
    box-shadow: 0 10px 20px rgba(99, 102, 241, 0.2);
  }

  .tool img {
    width: 35px;
    height: 35px;
    object-fit: contain;
    filter: brightness(0.9);
    transition: filter 0.3s;
  }

  .tool:hover img {
    filter: brightness(1.2);
  }

  .socials {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-top: 10px;
  }

  .social {
    width: 45px;
    height: 45px;
    border-radius: 50%;
    background: #0f172a;
    border: 1px solid #334155;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #94a3b8;
    text-decoration: none;
    font-size: 20px;
    transition: all 0.3s ease;
  }

  .social:hover {
    background: #6366f1;
    color: white;
    border-color: #6366f1;
    transform: translateY(-3px);
  }

  .stats {
    display: flex;
    justify-content: center;
    gap: 40px;
    margin: 30px 0;
    padding: 20px 0;
    border-top: 1px solid #334155;
    border-bottom: 1px solid #334155;
  }

  .stat {
    text-align: center;
  }

  .stat-number {
    font-size: 1.8rem;
    font-weight: 700;
    color: #818cf8;
  }

  .stat-label {
    font-size: 0.8rem;
    color: #64748b;
    text-transform: uppercase;
    letter-spacing: 1px;
  }

  .badge {
    display: inline-block;
    background: rgba(99, 102, 241, 0.15);
    color: #818cf8;
    padding: 4px 12px;
    border-radius: 20px;
    font-size: 0.75rem;
    margin: 5px;
    border: 1px solid rgba(99, 102, 241, 0.3);
  }

  .typing {
    overflow: hidden;
    border-right: 2px solid #818cf8;
    white-space: nowrap;
    animation: typing 3s steps(30, end), blink-caret 0.75s step-end infinite;
    display: inline-block;
    max-width: 100%;
  }

  @keyframes typing {
    from { width: 0 }
    to { width: 100% }
  }

  @keyframes blink-caret {
    from, to { border-color: transparent }
    50% { border-color: #818cf8 }
  }
</style>
<base target="_blank">
</head>
<body>

<div class="card">
  <div class="content">
    <div class="avatar">👩‍💻</div>
    <h1>Hi, I'm Yasmeen</h1>
    <h3 class="typing">Backend Developer from Egypt 🇪🇬</h3>

    <div style="margin: 15px 0;">
      <span class="badge">PHP</span>
      <span class="badge">Laravel</span>
      <span class="badge">Python</span>
      <span class="badge">SQL</span>
      <span class="badge">Docker</span>
      <span class="badge">Linux</span>
    </div>

    <div class="stats">
      <div class="stat">
        <div class="stat-number">5+</div>
        <div class="stat-label">Languages</div>
      </div>
      <div class="stat">
        <div class="stat-number">10+</div>
        <div class="stat-label">Tools</div>
      </div>
      <div class="stat">
        <div class="stat-number">∞</div>
        <div class="stat-label">Passion</div>
      </div>
    </div>

    <a href="https://github.com/Yasmeen-code/AILIXIR_BackEnd" class="project-link" target="_blank">
      🔭 Currently Working on: AILIXIR BackEnd
    </a>

    <div class="section-title">Connect With Me</div>
    <div class="socials">
      <a href="#" class="social" title="GitHub">🐙</a>
      <a href="#" class="social" title="LinkedIn">💼</a>
      <a href="#" class="social" title="Twitter">🐦</a>
      <a href="#" class="social" title="Email">✉️</a>
    </div>

    <div class="section-title">Languages & Tools</div>
    <div class="tools">
      <div class="tool" title="Bootstrap"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap"></div>
      <div class="tool" title="C"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c"></div>
      <div class="tool" title="C++"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus"></div>
      <div class="tool" title="C#"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg" alt="csharp"></div>
      <div class="tool" title="Docker"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker"></div>
      <div class="tool" title="Git"><img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git"></div>
      <div class="tool" title="HTML5"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5"></div>
      <div class="tool" title="Laravel"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/laravel/laravel-plain-wordmark.svg" alt="laravel"></div>
      <div class="tool" title="Linux"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux"></div>
      <div class="tool" title="MariaDB"><img src="https://www.vectorlogo.zone/logos/mariadb/mariadb-icon.svg" alt="mariadb"></div>
      <div class="tool" title="MATLAB"><img src="https://upload.wikimedia.org/wikipedia/commons/2/21/Matlab_Logo.png" alt="matlab"></div>
      <div class="tool" title="SQL Server"><img src="https://www.svgrepo.com/show/303229/microsoft-sql-server-logo.svg" alt="mssql"></div>
      <div class="tool" title="MySQL"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql"></div>
      <div class="tool" title="Oracle"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/oracle/oracle-original.svg" alt="oracle"></div>
      <div class="tool" title="PHP"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg" alt="php"></div>
      <div class="tool" title="PostgreSQL"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql"></div>
      <div class="tool" title="Python"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python"></div>
      <div class="tool" title="Tailwind CSS"><img src="https://www.vectorlogo.zone/logos/tailwindcss/tailwindcss-icon.svg" alt="tailwind"></div>
    </div>
  </div>
</div>

</body>
</html>
