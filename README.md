<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Respiratory System + Cardiovascular System</title>

  <style>
    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      background: #eef6ff;
      color: #222;
    }

    .top {
      background: white;
      padding: 28px 20px;
      text-align: center;
      border-bottom: 1px solid #d6e6f7;
    }

    .top h1 {
      margin: 0;
      color: #1d3557;
      font-size: 34px;
    }

    .top p {
      margin: 10px auto 0;
      max-width: 800px;
      color: #555;
      line-height: 1.5;
    }

    .page {
      max-width: 1100px;
      margin: 25px auto;
      padding: 0 18px 40px;
    }

    .layout {
      display: grid;
      grid-template-columns: 260px 1fr;
      gap: 22px;
    }

    .menu {
      background: white;
      border: 1px solid #d6e6f7;
      border-radius: 16px;
      padding: 15px;
      height: fit-content;
      box-shadow: 0 4px 15px rgba(0,0,0,0.06);
    }

    .menu h2 {
      font-size: 18px;
      margin-top: 0;
      color: #1d3557;
    }

    .menu button {
      display: block;
      width: 100%;
      margin-bottom: 9px;
      padding: 12px;
      border: 1px solid #cfe0f2;
      border-radius: 10px;
      background: #f8fbff;
      cursor: pointer;
      text-align: left;
      font-size: 15px;
    }

    .menu button:hover {
      background: #eaf5ff;
    }

    .menu button.active {
      background: #2b6cb0;
      color: white;
      font-weight: bold;
    }

    .content {
      background: white;
      border: 1px solid #d6e6f7;
      border-radius: 16px;
      padding: 28px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.06);
    }

    .section {
      display: none;
    }

    .section.active {
      display: block;
    }

    h2 {
      color: #1d3557;
      font-size: 30px;
      border-bottom: 3px solid #edf4fb;
      padding-bottom: 10px;
      margin-top: 0;
    }

    h3 {
      margin-top: 24px;
      color: #2b4a67;
      font-size: 20px;
    }

    p, li {
      font-size: 16px;
      line-height: 1.7;
    }

    .mini-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 14px;
      margin-bottom: 20px;
    }

    .mini-card {
      border-radius: 14px;
      padding: 17px;
      color: white;
    }

    .blue {
      background: #2b6cb0;
    }

    .red {
      background: #c53030;
    }

    .mini-card h3 {
      color: white;
      margin-top: 0;
    }

    .mini-card p {
      margin-bottom: 0;
      color: white;
    }

    .image-box {
      margin-top: 22px;
      padding: 14px;
      background: #f8fbff;
      border: 1px solid #d6e6f7;
      border-radius: 14px;
      text-align: center;
    }

    .image-box img {
      width: 100%;
      max-width: 750px;
      border-radius: 10px;
      border: 1px solid #ddd;
      background: white;
    }

    .caption {
      color: #666;
      font-size: 14px;
      margin-bottom: 0;
    }

    .flow {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      align-items: center;
      margin: 10px 0 20px;
    }

    .flow div {
      background: #eaf5ff;
      border: 1px solid #c6ddf3;
      color: #1d3557;
      padding: 12px 14px;
      border-radius: 10px;
      font-weight: bold;
    }

    .flow span {
      color: #2b6cb0;
      font-size: 24px;
      font-weight: bold;
    }

    .career-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 16px;
    }

    .career-card {
      background: #f8fbff;
      border: 1px solid #d6e6f7;
      border-radius: 14px;
      padding: 18px;
    }

    .source-box {
      background: #f8fbff;
      border: 1px solid #d6e6f7;
      border-radius: 14px;
      padding: 16px;
      margin-bottom: 12px;
    }

    .source-box b {
      display: block;
      color: #1d3557;
      margin-bottom: 8px;
    }

    .source-box a {
      color: #2b6cb0;
      overflow-wrap: anywhere;
    }

    @media (max-width: 800px) {
      .layout {
        grid-template-columns: 1fr;
      }

      .mini-grid,
      .career-grid {
        grid-template-columns: 1fr;
      }

      .top h1 {
        font-size: 27px;
      }
    }
  </style>
