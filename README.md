<!DOCTYPE html>
<html lang="ro">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Vlad Cristian – Călător între Lumi / Traveler Between Worlds</title>
  <style>
    /* Reset & base */
    * {
      box-sizing: border-box;
      margin: 0; padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      color: #eee;
    }
    body {
      background: linear-gradient(135deg, #0a0a0a 0%, #1a1a2e 100%);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 20px;
    }
    img {
      max-width: 100%;
      height: auto;
      border-radius: 12px;
      margin-bottom: 20px;
      filter: brightness(0.85) contrast(1.1);
    }
    header {
      text-align: center;
      margin-bottom: 40px;
    }
    h1 {
      font-size: 2.8rem;
      margin-bottom: 10px;
      font-weight: 700;
      line-height: 1.1;
    }
    h2 {
      font-weight: 400;
      font-style: italic;
      font-size: 1.3rem;
      color: #bbb;
      max-width: 380px;
      margin: 0 auto 40px;
    }
    nav {
      margin-bottom: 50px;
    }
    button.lang-btn {
      background: #222538;
      border: none;
      color: #eee;
      font-weight: 600;
      padding: 10px 18px;
      margin: 0 5px;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    button.lang-btn:hover {
      background: #555a8a;
    }
    button.lang-btn.active {
      background: #5f7aed;
      color: white;
      font-weight: 700;
    }
    section.content {
      max-width: 600px;
      text-align: center;
      font-size: 1.1rem;
      line-height: 1.5;
      color: #ddd;
      min-height: 160px;
    }
    footer {
      margin-top: 60px;
      font-size: 0.9rem;
      color: #777;
    }
  </style>
</head>
<body>
  <header>
    <h1 id="title">Vlad Cristian – Călător între Lumi</h1>
    <h2 id="subtitle">Scriitor al nevăzutului. Explorator al viselor. Ghid printre umbrele trecutului.</h2>
    <nav>
      <button class="lang-btn active" data-lang="ro">RO</button>
      <button class="lang-btn" data-lang="en">EN</button>
    </nav>
  </header>

  <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80" alt="Siluetă singuratică pe drum în ceață" />

  <section class="content" id="content">
    <p>
      Vlad Cristian nu scrie doar cuvinte, ci urmează ecoul viselor care i-au traversat sufletul o viață întreagă. Născut în București, într-un spital marcat de destin, și crescut între dealurile Stoieneștiului și tăcerea munților, a învățat să citească lumea cu ochii dinlăuntru.<br><br>
      Fascinat de simboluri, de civilizații vechi, de energii subtile și de fărâmele unei vieți anterioare care par să-i bântuie prezentul, Vlad nu trăiește cu picioarele pe pământ, ci cu sufletul printre lumi.<br><br>
      Visele i-au fost profesori. Femeia din vis – ghid tăcut. Bunicul și bunica – ancora în timpuri care nu mai sunt, dar care încă respiră în el.<br><br>
      Nu caută confirmare. Nu cere să fie înțeles. Dar dacă îl citești cu inima, s-ar putea să te regăsești.<br><br>
      Pentru unii, e doar un bărbat.<br>
      Pentru alții, un călător al conștiinței.<br>
      Pentru sine, este: o întrebare care încă nu s-a rostit.
    </p>
  </section>

  <footer>
    &copy; 2025 Vlad Cristian
  </footer>

  <script>
    const content = {
      ro: {
        title: "Vlad Cristian – Călător între Lumi",
        subtitle: "Scriitor al nevăzutului. Explorator al viselor. Ghid printre umbrele trecutului.",
        text: `
          Vlad Cristian nu scrie doar cuvinte, ci urmează ecoul viselor care i-au traversat sufletul o viață întreagă. Născut în București, într-un spital marcat de destin, și crescut între dealurile Stoieneștiului și tăcerea munților, a învățat să citească lumea cu ochii dinlăuntru.<br><br>
          Fascinat de simboluri, de civilizații vechi, de energii subtile și de fărâmele unei vieți anterioare care par să-i bântuie prezentul, Vlad nu trăiește cu picioarele pe pământ, ci cu sufletul printre lumi.<br><br>
          Visele i-au fost profesori. Femeia din vis – ghid tăcut. Bunicul și bunica – ancora în timpuri care nu mai sunt, dar care încă respiră în el.<br><br>
          Nu caută confirmare. Nu cere să fie înțeles. Dar dacă îl citești cu inima, s-ar putea să te regăsești.<br><br>
          Pentru unii, e doar un bărbat.<br>
          Pentru alții, un călător al conștiinței.<br>
          Pentru sine, este: o întrebare care încă nu s-a rostit.
        `
      },
      en: {
        title: "Vlad Cristian – Traveler Between Worlds",
        subtitle: "Writer of the unseen. Explorer of dreams. A guide through the shadows of the past.",
        text: `
          Vlad Cristian doesn’t just write words; he follows the echo of dreams that have crossed his soul for a lifetime. Born in Bucharest, in a hospital marked by destiny, and raised between the hills of Stoienești and the silence of the mountains, he learned to read the world with inner eyes.<br><br>
          Fascinated by symbols, ancient civilizations, subtle energies, and fragments of past lives that seem to haunt his present, Vlad doesn’t live with his feet on the ground, but with his soul among worlds.<br><br>
          Dreams were his teachers. The woman from the dream – a silent guide. Grandfather and grandmother – anchors in times that no longer exist but still breathe within him.<br><br>
          He doesn’t seek confirmation. He doesn’t ask to be understood. But if you read him with your heart, you might find yourself.<br><br>
          For some, he is just a man.<br>
          For others, a traveler of consciousness.<br>
          For himself, he is: a question yet to be spoken.
        `
      }
    };

    const buttons = document.querySelectorAll('.lang-btn');
    const titleEl = document.getElementById('title');
    const subtitleEl = document.getElementById('subtitle');
    const contentEl = document.getElementById('content');

    buttons.forEach(btn => {
      btn.addEventListener('click', () => {
        buttons.forEach(b => b.classList.remove('active'));
        btn.classList.add('active');
        const lang = btn.getAttribute('data-lang');

        titleEl.innerHTML = content[lang].title;
        subtitleEl.innerHTML = content[lang].subtitle;
        contentEl.innerHTML = `<p>${content[lang].text}</p>`;
      });
    });
  </script>
</body>
</html>
