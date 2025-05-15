<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Erweiterte Titrationssimulation</title>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/chartjs-plugin-annotation@2.2.1/dist/chartjs-plugin-annotation.min.js"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif; /* Verwendung der Inter Schrift */
            line-height: 1.6;
            margin: 20px;
            background-color: #f4f4f4;
            color: #333;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .container {
            background-color: #fff;
            padding: 25px;
            border-radius: 12px; /* Abgerundete Ecken */
            box-shadow: 0 4px 8px rgba(0,0,0,0.1); /* Verbesserter Schatten */
            max-width: 900px; /* Etwas breiter für mehr Controls */
            width: 100%;
            margin-bottom: 20px;
        }
        h1, h2 {
            color: #0056b3;
            text-align: center;
            margin-bottom: 15px;
        }
        .controls, .display {
            margin-bottom: 25px; /* Mehr Abstand */
            padding: 20px; /* Mehr Padding */
            border: 1px solid #ddd;
            border-radius: 8px; /* Abgerundete Ecken */
            background-color: #f9f9f9; /* Leichter Hintergrund */
        }
         .controls div {
             margin-bottom: 15px; /* Abstand zwischen Control-Gruppen */
        }
        .controls label {
            display: inline-block;
            margin-bottom: 8px; /* Mehr Abstand */
            font-weight: bold;
            width: 200px; /* Breite für Labels */
            vertical-align: top; /* Oben ausrichten */
        }
         .controls input[type="number"],
         .controls input[type="range"],
         .controls select {
             padding: 10px; /* Mehr Padding */
             border: 1px solid #ccc;
             border-radius: 5px; /* Abgerundete Ecken */
             margin-right: 10px;
             font-size: 1em;
        }
         .controls input[type="range"] {
             width: calc(100% - 250px); /* Slider nimmt restlichen Platz ein */
             vertical-align: top;
        }
         .controls button {
             background-color: #28a745; /* Grüne Farbe für Aktionen */
             color: white;
             padding: 12px 20px; /* Mehr Padding */
             border: none;
             border-radius: 5px; /* Abgerundete Ecken */
             cursor: pointer;
             font-size: 1.1em; /* Größere Schrift */
             margin-right: 15px; /* Mehr Abstand */
             transition: background-color 0.3s ease; /* Smooth Hover */
        }
         .controls button:hover {
             background-color: #218838;
        }
         .controls button:active {
             background-color: #1e7e34;
        }

        .display p {
            margin: 8px 0; /* Mehr Abstand */
            font-size: 1.2em; /* Größere Schrift */
            color: #0056b3; /* Akzentfarbe */
        }
         .chart-container {
             position: relative; /* Für responsive Chart */
             height: 500px; /* Feste Höhe für Chart */
             width: 100%;
        }
        #titrationChart {
            width: 100%;
            height: 100%; /* Chart füllt Container */
        }
        .checkbox-group, .select-group {
            margin-top: 15px; /* Mehr Abstand */
            padding-top: 15px;
            border-top: 1px solid #eee; /* Trennlinie */
        }
         .select-group label {
             width: auto; /* Auto Breite für Label */
             margin-right: 10px;
        }
         .explanation {
             margin-top: 20px;
             padding: 20px;
             border: 1px solid #ddd;
             border-radius: 8px;
             background-color: #e9ecef; /* Heller Hintergrund */
             font-size: 0.95em;
        }
         .explanation h3 {
             margin-top: 0;
             color: #0056b3;
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>

    <div class="container">
        <h1>Erweiterte Titrationssimulation</h1>
        <p>Simulieren Sie die Titration verschiedener Säuren mit verschiedenen Basen und erkunden Sie die Auswirkungen von Konzentrationen und Säure-/Basenstärke.</p>

        <div class="controls">
            <h2>Steuerung & Parameter</h2>
             <div>
                 <label for="acidSelect">Säure auswählen:</label>
                 <select id="acidSelect">
                     <option value="strong_acid">Starke Säure (z.B. HCl)</option>
                     <option value="acetic_acid">Schwache Säure (Essigsäure, pKs 4.76)</option>
                     <option value="formic_acid">Schwache Säure (Ameisensäure, pKs 3.75)</option>
                     <option value="hydrocyanic_acid">Schwache Säure (Blausäure, pKs 9.21)</option>
                     </select>
             </div>
             <div id="acidStrengthControls">
                 <label for="pKaInput">pKs-Wert der Säure:</label>
                 <input type="number" id="pKaInput" value="4.76" min="-2" max="14" step="0.01">
             </div>
             <div>
                 <label for="baseSelect">Base auswählen:</label>
                 <select id="baseSelect">
                     <option value="strong_base">Starke Base (z.B. NaOH)</option>
                     <option value="ammonia">Schwache Base (Ammoniak, pKb 4.75)</option>
                     </select>
             </div>
             <div id="baseStrengthControls">
                 <label for="pKbInput">pKb-Wert der Base:</label>
                 <input type="number" id="pKbInput" value="4.75" min="-2" max="14" step="0.01">
             </div>

            <div>
                <label for="initialAcidVolumeInput">Anfangs-Volumen Säure (mL):</label>
                <input type="number" id="initialAcidVolumeInput" value="20" min="10" step="10"> </div>
            <div>
                <label for="acidConcentrationInput">Konzentration Säure (mol/L):</label>
                <input type="number" id="acidConcentrationInput" value="0.1" min="0.001" step="0.001">
            </div>
             <div>
                <label for="baseConcentrationInput">Konzentration Base (mol/L):</label>
                <input type="number" id="baseConcentrationInput" value="0.1" min="0.001" step="0.001">
            </div>
             <div>
                 <label for="volumeSlider">Zugegebenes Volumen Base (mL):</label>
                 <input type="range" id="volumeSlider" min="0" max="50" value="0" step="1"> <span id="currentVolumeSpan">0.0</span> mL
             </div>

             <div class="checkbox-group">
                 <input type="checkbox" id="showConcentrations">
                 <label for="showConcentrations">Konzentrationen der Spezies anzeigen (nur schwache Säure/starke Base)</label>
             </div>
             <div class="checkbox-group">
                 <input type="checkbox" id="logScaleConcentrations">
                 <label for="logScaleConcentrations">Logarithmische Skala für Konzentrationen</label>
             </div>
             <div class="select-group">
                 <label for="indicatorSelect">pH-Indikator visualisieren:</label>
                 <select id="indicatorSelect">
                     <option value="none">Kein Indikator</option>
                     <option value="methyl_orange">Methylorange (3.1 - 4.4)</option>
                     <option value="methyl_red">Methylrot (4.4 - 6.2)</option>
                     <option value="bromothymol_blue">Bromthymolblau (6.0 - 7.6)</option>
                     <option value="phenolphthalein">Phenolphthalein (8.2 - 10.0)</option>
                 </select>
             </div>

            <button id="resetButton">Simulation zurücksetzen</button>
             </div>

        <div class="display">
            <h2>Aktuelle Werte</h2>
            <p>Aktueller pH-Wert: <span id="currentPH">-</span></p>
            <p>Zugegebenes Volumen Base: <span id="currentVolumeDisplay">-</span> mL</p>
             <p>Äquivalenzpunkt Volumen: <span id="equivalenceVolume">-</span> mL</p>
        </div>

        <div class="chart-container">
            <canvas id="titrationChart"></canvas>
        </div>

         <div class="explanation">
             <h3>Erläuterungen zur Titrationskurve</h3>
             <p>Die Form der Titrationskurve hängt stark von der Stärke der titrierten Säure und der verwendeten Base ab.</p>
             <p><strong>Starke Säure + Starke Base:</strong> Charakterisiert durch einen niedrigen Anfangs-pH, einen sehr steilen pH-Sprung am Äquivalenzpunkt (pH 7) und einen hohen pH im Überschussbereich der Base.</p>
             <p><strong>Schwache Säure + Starke Base:</strong> Höherer Anfangs-pH als bei einer starken Säure gleicher Konzentration. Vor dem Äquivalenzpunkt liegt ein Pufferbereich, in dem der pH-Wert sich nur langsam ändert ($pH = pK_s + \log\left(\frac{[A^-]}{[HA]}\right)$). Der Äquivalenzpunkt liegt bei pH > 7. Der pH-Sprung ist weniger steil.</p>
              <p><strong>Starke Säure + Schwache Base:</strong> Niedriger Anfangs-pH. Der Äquivalenzpunkt liegt bei pH < 7. Nach dem Äquivalenzpunkt gibt es einen Pufferbereich der schwachen Base und ihrer korrespondierenden Säure.</p>
              <p><strong>Schwache Säure + Schwache Base:</strong> Oft ein weniger ausgeprägter pH-Sprung. Der pH am Äquivalenzpunkt hängt von den relativen Stärken (pKs und pKb) ab.</p>
             <p><strong>Äquivalenzpunkt:</strong> Der Punkt, an dem die Stoffmenge der zugegebenen Base exakt der ursprünglichen Stoffmenge der Säure entspricht. Das Volumen der Base am Äquivalenzpunkt kann berechnet werden mit $V_{Base} \times c_{Base} = V_{Säure} \times c_{Säure}$.</p>
             <p><strong>pH-Indikatoren:</strong> Ihre Farbe ändert sich im Umschlagsbereich. Ein geeigneter Indikator hat einen Umschlagsbereich, der den pH-Sprung am Äquivalenzpunkt überlappt.</p>
             <p>Die Anzeige der Spezieskonzentrationen ist derzeit nur für die Titration einer schwachen Säure mit einer starken Base implementiert, um die Bildung des Puffers und die Änderung der Konzentrationen von HA und A⁻ zu visualisieren. Aktivieren Sie die logarithmische Skala, um sehr kleine Konzentrationen (wie H⁺ und OH⁻) besser sichtbar zu machen.</p>
         </div>
    </div>

    <script>
        // Konstanten
        const Kw = 1e-14; // Ionenprodukt des Wassers bei 25°C

        // HTML Elemente
        const acidSelect = document.getElementById('acidSelect');
        const acidStrengthControlsDiv = document.getElementById('acidStrengthControls');
        const pKaInput = document.getElementById('pKaInput');
        const baseSelect = document.getElementById('baseSelect');
        const baseStrengthControlsDiv = document.getElementById('baseStrengthControls');
        const pKbInput = document.getElementById('pKbInput');
        const initialAcidVolumeInput = document.getElementById('initialAcidVolumeInput');
        const acidConcentrationInput = document.getElementById('acidConcentrationInput');
        const baseConcentrationInput = document.getElementById('baseConcentrationInput');
        const volumeSlider = document.getElementById('volumeSlider');
        const currentVolumeSpan = document.getElementById('currentVolumeSpan');
        const currentPHSpan = document.getElementById('currentPH');
        const currentVolumeDisplaySpan = document.getElementById('currentVolumeDisplay');
        const equivalenceVolumeSpan = document.getElementById('equivalenceVolume');
        const resetButton = document.getElementById('resetButton');
        const showConcentrationsCheckbox = document.getElementById('showConcentrations');
        const concentrationsCheckboxGroup = showConcentrationsCheckbox.parentElement; // Get the parent div
        const logScaleConcentrationsCheckbox = document.getElementById('logScaleConcentrations');
        const indicatorSelect = document.getElementById('indicatorSelect');


        // Chart.js Instanz
        let titrationChart;

        // Vordefinierte Indikatoren (pH-Umschlagsbereich [Start, Ende] und Farbe)
        const indicators = {
            none: { range: null, color: null },
            methyl_orange: { range: [3.1, 4.4], color: 'rgba(255, 165, 0, 0.3)' }, // Orange transparent
            methyl_red: { range: [4.4, 6.2], color: 'rgba(255, 0, 0, 0.3)' }, // Rot transparent
            bromothymol_blue: { range: [6.0, 7.6], color: 'rgba(0, 128, 0, 0.3)' }, // Grün transparent
            phenolphthalein: { range: [8.2, 10.0], color: 'rgba(255, 192, 203, 0.4)' } // Pink transparent
        };


        // Funktion zur Berechnung des pH-Werts für die Titration
        function calculatePH(volumeBaseMl, acidType, baseType, initialAcidVolume, acidConcentration, baseConcentration, pKa, pKb) {
            const Va = initialAcidVolume / 1000; // Volumen Säure in L
            const Ca = acidConcentration; // Konzentration Säure
            const Vb = volumeBaseMl / 1000; // Volumen Base in L
            const Cb = baseConcentration; // Konzentration Base
            const totalVolume = Va + Vb; // Gesamtvolumen in L

            if (totalVolume <= 1e-12) {
                if (volumeBaseMl === 0) {
                    if (acidType === 'strong_acid') {
                        return -Math.log10(Math.max(Ca, 1e-14));
                    } else { // weak acid
                        const Ka_calc = Math.pow(10, -pKa);
                        const hPlus = (-Ka_calc + Math.sqrt(Math.max(0, Ka_calc * Ka_calc + 4 * Ka_calc * Ca))) / 2;
                        return -Math.log10(Math.max(hPlus, 1e-14));
                    }
                }
                return NaN;
            }

            const Ka = Math.pow(10, -pKa);
            const Kb = Math.pow(10, -pKb);
            const pKw = 14;
            // const pKa_Base = pKw - pKb; // Not directly used in this simplified logic path, but good for context
            // const Ka_Base = Math.pow(10, -pKa_Base); // Not directly used

            const molesAcidInitial = Va * Ca;
            const molesBaseAdded = Vb * Cb;
            const tolerance = 1e-9;

            // --- Before equivalence point ---
            if (molesBaseAdded < molesAcidInitial - tolerance) {
                if (acidType === 'strong_acid' && baseType === 'strong_base') {
                    const excessMolesH = molesAcidInitial - molesBaseAdded;
                    const concentrationH = excessMolesH / totalVolume;
                    return -Math.log10(Math.max(concentrationH, 1e-14));
                } else if (acidType !== 'strong_acid' && baseType === 'strong_base') { // Weak acid + strong base
                    const molesHA = molesAcidInitial - molesBaseAdded;
                    const molesA = molesBaseAdded;
                    if (molesHA <= 0) return NaN; // Should be caught by outer condition
                    const ratio = molesA / molesHA;
                     if (volumeBaseMl < 1e-9) { // Very beginning, effectively initial pH of weak acid
                        const Ka_calc = Math.pow(10, -pKa);
                        const hPlus_initial = (-Ka_calc + Math.sqrt(Math.max(0, Ka_calc * Ka_calc + 4 * Ka_calc * Ca))) / 2;
                        return -Math.log10(Math.max(hPlus_initial, 1e-14));
                    }
                    return pKa + Math.log10(Math.max(ratio, 1e-14));
                } else if (acidType === 'strong_acid' && baseType !== 'strong_base') { // Strong acid + weak base
                    const excessMolesAcid = molesAcidInitial - molesBaseAdded;
                    const concentrationH = excessMolesAcid / totalVolume;
                    return -Math.log10(Math.max(concentrationH, 1e-14));
                } else if (acidType !== 'strong_acid' && baseType !== 'strong_base') { // Weak acid + weak base
                    const molesHA = molesAcidInitial - molesBaseAdded;
                    const molesA = molesBaseAdded;
                    if (molesHA <= 0) return NaN;
                     if (volumeBaseMl < 1e-9) { // Very beginning
                        const Ka_calc = Math.pow(10, -pKa);
                        const hPlus_initial = (-Ka_calc + Math.sqrt(Math.max(0, Ka_calc * Ka_calc + 4 * Ka_calc * Ca))) / 2;
                        return -Math.log10(Math.max(hPlus_initial, 1e-14));
                    }
                    const ratio = molesA / molesHA;
                    return pKa + Math.log10(Math.max(ratio, 1e-14)); // Simplified
                }
            }
            // --- At equivalence point ---
            else if (Math.abs(molesBaseAdded - molesAcidInitial) < tolerance) {
                if (acidType === 'strong_acid' && baseType === 'strong_base') {
                    return 7;
                } else if (acidType !== 'strong_acid' && baseType === 'strong_base') { // Weak acid + strong base
                    const concentrationA_initial = molesAcidInitial / totalVolume;
                    const Kb_calc = Kw / Ka;
                    const ohMinus = (-Kb_calc + Math.sqrt(Math.max(0, Kb_calc * Kb_calc + 4 * Kb_calc * concentrationA_initial))) / 2;
                    return 14 - (-Math.log10(Math.max(ohMinus, 1e-14)));
                } else if (acidType === 'strong_acid' && baseType !== 'strong_base') { // Strong acid + weak base
                    const concentrationBH_initial = molesAcidInitial / totalVolume;
                    const Ka_calc = Kw / Kb;
                    const hPlus = (-Ka_calc + Math.sqrt(Math.max(0, Ka_calc * Ka_calc + 4 * Ka_calc * concentrationBH_initial))) / 2;
                    return -Math.log10(Math.max(hPlus, 1e-14));
                } else if (acidType !== 'strong_acid' && baseType !== 'strong_base') { // Weak acid + weak base
                    return 7 + 0.5 * (pKa - pKb);
                }
            }
            // --- After equivalence point ---
            else { // molesBaseAdded > molesAcidInitial + tolerance
                if (baseType === 'strong_base') { // Strong base excess
                    const excessMolesOH = molesBaseAdded - molesAcidInitial;
                    const concentrationOH = excessMolesOH / totalVolume;
                    const pOH = -Math.log10(Math.max(concentrationOH, 1e-14));
                    return 14 - pOH;
                } else if (baseType !== 'strong_base') { // Weak base excess
                    const excessMolesBase = molesBaseAdded - molesAcidInitial; // Moles of B
                    const molesBH = molesAcidInitial; // Moles of BH+ formed
                    if (excessMolesBase <= 0) { // Should not happen if truly after ÄP with weak base
                         // Fallback: if somehow molesBaseAdded is not greater, calculate as strong base excess (less accurate but avoids log(0))
                        const tempExcessOH = molesBaseAdded - molesAcidInitial;
                        if (tempExcessOH <=0) return NaN; // still problematic
                        const tempConcOH = tempExcessOH / totalVolume;
                        return 14 - (-Math.log10(Math.max(tempConcOH, 1e-14)));
                    }
                    const ratio_BH_B = molesBH / excessMolesBase; // [BH+]/[B]
                    const pOH = pKb + Math.log10(Math.max(ratio_BH_B, 1e-14));
                    return 14 - pOH;
                }
            }
            console.error(`calculatePH: Reached unhandled case for volume ${volumeBaseMl}, acidType ${acidType}, baseType ${baseType}`);
            return NaN;
        }

        // Funktion zur Berechnung der Spezieskonzentrationen (nur für schwache Säure/starke Base)
        function calculateSpeciesConcentrations(volumeBaseMl, initialAcidVolume, acidConcentration, baseConcentration, pKa) {
            const Va = initialAcidVolume / 1000;
            const Ca = acidConcentration;
            const Vb = volumeBaseMl / 1000;
            const Cb = baseConcentration;
            const totalVolume = Va + Vb;

            if (totalVolume <= 1e-12) {
                if (volumeBaseMl === 0) {
                    const Ka_calc = Math.pow(10, -pKa);
                    const hPlus = (-Ka_calc + Math.sqrt(Math.max(0, Ka_calc * Ka_calc + 4 * Ka_calc * Ca))) / 2;
                    const ohMinus = Kw / Math.max(hPlus, 1e-14);
                    const concA = hPlus;
                    const concHA = Ca - concA;
                    return { concentrationHA: Math.max(concHA, 0), concentrationA: Math.max(concA, 0), concentrationH: Math.max(hPlus, 1e-18), concentrationOH: Math.max(ohMinus, 1e-18) };
                }
                return { concentrationHA: NaN, concentrationA: NaN, concentrationH: NaN, concentrationOH: NaN };
            }

            const Ka = Math.pow(10, -pKa);
            let concentrationHA, concentrationA, concentrationH, concentrationOH;
            const molesAcidInitial = Va * Ca;
            const molesBaseAdded = Vb * Cb;
            const tolerance = 1e-9;

            if (molesBaseAdded < molesAcidInitial - tolerance) {
                concentrationHA = (molesAcidInitial - molesBaseAdded) / totalVolume;
                concentrationA = molesBaseAdded / totalVolume;
                if (concentrationA > 1e-18 && concentrationHA > 1e-18) {
                    concentrationH = Ka * concentrationHA / concentrationA;
                } else {
                    const ph = calculatePH(volumeBaseMl, 'weak_acid', 'strong_base', initialAcidVolume, acidConcentration, baseConcentration, pKa, 0);
                    if (!isNaN(ph) && isFinite(ph)) {
                        concentrationH = Math.pow(10, -ph);
                    } else {
                        concentrationH = NaN;
                    }
                }
                concentrationOH = Kw / Math.max(concentrationH, 1e-18);
            } else if (Math.abs(molesBaseAdded - molesAcidInitial) < tolerance) {
                const concentrationA_initial = molesAcidInitial / totalVolume;
                const Kb_calc = Kw / Ka;
                concentrationOH = (-Kb_calc + Math.sqrt(Math.max(0, Kb_calc * Kb_calc + 4 * Kb_calc * concentrationA_initial))) / 2;
                concentrationH = Kw / Math.max(concentrationOH, 1e-18);
                concentrationHA = concentrationOH;
                concentrationA = concentrationA_initial - concentrationOH;
            } else {
                concentrationOH = (molesBaseAdded - molesAcidInitial) / totalVolume;
                concentrationH = Kw / Math.max(concentrationOH, 1e-18);
                concentrationA = molesAcidInitial / totalVolume;
                concentrationHA = (concentrationH * concentrationA) / Ka;
                if (concentrationHA < 1e-18) concentrationHA = 0;
                if (concentrationA < 1e-18) concentrationA = 0;
            }

            concentrationH = Math.max(concentrationH, 1e-18);
            concentrationOH = Math.max(concentrationOH, 1e-18);
            concentrationHA = Math.max(concentrationHA, 0);
            concentrationA = Math.max(concentrationA, 0);

            return { concentrationHA, concentrationA, concentrationH, concentrationOH };
        }

        // Funktion zum Initialisieren des Diagramms
        function initializeChart() {
            const ctx = document.getElementById('titrationChart').getContext('2d');

            if (titrationChart) {
                titrationChart.destroy();
            }

            const concScaleType = logScaleConcentrationsCheckbox.checked ? 'logarithmic' : 'linear';

            titrationChart = new Chart(ctx, {
                type: 'line',
                data: {
                    labels: [],
                    datasets: [{
                        label: 'pH-Wert',
                        data: [],
                        borderColor: 'rgba(75, 192, 192, 1)',
                        backgroundColor: 'rgba(75, 192, 192, 0.2)',
                        borderWidth: 2,
                        pointRadius: 0,
                        fill: false,
                        yAxisID: 'y-ph',
                        tension: 0.1
                    },
                    {
                        label: '[HA]', data: [], borderColor: 'rgba(255, 99, 132, 1)', backgroundColor: 'rgba(255, 99, 132, 0.2)',
                        borderWidth: 2, pointRadius: 0, fill: false, hidden: true, yAxisID: 'y-conc', tension: 0.1
                    },
                    {
                        label: '[A⁻]', data: [], borderColor: 'rgba(54, 162, 235, 1)', backgroundColor: 'rgba(54, 162, 235, 0.2)',
                        borderWidth: 2, pointRadius: 0, fill: false, hidden: true, yAxisID: 'y-conc', tension: 0.1
                    },
                    {
                        label: '[H⁺]', data: [], borderColor: 'rgba(255, 205, 86, 1)', backgroundColor: 'rgba(255, 205, 86, 0.2)',
                        borderWidth: 2, pointRadius: 0, fill: false, hidden: true, yAxisID: 'y-conc', tension: 0.1
                    },
                    {
                        label: '[OH⁻]', data: [], borderColor: 'rgba(153, 102, 255, 1)', backgroundColor: 'rgba(153, 102, 255, 0.2)',
                        borderWidth: 2, pointRadius: 0, fill: false, hidden: true, yAxisID: 'y-conc', tension: 0.1
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: {
                        x: {
                            title: { display: true, text: 'Zugegebenes Volumen Base (mL)' },
                            type: 'linear',
                            position: 'bottom',
                            min: 0,
                            max: parseFloat(volumeSlider.max)
                        },
                        'y-ph': {
                            title: { display: true, text: 'pH-Wert' },
                            min: 0,
                            max: 14,
                            position: 'left',
                            grid: { drawOnChartArea: true }
                        },
                        'y-conc': {
                            title: { display: true, text: 'Konzentration (mol/L)', color: 'rgba(0,0,0,0.5)' },
                            position: 'right',
                            min: concScaleType === 'logarithmic' ? 1e-14 : 0,
                            max: parseFloat(acidConcentrationInput.value) * 1.2,
                            type: concScaleType,
                            grid: { drawOnChartArea: false },
                            ticks: {
                                color: 'rgba(0,0,0,0.5)',
                                callback: function(value) {
                                    if (concScaleType === 'logarithmic') {
                                        if (value <= 1e-18) return '0';
                                        return value.toExponential(0);
                                    }
                                    return value.toPrecision(2); // More general precision
                                }
                            },
                            display: false
                        }
                    },
                    plugins: {
                        legend: { display: true },
                        tooltip: { enabled: true },
                        annotation: { // Configuration for chartjs-plugin-annotation v2.x
                            annotations: {} // Initialize as an empty object
                        }
                    }
                }
            });
            // Check if plugin is registered (for v2.x, it's usually automatic)
            if (Chart.registry && Chart.registry.plugins.get('annotation')) {
                 console.log("Chartjs Annotation Plugin (v2.x style) is registered.");
            } else {
                 console.warn("Chartjs Annotation Plugin (v2.x style) may NOT be registered correctly.");
            }
        }

        // Funktion zum Aktualisieren des Diagramms und der Anzeigen
        function updateSimulation(volumeMl) {
            const acidType = acidSelect.value;
            const baseType = baseSelect.value;
            const initialAcidVolume = parseFloat(initialAcidVolumeInput.value);
            const acidConcentration = parseFloat(acidConcentrationInput.value);
            const baseConcentration = parseFloat(baseConcentrationInput.value);
            const pKa = parseFloat(pKaInput.value);
            const pKb = parseFloat(pKbInput.value);

            if (isNaN(initialAcidVolume) || initialAcidVolume <= 0 || isNaN(acidConcentration) || acidConcentration <= 0 || isNaN(baseConcentration) || baseConcentration <= 0) {
                console.error("Invalid input parameters detected. Cannot update simulation.");
                currentPHSpan.textContent = 'Ungültige Parameter';
                equivalenceVolumeSpan.textContent = 'Ungültige Parameter';
                if(titrationChart) {
                    titrationChart.data.labels = [];
                    titrationChart.data.datasets.forEach(dataset => dataset.data = []);
                    titrationChart.update();
                }
                return;
            }

            const equivalenceVolume = (initialAcidVolume * acidConcentration / baseConcentration);
            equivalenceVolumeSpan.textContent = (!isNaN(equivalenceVolume) && isFinite(equivalenceVolume)) ? equivalenceVolume.toFixed(2) : 'Ungültige Parameter';
            
            if(!titrationChart) {
                console.error("Chart not initialized in updateSimulation.");
                initializeChart(); // Attempt to initialize if not present
                if(!titrationChart) return; // Exit if still not initialized
            }

            titrationChart.data.labels = [];
            titrationChart.data.datasets.forEach(dataset => dataset.data = []);

            const step = 0.5;
            const fineStep = 0.05; // Adjusted fine step for smoother curve near equivalence
            const fineRange = 1.5; // Adjusted range for fine steps

            const volumesToCalculate = [];
            let currentVol = 0;
            while(currentVol <= volumeMl + 1e-9) { // Ensure the final volume is included or very close
                volumesToCalculate.push(currentVol);
                let actualStep = step;
                if (!isNaN(equivalenceVolume) && isFinite(equivalenceVolume)) {
                    if (Math.abs(currentVol - equivalenceVolume) < fineRange) {
                         actualStep = fineStep;
                    }
                }
                currentVol += actualStep;
                if (actualStep < 1e-9) break; // Safety break for extremely small steps
            }
             // Ensure the exact final volume (volumeMl) is included if the loop didn't hit it precisely
            if (volumesToCalculate.length === 0 || Math.abs(volumesToCalculate[volumesToCalculate.length - 1] - volumeMl) > 1e-9 && volumeMl > (volumesToCalculate[volumesToCalculate.length -1] || 0) ) {
                 volumesToCalculate.push(volumeMl);
            }
             // Sort volumes to ensure they are in ascending order, important if volumeMl was pushed separately
            volumesToCalculate.sort((a, b) => a - b);
            // Remove duplicates that might arise from floating point issues
            const uniqueVolumes = [...new Set(volumesToCalculate.map(v => parseFloat(v.toFixed(3))))];


            uniqueVolumes.forEach(vol => {
                const ph = calculatePH(vol, acidType, baseType, initialAcidVolume, acidConcentration, baseConcentration, pKa, pKb);
                titrationChart.data.labels.push(vol.toFixed(1));

                if (isNaN(ph) || !isFinite(ph)) {
                    titrationChart.data.datasets[0].data.push(NaN);
                } else {
                    titrationChart.data.datasets[0].data.push(ph);
                    if (acidType !== 'strong_acid' && baseType === 'strong_base') {
                        const concentrations = calculateSpeciesConcentrations(vol, initialAcidVolume, acidConcentration, baseConcentration, pKa);
                        titrationChart.data.datasets[1].data.push((!isNaN(concentrations.concentrationHA) && isFinite(concentrations.concentrationHA)) ? concentrations.concentrationHA : NaN);
                        titrationChart.data.datasets[2].data.push((!isNaN(concentrations.concentrationA) && isFinite(concentrations.concentrationA)) ? concentrations.concentrationA : NaN);
                        titrationChart.data.datasets[3].data.push((!isNaN(concentrations.concentrationH) && isFinite(concentrations.concentrationH)) ? concentrations.concentrationH : NaN);
                        titrationChart.data.datasets[4].data.push((!isNaN(concentrations.concentrationOH) && isFinite(concentrations.concentrationOH)) ? concentrations.concentrationOH : NaN);
                    } else {
                        [1, 2, 3, 4].forEach(i => titrationChart.data.datasets[i].data.push(NaN));
                    }
                }
            });

            currentVolumeSpan.textContent = volumeMl.toFixed(1);
            currentVolumeDisplaySpan.textContent = volumeMl.toFixed(1);
            
            let lastValidPH = NaN;
            const phData = titrationChart.data.datasets[0].data;
            for(let i = phData.length - 1; i >= 0; i--) {
                if (!isNaN(phData[i]) && isFinite(phData[i])) {
                    lastValidPH = phData[i];
                    break;
                }
            }
            currentPHSpan.textContent = isNaN(lastValidPH) ? '-' : lastValidPH.toFixed(2);
            
            titrationChart.update();
        }

        // Funktion zum Zurücksetzen der Simulation
        function resetSimulation() {
            console.log("Resetting simulation...");
            volumeSlider.value = 0;
            currentVolumeSpan.textContent = '0.0';
            currentVolumeDisplaySpan.textContent = '0.0';
            currentPHSpan.textContent = '-';

            if(!titrationChart) {
                initializeChart();
                 if(!titrationChart) {
                     console.error("Chart initialization failed during reset.");
                     return;
                 }
            }
            
            titrationChart.data.labels = [];
            titrationChart.data.datasets.forEach(dataset => dataset.data = []);

            const acidType = acidSelect.value;
            const baseType = baseSelect.value;
            const initialAcidVolume = parseFloat(initialAcidVolumeInput.value);
            const acidConcentration = parseFloat(acidConcentrationInput.value);
            const baseConcentration = parseFloat(baseConcentrationInput.value);
            const pKa = parseFloat(pKaInput.value);
            const pKb = parseFloat(pKbInput.value);

            if (!isNaN(initialAcidVolume) && initialAcidVolume > 0 && !isNaN(acidConcentration) && acidConcentration > 0 && !isNaN(baseConcentration) && baseConcentration > 0) {
                const initialPH = calculatePH(0, acidType, baseType, initialAcidVolume, acidConcentration, baseConcentration, pKa, pKb);
                if (!isNaN(initialPH) && isFinite(initialPH)) {
                    titrationChart.data.labels.push('0.0');
                    titrationChart.data.datasets[0].data.push(initialPH);
                    currentPHSpan.textContent = initialPH.toFixed(2);

                    if (acidType !== 'strong_acid' && baseType === 'strong_base') {
                        const initialConcs = calculateSpeciesConcentrations(0, initialAcidVolume, acidConcentration, baseConcentration, pKa);
                        titrationChart.data.datasets[1].data.push((!isNaN(initialConcs.concentrationHA) && isFinite(initialConcs.concentrationHA)) ? initialConcs.concentrationHA : NaN);
                        titrationChart.data.datasets[2].data.push((!isNaN(initialConcs.concentrationA) && isFinite(initialConcs.concentrationA)) ? initialConcs.concentrationA : NaN);
                        titrationChart.data.datasets[3].data.push((!isNaN(initialConcs.concentrationH) && isFinite(initialConcs.concentrationH)) ? initialConcs.concentrationH : NaN);
                        titrationChart.data.datasets[4].data.push((!isNaN(initialConcs.concentrationOH) && isFinite(initialConcs.concentrationOH)) ? initialConcs.concentrationOH : NaN);
                    } else {
                         [1, 2, 3, 4].forEach(i => titrationChart.data.datasets[i].data.push(NaN));
                    }
                } else {
                    currentPHSpan.textContent = 'Fehler bei Anfangs-pH';
                }
            } else {
                currentPHSpan.textContent = 'Ungültige Parameter';
            }

            const equivalenceVolume = (initialAcidVolume * acidConcentration / baseConcentration);
            equivalenceVolumeSpan.textContent = (!isNaN(equivalenceVolume) && isFinite(equivalenceVolume)) ? equivalenceVolume.toFixed(2) : 'Ungültige Parameter';
            
            // Update X-axis max based on current slider settings or a default like 50
            const sliderMax = parseFloat(volumeSlider.max) || 50;
            titrationChart.options.scales.x.max = sliderMax;


            titrationChart.update();
            console.log("Simulation reset complete.");
            updateIndicatorAnnotation(); // Update indicator after reset and chart update
        }

        // Funktion zum Hinzufügen von Indikator-Annotationen (angepasst für chartjs-plugin-annotation v2.x)
        function updateIndicatorAnnotation() {
            if (!titrationChart || !titrationChart.options || !titrationChart.options.plugins || !titrationChart.options.plugins.annotation) {
                console.error("Chart or annotation plugin options not initialized. Cannot update indicator annotations.");
                return;
            }

            const selectedIndicator = indicatorSelect.value;
            const indicatorData = indicators[selectedIndicator];
            const newAnnotations = {}; // For v2.x, annotations are an object with keys

            if (indicatorData && indicatorData.range) {
                const [phStart, phEnd] = indicatorData.range;
                const color = indicatorData.color;
                const xAxis = titrationChart.scales.x; // Get the x-axis scale

                if (!xAxis) {
                    console.error("X-axis scale not found. Cannot set annotation xMin/xMax accurately.");
                    // Fallback or skip annotation
                } else {
                     newAnnotations.indicatorRange = { // Use a unique key for the annotation
                        type: 'box',
                        xScaleID: 'x',       // ID of the X scale
                        yScaleID: 'y-ph',    // ID of the Y scale for pH
                        yMin: phStart,       // Bottom edge of the box (pH start)
                        yMax: phEnd,         // Top edge of the box (pH end)
                        xMin: xAxis.min,     // Left edge of the box (start of x-axis)
                        xMax: xAxis.max,     // Right edge of the box (end of x-axis)
                        backgroundColor: color,
                        borderColor: 'rgba(0,0,0,0)', // No visible border
                        borderWidth: 0,
                        drawTime: 'beforeDatasetsDraw' // Draw annotation before dataset lines
                    };
                    console.log("Setting indicator annotation (v2 format):", newAnnotations.indicatorRange);
                }
            } else {
                console.log("No indicator selected or range undefined, clearing annotations (v2 format).");
            }

            titrationChart.options.plugins.annotation.annotations = newAnnotations; // Assign the new set of annotations
            titrationChart.update();
        }

        // Event Listener für den Slider
        volumeSlider.addEventListener('input', (event) => {
            const volume = parseFloat(event.target.value);
            updateSimulation(volume);
        });

        resetButton.addEventListener('click', resetSimulation);

        acidSelect.addEventListener('change', (event) => {
            if (event.target.value !== 'strong_acid') {
                acidStrengthControlsDiv.style.display = 'block';
                if (event.target.value === 'acetic_acid') pKaInput.value = '4.76';
                else if (event.target.value === 'formic_acid') pKaInput.value = '3.75';
                else if (event.target.value === 'hydrocyanic_acid') pKaInput.value = '9.21';
            } else {
                acidStrengthControlsDiv.style.display = 'none';
            }
            updateConcentrationsCheckboxVisibility();
            resetSimulation();
        });

        baseSelect.addEventListener('change', (event) => {
            if (event.target.value !== 'strong_base') {
                baseStrengthControlsDiv.style.display = 'block';
                if (event.target.value === 'ammonia') pKbInput.value = '4.75';
            } else {
                baseStrengthControlsDiv.style.display = 'none';
            }
            updateConcentrationsCheckboxVisibility();
            resetSimulation();
        });

        function updateConcentrationsCheckboxVisibility() {
            const acidType = acidSelect.value;
            const baseType = baseSelect.value;
            if (acidType !== 'strong_acid' && baseType === 'strong_base') {
                concentrationsCheckboxGroup.style.display = 'block';
            } else {
                concentrationsCheckboxGroup.style.display = 'none';
                showConcentrationsCheckbox.checked = false; // Uncheck and hide datasets if condition not met
                if (titrationChart) { // Ensure chart exists
                    [1, 2, 3, 4].forEach(i => titrationChart.data.datasets[i].hidden = true);
                    titrationChart.options.scales['y-conc'].display = false;
                    // No need to call titrationChart.update() here, resetSimulation or other updates will handle it.
                }
            }
             // Call resetSimulation to re-evaluate everything, including chart data and scales
            if (titrationChart) resetSimulation(); // Or a more targeted update if preferred
        }

        logScaleConcentrationsCheckbox.addEventListener('change', () => {
            // Re-initialize chart to apply new scale type, then update data
            initializeChart(); 
            updateSimulation(parseFloat(volumeSlider.value));
            updateIndicatorAnnotation(); // Also update indicator
            if(titrationChart) {
                 titrationChart.options.scales['y-conc'].display = showConcentrationsCheckbox.checked && (acidSelect.value !== 'strong_acid' && baseSelect.value === 'strong_base');
                 titrationChart.update();
            }
        });

        [initialAcidVolumeInput, acidConcentrationInput, baseConcentrationInput, pKaInput, pKbInput].forEach(input => {
            input.addEventListener('change', resetSimulation);
        });
        
        showConcentrationsCheckbox.addEventListener('change', (event) => {
            if(!titrationChart) return;
            const isHidden = !event.target.checked;
            [1, 2, 3, 4].forEach(i => titrationChart.data.datasets[i].hidden = isHidden);
            titrationChart.options.scales['y-conc'].display = !isHidden;
            titrationChart.update();
        });

        indicatorSelect.addEventListener('change', updateIndicatorAnnotation);

        window.onload = () => {
            // Set default selections first
            acidSelect.value = 'acetic_acid'; 
            baseSelect.value = 'strong_base'; 
            
            // Initialize chart structure (scales, datasets etc.)
            initializeChart(); 
            
            // Update visibility of controls based on defaults
            acidStrengthControlsDiv.style.display = (acidSelect.value !== 'strong_acid') ? 'block' : 'none';
            if (acidSelect.value === 'acetic_acid') pKaInput.value = '4.76'; // Ensure pKa is set for default weak acid
            
            baseStrengthControlsDiv.style.display = (baseSelect.value !== 'strong_base') ? 'block' : 'none';
             if (baseSelect.value === 'ammonia') pKbInput.value = '4.75';


            updateConcentrationsCheckboxVisibility(); // This will also call resetSimulation if chart exists

            // Call resetSimulation explicitly if updateConcentrationsCheckboxVisibility doesn't (e.g., if chart wasn't ready)
            // resetSimulation will calculate initial pH, equivalence point, and update the chart.
            if (!titrationChart) { // If chart wasn't initialized by updateConcentrationsCheckboxVisibility
                resetSimulation();
            }
            // Ensure indicator annotation is called after the chart is fully set up by resetSimulation
             updateIndicatorAnnotation();
        };
    </script>
</body>
</html>