</head>

<body>

  <div class="top">
    <h1>Respiratory System + Cardiovascular System</h1>
    <p>Anatomy & Physiology II Final Project: how these two body systems work together to maintain homeostasis in the body.</p>
  </div>

  <div class="page">
    <div class="layout">

      <div class="menu">
        <h2>Click A Section</h2>
        <button class="tab active" onclick="showSection('overview', this)">Project Overview</button>
        <button class="tab" onclick="showSection('respiratory', this)">Respiratory System</button>
        <button class="tab" onclick="showSection('cardiovascular', this)">Cardiovascular System</button>
        <button class="tab" onclick="showSection('together', this)">How They Work Together</button>
        <button class="tab" onclick="showSection('asthma', this)">Disease / Disorder</button>
        <button class="tab" onclick="showSection('careers', this)">Careers</button>
        <button class="tab" onclick="showSection('sources', this)">Sources</button>
      </div>

      <div class="content">

        <div id="overview" class="section active">
          <h2>Project Overview</h2>

          <div class="mini-grid">
            <div class="mini-card blue">
              <h3>Respiratory System</h3>
              <p>Brings oxygen in and removes carbon dioxide.</p>
            </div>

            <div class="mini-card red">
              <h3>Cardiovascular System</h3>
              <p>Moves blood, oxygen, nutrients, and waste.</p>
            </div>
          </div>

          <p>
            This website is about the respiratory system and cardiovascular system. It explains what each system does, the organs in each system, how they work together, and how they help maintain homeostasis in the body.
          </p>
        </div>

        <div id="respiratory" class="section">
          <h2>Respiratory System</h2>

          <h3>Body System #1</h3>
          <p>Respiratory system</p>

          <h3>Main Organs</h3>
          <p>
            The main organs that are in this system are : Lungs, trachea, bronchi, bronchioles, alveoli, diaphragm, nose, and mouth.
          </p>

          <h3>What It Does For The Body</h3>
          <p>
            The respiratory system gets oxygen into the body and removes carbon dioxide. Oxygen is used by cells to make energy, and carbon dioxide is a waste of gas that must be removed.
          </p>

          <div class="image-box">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/Respiratory_system_complete_en.svg/800px-Respiratory_system_complete_en.svg.png" alt="Respiratory system diagram">
            <p class="caption">Respiratory system diagram</p>
          </div>
        </div>

        <div id="cardiovascular" class="section">
          <h2>Cardiovascular System</h2>

          <h3>Body System #2</h3>
          <p>Cardiovascular system</p>

          <h3>Main Organs</h3>
          <p>The main organs of this are: Heart, blood, arteries, veins, and capillaries.</p>

          <h3>What It Does For The Body</h3>
          <p>
            The cardiovascular system pumps blood in the whole body. It carries oxygen, nutrients, hormones, and waste products to the cells and from the cells.
          </p>

          <div class="image-box">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/0e/Circulatory_System_en.svg/800px-Circulatory_System_en.svg.png" alt="Cardiovascular system diagram">
            <p class="caption">Cardiovascular system diagram</p>
          </div>
        </div>

        <div id="together" class="section">
          <h2>How They Work Together</h2>

          <div class="flow">
            <div>Oxygen enters lungs</div>
            <span>→</span>
            <div>Blood picks it up</div>
            <span>→</span>
            <div>Heart pumps it to body</div>
          </div>

          <h3>How These Two Systems Connect</h3>
          <p>
            The respiratory system gets oxygen into the lungs. Then the cardiovascular system picks up that oxygen in the blood and delivers it to the rest of the body. The blood also has carbon dioxide back to the lungs so it can be breathed out.
          </p>

          <h3>Homeostasis</h3>
          <p>
            They help maintain the oxygen levels, carbon dioxide levels, blood pH, and the energy balance.
          </p>

          <h3>Real-Life Example</h3>
          <p>
            While you're exercising, your muscles need more oxygen. Your breathing rate will go up to bring in more oxygen, and your heart rate also increases to pump more oxygen-rich blood to your muscles even faster.
          </p>
        </div>

        <div id="asthma" class="section">
          <h2>Disease / Disorder: Asthma</h2>

          <h3>What Disease Or Disorder?</h3>
          <p>Asthma</p>

          <h3>Which System It Affects More</h3>
          <p>
            It affects the respiratory system more, but it is also impacting the cardiovascular system since the heart has to work harder when the body is not getting enough oxygen.
          </p>

          <h3>Symptoms</h3>
          <p>
            Asthma can cause wheezing, coughing, chest tightness, and shortness of breath. These symptoms happen when the airways become swollen, tight, or become filled with mucus.
          </p>

          <h3>Diagnosis</h3>
          <p>
            A doctor diagnoses asthma by checking their symptoms, asking about medical history, doing a physical exam, and using lung tests like spirometry to see how much breathing is happening.
          </p>

          <h3>Treatment</h3>
          <p>
            Asthma can be treated with inhalers, medications, avoiding triggers, and following the asthma plan by the doctor. It can’t always be fully cured, but it can usually be controlled to not affect as much.
          </p>

          <h3>How It Disrupts Homeostasis</h3>
          <p>
            Asthma disrupts homeostasis by making it more difficult for the oxygen to enter the lungs and get to the blood. This lowers oxygen levels, and increases carbon dioxide levels, and make the heart and lungs work even harder to keep the body more balanced.
          </p>
        </div>

        <div id="careers" class="section">
          <h2>Careers</h2>

          <div class="career-grid">
            <div class="career-card">
              <h3>Pulmonologist</h3>
              <p>
                A pulmonologist is a doctor who is a specialist in the lungs and breathing problems. They treat diseases like asthma, pneumonia, COPD, and other respiratory problems.
              </p>
            </div>

            <div class="career-card">
              <h3>Respiratory Therapist</h3>
              <p>
                A respiratory therapist can help patients with breathing problems. They can give breathing treatments, help with oxygen therapy, do breathing tests, and work with doctors to help maintain lung conditions.
              </p>
            </div>
          </div>
        </div>

        <div id="sources" class="section">
          <h2>Sources</h2>

          <p>These are the website links I used for my project.</p>

          <div class="source-box">
            <b>Source 1</b>
            <a href="https://www.mayoclinic.org/diseases-conditions/asthma/symptoms-causes/syc-20369653" target="_blank">
              https://www.mayoclinic.org/diseases-conditions/asthma/symptoms-causes/syc-20369653
            </a>
          </div>

          <div class="source-box">
            <b>Source 2</b>
            <a href="https://my.clevelandclinic.org/health/body/circulatory-and-cardiovascular-system" target="_blank">
              https://my.clevelandclinic.org/health/body/circulatory-and-cardiovascular-system
            </a>
          </div>

          <div class="source-box">
            <b>Source 3</b>
            <a href="https://my.clevelandclinic.org/health/body/21205-respiratory-system" target="_blank">
              https://my.clevelandclinic.org/health/body/21205-respiratory-system
            </a>
          </div>

          <div class="source-box">
            <b>Source 4</b>
            <a href="https://www.webmd.com/health-insurance/insurance-doctor-types" target="_blank">
              https://www.webmd.com/health-insurance/insurance-doctor-types
            </a>
          </div>
        </div>

      </div>
    </div>
  </div>

  <script>
    function showSection(sectionId, button) {
      var sections = document.querySelectorAll('.section');
      var tabs = document.querySelectorAll('.tab');

      sections.forEach(function(section) {
        section.classList.remove('active');
      });

      tabs.forEach(function(tab) {
        tab.classList.remove('active');
      });

      document.getElementById(sectionId).classList.add('active');
      button.classList.add('active');
    }
  </script>

</body>
</html>
