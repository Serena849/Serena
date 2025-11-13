
```html
<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <title>ASIA - Mappa Interattiva (Geografia 3ª Media)</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        :root {
            --blu: #004a99;
            --arancio: #cc6600;
            --accent: #007bff;
            --bg: #f5f7fb;
            --card-bg: #ffffff;
            --shadow: 0 10px 25px rgba(0,0,0,0.08);
        }

        * { box-sizing: border-box; }

        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
            background: var(--bg);
            color: #222;
        }

        h1 {
            color: var(--blu);
            border-bottom: 2px solid var(--blu);
            padding-bottom: 5px;
            margin-top: 0;
        }

        h2 {
            color: var(--arancio);
            margin-top: 30px;
        }

        ul { list-style-type: none; padding-left: 20px; }
        li { margin-bottom: 8px; }

        .focus {
            font-weight: bold;
            color: var(--accent);
        }

        /* LAYOUT MAPPA INTERATTIVA */
        .app-container {
            max-width: 1100px;
            margin: 0 auto;
        }

        .intro {
            margin-bottom: 20px;
            font-size: 0.95rem;
        }

        .layout {
            display: grid;
            grid-template-columns: minmax(0, 1.1fr) minmax(0, 1.3fr);
            gap: 20px;
            align-items: stretch;
            margin-bottom: 40px;
        }

        @media (max-width: 800px) {
            .layout {
                grid-template-columns: 1fr;
            }
        }

        .card {
            background: var(--card-bg);
            border-radius: 18px;
            padding: 18px;
            box-shadow: var(--shadow);
        }

        .card h2 {
            margin-top: 0;
        }

        .subtitle {
            font-size: 0.85rem;
            color: #555;
        }

        /* MINDMAP GRAFICA */
        .mindmap {
            position: relative;
            min-height: 320px;
            padding: 20px;
            overflow: hidden;
        }

        .node {
            position: absolute;
            border-radius: 999px;
            padding: 10px 16px;
            border: none;
            cursor: pointer;
            font-weight: bold;
            background: #ffffff;
            box-shadow: 0 6px 15px rgba(0,0,0,0.12);
            transition: transform 0.2s ease, box-shadow 0.2s ease, background 0.2s ease;
            font-size: 0.9rem;
            text-align: center;
        }

        .node.center {
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
            background: linear-gradient(135deg, var(--blu), var(--accent));
            color: #fff;
            padding: 14px 22px;
            font-size: 1rem;
        }

        .node[data-topic="fisica"] { top: 10%; left: 50%; transform: translateX(-50%); }
        .node[data-topic="politica"] { top: 65%; left: 10%; }
        .node[data-topic="climi"] { top: 65%; right: 10%; }

        .node:hover {
            transform: translate(-50%, -50%) scale(1.03);
        }

        .node:not(.center):hover {
            transform: translateY(-2px);
        }

        .node.active {
            outline: 3px solid var(--accent);
        }

        /* LINES (semplici) */
        .mindmap::before,
        .mindmap::after {
            content: "";
            position: absolute;
            border-radius: 999px;
        }

        /* Usando pseudo-elementi + gradienti solo come effetto grafico di sfondo */
        .mindmap::before {
            inset: 15% 25%;
            border: 1px dashed rgba(0,0,0,0.08);
        }

        /* DETTAGLI */
        .details-title {
            margin-top: 0;
            margin-bottom: 6px;
            color: var(--blu);
        }

        .details-subtitle {
            font-size: 0.85rem;
            color: #555;
            margin-bottom: 10px;
        }

        .pill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
            margin-bottom: 10px;
        }

        .pill {
            font-size: 0.8rem;
            border-radius: 999px;
            padding: 4px 10px;
            background: #eef4ff;
            color: #234;
        }

        .detail-section-title {
            font-weight: bold;
            margin-top: 10px;
            color: var(--arancio);
        }

        .detail-ul {
            padding-left: 18px;
            margin: 4px 0 4px 0;
        }

        .detail-ul li {
            margin-bottom: 4px;
            font-size: 0.9rem;
        }

        .hint {
            font-size: 0.78rem;
            color: #666;
            margin-top: 10px;
            font-style: italic;
        }

        .divider {
            height: 1px;
            background: rgba(0,0,0,0.06);
            margin: 30px 0 20px;
        }

        /* SEZIONE TESTO ORIGINALE */
        .static-section {
            max-width: 1100px;
            margin: 0 auto;
            background: #fff;
            padding: 18px;
            border-radius: 18px;
            box-shadow: var(--shadow);
        }

        .static-section h2 {
            border-left: 4px solid var(--arancio);
            padding-left: 8px;
        }
    </style>
</head>
<body>
<div class="app-container">
    <h1>ASIA: Il Continente dei Record</h1>
    <p class="intro">
        Mappa concettuale interattiva per la classe terza media – Geografia fisica, politica, climi e ambienti.
        Clicca sui cerchi della mappa o sulle parole in evidenza per vedere i dettagli.
    </p>

    <div class="layout">
        <!-- MAPPA INTERATTIVA -->
        <section class="card">
            <h2>🧠 Mappa Concettuale Interattiva</h2>
            <p class="subtitle">
                Clicca su <strong>Geografia Fisica</strong>, <strong>Geografia Politica</strong> o
                <strong>Climi e Ambienti</strong> per esplorare i punti chiave.
            </p>
            <div class="mindmap">
                <button class="node center" data-topic="overview">ASIA<br><span style="font-size:0.8rem;">Continente dei Record</span></button>
                <button class="node" data-topic="fisica">Geografia fisica</button>
                <button class="node" data-topic="politica">Geografia politica</button>
                <button class="node" data-topic="climi">Climi &amp; ambienti</button>
            </div>
        </section>

        <!-- DETTAGLI DINAMICI -->
        <section class="card" id="details-card">
            <h2 class="details-title" id="details-title">Come usare la mappa</h2>
            <p class="details-subtitle" id="details-subtitle">
                Seleziona un nodo della mappa a sinistra per vedere il riassunto e gli esempi principali.
            </p>

            <div id="details-content">
                <p>
                    Questa mappa ti aiuta a organizzare lo studio in tre grandi blocchi:
                </p>
                <ul class="detail-ul">
                    <li><strong>Geografia fisica</strong>: rilievi, fiumi, grandi pianure.</li>
                    <li><strong>Geografia politica</strong>: popolazione, stati, economie.</li>
                    <li><strong>Climi e ambienti</strong>: monsoni, fasce climatiche, biomi.</li>
                </ul>
                <p class="hint">
                    Suggerimento: puoi usare questa scheda come base per creare una tua mappa sul quaderno,
                    aggiungendo frecce, colori e immagini.
                </p>
            </div>
        </section>
    </div>

    <div class="divider"></div>

    <!-- SEZIONE TESTO ORIGINALE PER STAMPA/STUDIO -->
    <section class="static-section">
        <h2>🌎 GEOGRAFIA FISICA: Il Gigante del Mondo</h2>
        <ul>
            <li><span class="focus">Posizione e Confini</span>
                <ul>
                    <li>Confine Ovest: Monti <strong>Urali</strong> (con l'Europa)</li>
                    <li>Sud-Ovest: Canale di <strong>Suez</strong> (con l'Africa)</li>
                    <li>A Nord: Oceano <strong>Artico</strong></li>
                </ul>
            </li>
            <li><span class="focus">Rilievi e Morfologia</span>
                <ul>
                    <li><strong>Fascia Alpino-Himalayana</strong> (la catena più alta)
                        <ul>
                            <li><strong>Himalaya</strong>: Con il <strong>Monte Everest</strong> (8.848 m)</li>
                            <li>Altopiano del <strong>Tibet</strong> (detto "Il Tetto del Mondo")</li>
                        </ul>
                    </li>
                    <li>Grandi Pianure: Siberiana, Manciuria, Indo-Gangetica</li>
                </ul>
            </li>
            <li><span class="focus">Idrografia (Fiumi e Laghi)</span>
                <ul>
                    <li>Fiumi Principali (vitali per la vita e le economie):
                        <ul>
                            <li><strong>Yangtze</strong> (il più lungo, in Cina)</li>
                            <li><strong>Gange</strong> (sacro in India)</li>
                            <li><strong>Indo</strong> (Pakistan)</li>
                        </ul>
                    </li>
                    <li>Laghi e Bacini: <strong>Mar Caspio</strong> (il lago più grande), <strong>Mar d'Aral</strong> (prosciugamento)</li>
                </ul>
            </li>
        </ul>

        <h2>️ GEOGRAFIA POLITICA: Popoli e Nazioni</h2>
        <ul>
            <li><span class="focus">Popolazione</span>
                <ul>
                    <li>Il Continente più <strong>Popolato</strong> (oltre 4,7 miliardi di abitanti)</li>
                    <li><strong>Densità</strong> molto variabile (altissima in India/Cina, bassissima in Siberia/Deserti)</li>
                </ul>
            </li>
            <li><span class="focus">Macro-aree Geografiche</span>
                <ul>
                    <li>Estremo Oriente: Cina, Giappone, Coree</li>
                    <li>Subcontinente Indiano: India, Pakistan, Bangladesh</li>
                    <li>Sud-Est Asiatico: Indonesia, Thailandia, Filippine</li>
                    <li>Medio Oriente/Asia Occidentale: Penisola Arabica, Turchia, Iran</li>
                    <li>Asia Centrale: Kazakhstan, Uzbekistan (i paesi "stan")</li>
                </ul>
            </li>
            <li><span class="focus">Aspetti Economici</span>
                <ul>
                    <li>Paesi in Sviluppo (Economie emergenti come Cina e India)</li>
                    <li>Risorse chiave: Petrolio e gas (Medio Oriente, Russia asiatica)</li>
                    <li>Paesi ad alta tecnologia (Giappone, Corea del Sud)</li>
                </ul>
            </li>
        </ul>

        <h2>️ CLIMI e AMBIENTI: Una Varietà Estrema</h2>
        <ul>
            <li><span class="focus">Fattore Climatico Dominante</span>
                <ul>
                    <li>I <strong>Monsoni</strong>: Venti stagionali che portano piogge (estate) e siccità (inverno).</li>
                </ul>
            </li>
            <li><span class="focus">Principali Fasce Climatiche</span>
                <ul>
                    <li>Clima Equatoriale: Caldo e umido tutto l'anno (Sud-Est Asiatico).</li>
                    <li>Clima Continentale Freddo: Inverno lunghissimo e gelido (Siberia).</li>
                    <li>Clima Desertico/Arido: Forti escursioni termiche (Penisola Arabica).</li>
                    <li>Clima di Montagna: Varia con l'altitudine (Himalaya).</li>
                </ul>
            </li>
            <li><span class="focus">Biomi e Paesaggi Tipici</span>
                <ul>
                    <li>Foresta Pluviale (Equatoriale)</li>
                    <li>Taiga (Foresta di conifere in Siberia)</li>
                    <li>Tundra (Nord estremo)</li>
                    <li>Steppa (Asia Centrale)</li>
                </ul>
            </li>
        </ul>
    </section>
</div>

<script>
    // Dati della mappa concettuale
    const TOPICS = {
        overview: {
            title: "ASIA – Il Continente dei Record",
            subtitle: "Panoramica generale",
            pills: ["Continente più vasto", "Continente più popolato", "Grandi contrasti fisici e climatici"],
            sections: [
                {
                    title: "Perché è un continente di record?",
                    points: [
                        "È il continente più esteso della Terra.",
                        "È il continente più popolato (oltre 4,7 miliardi di abitanti).",
                        "Presenta i rilievi più alti (Himalaya, Monte Everest) e alcune tra le zone più fredde e più calde del pianeta."
                    ]
                },
                {
                    title: "Tre grandi blocchi da studiare",
                    points: [
                        "Geografia fisica: rilievi, pianure, fiumi, laghi.",
                        "Geografia politica: stati, popolazione, aree economiche.",
                        "Climi e ambienti: fasce climatiche, monsoni, biomi."
                    ]
                }
            ]
        },
        fisica: {
            title: "Geografia fisica dell’Asia",
            subtitle: "Rilievi, pianure, fiumi e laghi",
            pills: ["Monti Urali", "Himalaya", "Tibet", "Yangtze", "Gange", "Indo", "Mar Caspio"],
            sections: [
                {
                    title: "Posizione e confini",
                    points: [
                        "Confine Ovest con l’Europa: catena dei Monti Urali.",
                        "Confine Sud-Ovest con l’Africa: Canale di Suez.",
                        "A Nord: Oceano Artico."
                    ]
                },
                {
                    title: "Rilievi e morfologia",
                    points: [
                        "Fascia Alpino-Himalayana: la catena montuosa più alta del mondo.",
                        "Himalaya con il Monte Everest (8.848 m).",
                        "Altopiano del Tibet, chiamato anche “Tetto del Mondo”.",
                        "Grandi pianure: Siberiana, Manciuria, Indo-Gangetica."
                    ]
                },
                {
                    title: "Idrografia (fiumi e laghi)",
                    points: [
                        "Yangtze: il fiume più lungo dell’Asia, in Cina.",
                        "Gange: fiume sacro in India, fondamentale per la vita delle popolazioni.",
                        "Indo: fiume principale del Pakistan.",
                        "Mar Caspio: il lago più grande del mondo.",
                        "Mar d’Aral: lago in forte prosciugamento a causa degli usi umani dell’acqua."
                    ]
                }
            ]
        },
        politica: {
            title: "Geografia politica: popoli e nazioni",
            subtitle: "Popolazione, stati e aree geografiche",
            pills: ["4,7 miliardi di abitanti", "Macro-aree", "Economie emergenti"],
            sections: [
                {
                    title: "Popolazione",
                    points: [
                        "È il continente più popolato al mondo (oltre 4,7 miliardi di persone).",
                        "La densità di popolazione è molto variabile:",
                        "• altissima in paesi come India e Cina;",
                        "• bassissima in regioni come la Siberia o le aree desertiche."
                    ]
                },
                {
                    title: "Macro-aree geografiche",
                    points: [
                        "Estremo Oriente: Cina, Giappone, Coree.",
                        "Subcontinente indiano: India, Pakistan, Bangladesh.",
                        "Sud-Est asiatico: Indonesia, Thailandia, Filippine e altri stati insulari e peninsulari.",
                        "Medio Oriente / Asia occidentale: Penisola Arabica, Turchia, Iran.",
                        "Asia centrale: paesi “-stan”, come Kazakhstan, Uzbekistan, ecc."
                    ]
                },
                {
                    title: "Aspetti economici",
                    points: [
                        "Numerosi paesi in via di sviluppo, con economie emergenti come Cina e India.",
                        "Area ricchissima di risorse energetiche (petrolio e gas) soprattutto in Medio Oriente e Russia asiatica.",
                        "Presenza di paesi ad alta tecnologia come Giappone e Corea del Sud."
                    ]
                }
            ]
        },
        climi: {
            title: "Climi e ambienti dell’Asia",
            subtitle: "Monsoni, fasce climatiche e biomi",
            pills: ["Monsoni", "Clima equatoriale", "Clima continentale freddo", "Clima desertico", "Taiga", "Steppa"],
            sections: [
                {
                    title: "Fattore climatico dominante: i monsoni",
                    points: [
                        "I monsoni sono venti stagionali che cambiano direzione durante l’anno.",
                        "In estate portano aria umida dall’oceano e forti piogge.",
                        "In inverno prevale aria secca dall’interno del continente, con condizioni più asciutte."
                    ]
                },
                {
                    title: "Principali fasce climatiche",
                    points: [
                        "Clima equatoriale: caldo e umido tutto l’anno (Sud-Est asiatico).",
                        "Clima continentale freddo: inverni lunghissimi e gelidi, tipici della Siberia.",
                        "Clima desertico / arido: forti escursioni termiche tra giorno e notte (Penisola Arabica e altre zone interne).",
                        "Clima di montagna: varia molto con l’altitudine, come nell’Himalaya."
                    ]
                },
                {
                    title: "Biomi e paesaggi tipici",
                    points: [
                        "Foresta pluviale equatoriale nelle zone più calde e umide.",
                        "Taiga: vasta foresta di conifere soprattutto in Siberia.",
                        "Tundra: vegetazione bassa e resistente al freddo, nel nord estremo.",
                        "Steppa: grandi praterie dell’Asia centrale, adatte all’allevamento."
                    ]
                }
            ]
        }
    };

    function renderTopic(topicKey) {
        const topic = TOPICS[topicKey] || TOPICS.overview;
        const titleEl = document.getElementById('details-title');
        const subtitleEl = document.getElementById('details-subtitle');
        const contentEl = document.getElementById('details-content');

        titleEl.textContent = topic.title;
        subtitleEl.textContent = topic.subtitle || "";

        // Pills
        let html = "";
        if (topic.pills && topic.pills.length) {
            html += '<div class="pill-list">';
            topic.pills.forEach(p => {
                html += `<span class="pill">${p}</span>`;
            });
            html += '</div>';
        }

        // Sections
        if (topic.sections && topic.sections.length) {
            topic.sections.forEach(sec => {
                html += `<div class="detail-section">`;
                html += `<div class="detail-section-title">${sec.title}</div>`;
                if (sec.points && sec.points.length) {
                    html += `<ul class="detail-ul">`;
                    sec.points.forEach(pt => {
                        html += `<li>${pt}</li>`;
                    });
                    html += `</ul>`;
                }
                html += `</div>`;
            });
        }

        html += `<p class="hint">Suggerimento: prova a trasformare queste informazioni in una tua mappa sul quaderno, usando frecce e colori diversi per fisica, politica e climi.</p>`;

        contentEl.innerHTML = html;

        // Evidenzia il nodo attivo
        document.querySelectorAll('.node').forEach(btn => {
            btn.classList.toggle('active', btn.dataset.topic === topicKey);
        });
    }

    // Eventi click sui nodi
    document.querySelectorAll('.node').forEach(btn => {
        btn.addEventListener('click', () => {
            const topic = btn.dataset.topic || 'overview';
            renderTopic(topic);
        });
    });

    // Stato iniziale
    renderTopic('overview');
</script>
</body>
</html>
```
