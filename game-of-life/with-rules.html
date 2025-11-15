<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Game of Life</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #000;
      color: #0f0;
      font-family: 'Courier New', monospace;
      overflow: hidden;
      height: 100vh;
    }

    #container {
      display: flex;
      height: 100vh;
    }

    #canvas-wrapper {
      flex: 1;
      position: relative;
      cursor: grab;
    }

    #canvas-wrapper.grabbing {
      cursor: grabbing;
    }

    canvas {
      display: block;
      width: 100%;
      height: 100%;
    }

    #controls {
      width: 280px;
      background: #111;
      padding: 20px;
      border-left: 2px solid #0f0;
      overflow-y: auto;
      transition: transform 0.3s ease;
    }

    #controls.hidden {
      transform: translateX(100%);
      position: absolute;
      right: 0;
      height: 100vh;
    }

    #fullscreen-exit {
      position: fixed;
      top: 20px;
      right: 20px;
      padding: 10px 20px;
      background: #000;
      color: #0f0;
      border: 2px solid #0f0;
      cursor: pointer;
      font-family: 'Courier New', monospace;
      font-size: 14px;
      z-index: 1000;
      display: none;
    }

    #fullscreen-exit:hover {
      background: #0f0;
      color: #000;
    }

    h2 {
      color: #0f0;
      margin-bottom: 15px;
      font-size: 18px;
      border-bottom: 1px solid #0f0;
      padding-bottom: 5px;
    }

    .control-group {
      margin-bottom: 20px;
    }

    button {
      width: 100%;
      padding: 10px;
      margin-bottom: 8px;
      background: #000;
      color: #0f0;
      border: 2px solid #0f0;
      cursor: pointer;
      font-family: 'Courier New', monospace;
      font-size: 14px;
      transition: all 0.2s;
    }

    button:hover {
      background: #0f0;
      color: #000;
    }

    button:active {
      transform: scale(0.98);
    }

    .speed-control {
      display: flex;
      align-items: center;
      margin-bottom: 10px;
    }

    .speed-control label {
      flex: 1;
      font-size: 14px;
    }

    .speed-control input {
      width: 60px;
      padding: 5px;
      background: #000;
      color: #0f0;
      border: 1px solid #0f0;
      font-family: 'Courier New', monospace;
    }

    .checkbox-control {
      margin: 10px 0;
    }

    .checkbox-control label {
      display: flex;
      align-items: center;
      cursor: pointer;
      font-size: 13px;
    }

    .checkbox-control input[type="checkbox"] {
      margin-right: 10px;
      width: 16px;
      height: 16px;
      cursor: pointer;
      accent-color: #0f0;
    }

    .stats,
    .control-group {
      margin-top: 20px;
    }

    .stat-row {
      display: flex;
      justify-content: space-between;
      padding: 6px 0;
      border-bottom: 1px solid #333;
      font-size: 13px;
    }

    .stat-label {
      color: #0a0;
    }

    .stat-value {
      color: #0f0;
      font-weight: bold;
    }

    .info {
      margin-top: 15px;
      padding: 10px;
      background: #0a0a0a;
      border: 1px solid #0f0;
      font-size: 11px;
      color: #0a0;
    }

    .info p {
      margin-bottom: 5px;
    }

    .controls-container {
      position: absolute;
      top: 2px;
      right: 20px;
      z-index: 1000;
      width: 38px;
      opacity: 0.25;
      transition: opacity 0.3s;
    }

    .controls-container:hover {
      opacity: 1;
    }

    .rule-option {
      margin: 8px 0;
    }

    .rule-option label {
      display: flex;
      align-items: center;
      cursor: pointer;
      font-size: 13px;
      padding: 8px;
      border: 1px solid #333;
      border-radius: 3px;
      transition: all 0.2s;
    }

    .rule-option label:hover {
      border-color: #0f0;
      background: #001100;
    }

    .rule-option input[type="radio"] {
      margin-right: 10px;
      width: 16px;
      height: 16px;
      cursor: pointer;
      accent-color: #0f0;
    }

    .rule-option label.selected {
      border-color: #0f0;
      background: #002200;
    }

    .rule-description {
      margin-top: 10px;
      padding: 10px;
      background: #0a0a0a;
      border: 1px solid #0f0;
      font-size: 11px;
      color: #0a0;
      border-radius: 3px;
    }

    .rule-description h4 {
      color: #0f0;
      margin-bottom: 5px;
      font-size: 12px;
    }

    .color-customization {
      margin-top: 15px;
      padding: 10px;
      background: #0a0a0a;
      border: 1px solid #0f0;
      border-radius: 3px;
    }

    .color-customization h3 {
      color: #0f0;
      margin-bottom: 10px;
      font-size: 14px;
      border-bottom: 1px solid #333;
      padding-bottom: 5px;
    }

    .color-control {
      display: flex;
      align-items: center;
      margin-bottom: 8px;
    }

    .color-control label {
      flex: 1;
      font-size: 12px;
      color: #0a0;
    }

    .color-control input[type="color"] {
      width: 40px;
      height: 25px;
      border: 1px solid #0f0;
      background: #000;
      cursor: pointer;
      border-radius: 3px;
    }

    .color-control input[type="color"]::-webkit-color-swatch-wrapper {
      padding: 0;
    }

    .color-control input[type="color"]::-webkit-color-swatch {
      border: none;
      border-radius: 2px;
    }

    .color-section {
      margin-bottom: 12px;
      padding: 8px;
      background: #0a0a0a;
      border: 1px solid #333;
      border-radius: 3px;
    }

    .color-section h4 {
      color: #0f0;
      font-size: 11px;
      margin-bottom: 6px;
      text-transform: uppercase;
    }
  </style>
</head>

<body>
  <div id="container">
    <div id="canvas-wrapper">
      <canvas id="gameCanvas"></canvas>
    </div>
    <div class="controls-container">
      <button id="controls-toggler">x</button>
    </div>
    <div id="controls">
      <h2>CONTROLS</h2>
      <div class="control-group">
        <button id="startBtn">START</button>
        <button id="stopBtn">STOP</button>
        <button id="clearBtn">CLEAR</button>
        <button id="randomBtn">RANDOM SEED</button>
        <button id="fullscreenBtn">FULLSCREEN</button>
      </div>

      <div class="control-group">
        <h2>SPEED</h2>
        <div class="speed-control">
          <label>Gen/sec:</label>
          <input type="number" id="speedInput" value="10" min="1" max="60">
        </div>
      </div>

      <div class="control-group">
        <h2>VIEW OPTIONS</h2>
        <div class="checkbox-control">
          <label>
            <input type="checkbox" id="gridToggle" checked>
            Show Grid Borders
          </label>
        </div>
      </div>

      <div class="control-group">
        <h2>RULES</h2>
        <div class="rule-option">
          <label>
            <input type="radio" name="rule" id="classicRule" value="classic" checked>
            Classic Green
          </label>
        </div>
        <div class="rule-option">
          <label>
            <input type="radio" name="rule" id="neighborColorRule" value="neighborColor">
            Neighbor Color Coding
          </label>
        </div>
        <div class="rule-option">
          <label>
            <input type="radio" name="rule" id="ageBasedRule" value="ageBased">
            Cell Age & Size
          </label>
        </div>
        <div class="rule-option">
          <label>
            <input type="radio" name="rule" id="densityRule" value="density">
            Population Density
          </label>
        </div>
        <div class="rule-option">
          <label>
            <input type="radio" name="rule" id="heatmapRule" value="heatmap">
            Activity Heatmap
          </label>
        </div>
        <div class="rule-option">
          <label>
            <input type="radio" name="rule" id="ghostRule" value="ghost">
            Ghost Trail
          </label>
        </div>
        <div class="rule-description" id="ruleDescription">
          <h4>Classic Green</h4>
          <p>Traditional Conway's Game of Life appearance with all living cells displayed in bright green. Simple and classic visualization.</p>
        </div>
        
        <div class="color-customization" id="colorCustomization" style="display: block;">
          <h3>Color Customization</h3>
          <div id="colorControlsContainer">
            <!-- Dynamic color controls will be inserted here -->
          </div>
        </div>
      </div>

      <div class="stats">
        <h2>STATISTICS</h2>
        <div class="stat-row">
          <span class="stat-label">Generation:</span>
          <span class="stat-value" id="generation">0</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">Initial Cells:</span>
          <span class="stat-value" id="initialCells">0</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">Current Population:</span>
          <span class="stat-value" id="liveCells">0</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">Population Change:</span>
          <span class="stat-value" id="popChange">0</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">Peak Population:</span>
          <span class="stat-value" id="peakPop">0</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">Births This Gen:</span>
          <span class="stat-value" id="births">0</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">Deaths This Gen:</span>
          <span class="stat-value" id="deaths">0</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">Total Births:</span>
          <span class="stat-value" id="totalBirths">0</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">Total Deaths:</span>
          <span class="stat-value" id="totalDeaths">0</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">Stability:</span>
          <span class="stat-value" id="stability">-</span>
        </div>
      </div>

      <div class="control-group">
        <h2>PATTERNS</h2>
        <div id="patternsContainer"></div>
      </div>

      <div class="info">
        <p><strong>INSTRUCTIONS:</strong></p>
        <p>• Click cells to toggle</p>
        <p>• Drag to pan</p>
        <p>• Scroll to zoom</p>
        <p>• Space to start/stop</p>
      </div>
    </div>
  </div>

  <script type="module">
    import { patterns } from './patterns.js';
    const canvas = document.getElementById('gameCanvas');
    const ctx = canvas.getContext('2d');
    const wrapper = document.getElementById('canvas-wrapper');

    // State
    let grid = new Map();
    let running = false;
    let cellSize = 20;
    let offsetX = 0;
    let offsetY = 0;
    let lastTime = 0;
    let speed = 10;
    let generation = 0;
    let initialCellCount = 0;
    let peakPopulation = 0;
    let totalBirths = 0;
    let totalDeaths = 0;
    let birthsThisGen = 0;
    let deathsThisGen = 0;
    let previousPopulation = 0;
    let stabilityCounter = 0;
    let showGrid = true;
    let currentRule = 'classic';
    
    // Color customization for each rule
    let ruleColors = {
      classic: {
        cellColor: '#00ff00',
        gridColor: '#333333',
        bgColor: '#000000'
      },
      neighborColor: {
        neighbor0: '#ff0000', // 0 neighbors - red (dying)
        neighbor1: '#ff4400', // 1 neighbor - red-orange
        neighbor2: '#00ff00', // 2 neighbors - green (stable)
        neighbor3: '#00ff00', // 3 neighbors - green (stable/birth)
        neighbor4: '#ffff00', // 4 neighbors - yellow
        neighbor5: '#ff8800', // 5 neighbors - orange
        neighbor6: '#ff4400', // 6 neighbors - red-orange
        neighbor7: '#ff0000', // 7 neighbors - red
        neighbor8: '#8800ff', // 8 neighbors - purple (overcrowded)
        gridColor: '#333333',
        bgColor: '#000000'
      },
      ageBased: {
        youngColor: '#00ff00', // Young cells - bright green
        oldColor: '#ff0000',   // Old cells - red
        gridColor: '#333333',
        bgColor: '#000000'
      },
      density: {
        sparseColor: '#0080ff',    // Blue - sparse
        normalColor: '#00ff80',    // Green - normal
        crowdedColor: '#ffff00',   // Yellow - crowded
        denseColor: '#ff8000',     // Orange - dense
        overcrowdedColor: '#ff0000', // Red - overcrowded
        gridColor: '#333333',
        bgColor: '#000000'
      },
      heatmap: {
        coldColor: '#0000ff',    // Blue - low activity
        warmColor: '#ffff00',    // Yellow - medium activity
        hotColor: '#ff0000',     // Red - high activity
        gridColor: '#333333',
        bgColor: '#000000'
      },
      ghost: {
        aliveColor: '#00ffff',   // Cyan - living cells
        deadColor: '#666666',    // Gray - ghost trails
        gridColor: '#333333',
        bgColor: '#000000'
      }
    };
    let cellAges = new Map(); // Track age of each cell
    let populationDensityMap = new Map(); // Track local density
    let cellActivity = new Map(); // Track cell activity for heatmap
    let deadCells = new Map(); // Track recently dead cells for ghost effect
    let animationTime = 0; // For pulse animations
    let particleTrails = new Map(); // Track particle trails
    let wavePhases = new Map(); // Track wave phases for cells
    let cellDirections = new Map(); // Track movement directions

    // Panning
    let isDragging = false;
    let dragStartX = 0;
    let dragStartY = 0;
    let dragOffsetX = 0;
    let dragOffsetY = 0;

    function resize() {
      canvas.width = wrapper.clientWidth;
      canvas.height = wrapper.clientHeight;
      draw();
    }

    function getCellKey(x, y) {
      return `${x},${y}`;
    }

    function parseCellKey(key) {
      const [x, y] = key.split(',').map(Number);
      return { x, y };
    }

    function getColorByNeighborCount(neighborCount) {
      const colors = ruleColors.neighborColor;
      const colorKeys = ['neighbor0', 'neighbor1', 'neighbor2', 'neighbor3', 'neighbor4', 'neighbor5', 'neighbor6', 'neighbor7', 'neighbor8'];
      return colors[colorKeys[neighborCount]] || '#0f0';
    }

    function getAgeBasedProperties(age) {
      // Younger cells are smaller and brighter, older cells are larger and dimmer
      const maxAge = 20;
      const normalizedAge = Math.min(age, maxAge) / maxAge;
      
      // Interpolate between young and old colors
      const youngColor = hexToRgb(ruleColors.ageBased.youngColor);
      const oldColor = hexToRgb(ruleColors.ageBased.oldColor);
      
      const r = Math.round(youngColor.r + (oldColor.r - youngColor.r) * normalizedAge);
      const g = Math.round(youngColor.g + (oldColor.g - youngColor.g) * normalizedAge);
      const b = Math.round(youngColor.b + (oldColor.b - youngColor.b) * normalizedAge);
      
      return {
        color: `rgb(${r}, ${g}, ${b})`,
        sizeMultiplier: 0.6 + (normalizedAge * 0.4) // Size grows from 60% to 100%
      };
    }

    function getDensityBasedProperties(density) {
      const colors = ruleColors.density;
      // Colors based on local population density in 5x5 area
      if (density <= 2) return { color: colors.sparseColor, alpha: 0.7 }; // Blue - sparse
      if (density <= 5) return { color: colors.normalColor, alpha: 0.8 }; // Green - normal
      if (density <= 8) return { color: colors.crowdedColor, alpha: 0.9 }; // Yellow - crowded
      if (density <= 12) return { color: colors.denseColor, alpha: 1.0 }; // Orange - dense
      return { color: colors.overcrowdedColor, alpha: 1.0 }; // Red - overcrowded
    }

    function calculateLocalDensity(x, y) {
      let count = 0;
      // Check 5x5 area around cell
      for (let dx = -2; dx <= 2; dx++) {
        for (let dy = -2; dy <= 2; dy++) {
          if (grid.has(getCellKey(x + dx, y + dy))) count++;
        }
      }
      return count;
    }



    function getHeatmapProperties(activity) {
      // Activity-based coloring (0-100 scale)
      const normalizedActivity = Math.min(activity, 100) / 100;
      const colors = ruleColors.heatmap;
      
      let color;
      if (normalizedActivity < 0.5) {
        // Interpolate between cold and warm
        const coldColor = hexToRgb(colors.coldColor);
        const warmColor = hexToRgb(colors.warmColor);
        const t = normalizedActivity * 2;
        const r = Math.round(coldColor.r + (warmColor.r - coldColor.r) * t);
        const g = Math.round(coldColor.g + (warmColor.g - coldColor.g) * t);
        const b = Math.round(coldColor.b + (warmColor.b - coldColor.b) * t);
        color = `rgb(${r}, ${g}, ${b})`;
      } else {
        // Interpolate between warm and hot
        const warmColor = hexToRgb(colors.warmColor);
        const hotColor = hexToRgb(colors.hotColor);
        const t = (normalizedActivity - 0.5) * 2;
        const r = Math.round(warmColor.r + (hotColor.r - warmColor.r) * t);
        const g = Math.round(warmColor.g + (hotColor.g - warmColor.g) * t);
        const b = Math.round(warmColor.b + (hotColor.b - warmColor.b) * t);
        color = `rgb(${r}, ${g}, ${b})`;
      }
      
      return {
        color: color,
        alpha: 0.6 + (normalizedActivity * 0.4)
      };
    }



    function getGhostProperties(isAlive, age, deadAge) {
      const colors = ruleColors.ghost;
      if (isAlive) {
        return {
          color: colors.aliveColor,
          alpha: 0.9
        };
      } else {
        // Ghost trail for dead cells
        const fadeTime = 10;
        const alpha = Math.max(0, (fadeTime - deadAge) / fadeTime);
        return {
          color: colors.deadColor,
          alpha: alpha * 0.3,
          sizeMultiplier: 1 - (deadAge / fadeTime) * 0.5
        };
      }
    }











    function hexToRgb(hex) {
      const result = /^#?([a-f\d]{2})([a-f\d]{2})([a-f\d]{2})$/i.exec(hex);
      return result ? {
        r: parseInt(result[1], 16),
        g: parseInt(result[2], 16),
        b: parseInt(result[3], 16)
      } : null;
    }

    function calculateSurfaceTension(x, y) {
      let edges = 0;
      for (let dx = -1; dx <= 1; dx++) {
        for (let dy = -1; dy <= 1; dy++) {
          if (dx === 0 && dy === 0) continue;
          if (!grid.has(getCellKey(x + dx, y + dy))) edges++;
        }
      }
      return edges / 8;
    }



    function toggleCell(x, y) {
      const key = getCellKey(x, y);
      if (grid.has(key)) {
        grid.delete(key);
        cellAges.delete(key);
      } else {
        grid.set(key, true);
        cellAges.set(key, 0); // New cells start at age 0
      }

      const currentPattern = Array.from(grid.keys()).map(k => parseCellKey(k));
      console.log("Current Pattern:", JSON.stringify(currentPattern.map(({ x, y }) => [x, y])));

      if (!running && generation === 0) {
        initialCellCount = grid.size;
        updateStats();
      }
      draw();
    }

    function getNeighbors(x, y) {
      let count = 0;
      for (let dx = -1; dx <= 1; dx++) {
        for (let dy = -1; dy <= 1; dy++) {
          if (dx === 0 && dy === 0) continue;
          if (grid.has(getCellKey(x + dx, y + dy))) count++;
        }
      }
      return count;
    }

    function nextGeneration() {
      const newGrid = new Map();
      const toCheck = new Set();

      // Add all live cells and their neighbors to check list
      for (const key of grid.keys()) {
        const { x, y } = parseCellKey(key);
        for (let dx = -1; dx <= 1; dx++) {
          for (let dy = -1; dy <= 1; dy++) {
            toCheck.add(getCellKey(x + dx, y + dy));
          }
        }
      }

      const prevPopulation = grid.size;
      let births = 0;
      let deaths = 0;

      // Apply rules
      const newCellAges = new Map();
      
      for (const key of toCheck) {
        const { x, y } = parseCellKey(key);
        const neighbors = getNeighbors(x, y);
        const isAlive = grid.has(key);
        const currentAge = cellAges.get(key) || 0;

        if (isAlive && (neighbors === 2 || neighbors === 3)) {
          newGrid.set(key, true);
          newCellAges.set(key, currentAge + 1); // Age the cell
        } else if (!isAlive && neighbors === 3) {
          newGrid.set(key, true);
          newCellAges.set(key, 0); // New born cell
          births++;
        } else if (isAlive) {
          deaths++;
        }
      }
      
      cellAges = newCellAges;
      
      // Update activity tracking for heatmap
      for (const key of newGrid.keys()) {
        const currentActivity = cellActivity.get(key) || 0;
        cellActivity.set(key, Math.min(currentActivity + 1, 100));
      }
      
      // Track recently dead cells for ghost effect
      for (const key of grid.keys()) {
        if (!newGrid.has(key)) {
          deadCells.set(key, 0); // Just died
        }
      }
      
      // Age dead cells and remove old ones
      const newDeadCells = new Map();
      for (const [key, deadAge] of deadCells.entries()) {
        if (deadAge < 10) {
          newDeadCells.set(key, deadAge + 1);
        }
      }
      deadCells = newDeadCells;
      
      // Decay activity for cells that aren't alive
      for (const [key, activity] of cellActivity.entries()) {
        if (!newGrid.has(key)) {
          if (activity > 0) {
            cellActivity.set(key, Math.max(0, activity - 2));
          } else {
            cellActivity.delete(key);
          }
        }
      }

      grid = newGrid;
      generation++;
      animationTime++;

      const currentPopulation = grid.size;

      birthsThisGen = births;
      deathsThisGen = deaths;
      totalBirths += births;
      totalDeaths += deaths;

      peakPopulation = Math.max(peakPopulation, currentPopulation);

      // Check stability (same population for 3+ generations)
      if (currentPopulation === previousPopulation) {
        stabilityCounter++;
      } else {
        stabilityCounter = 0;
      }
      previousPopulation = currentPopulation;

      updateStats();
      draw();
    }

    function draw() {
      ctx.fillStyle = ruleColors[currentRule]?.bgColor || '#000';
      ctx.fillRect(0, 0, canvas.width, canvas.height);

      const startCol = Math.floor(-offsetX / cellSize) - 1;
      const endCol = Math.ceil((canvas.width - offsetX) / cellSize) + 1;
      const startRow = Math.floor(-offsetY / cellSize) - 1;
      const endRow = Math.ceil((canvas.height - offsetY) / cellSize) + 1;

      // Draw grid (if enabled)
      if (showGrid) {
        // ctx.strokeStyle = '#fff';
        ctx.strokeStyle = ruleColors[currentRule]?.gridColor || '#333';
        ctx.lineWidth = 1;

        for (let i = startCol; i <= endCol; i++) {
          const x = i * cellSize + offsetX;
          ctx.beginPath();
          ctx.moveTo(x, 0);
          ctx.lineTo(x, canvas.height);
          ctx.stroke();
        }

        for (let i = startRow; i <= endRow; i++) {
          const y = i * cellSize + offsetY;
          ctx.beginPath();
          ctx.moveTo(0, y);
          ctx.lineTo(canvas.width, y);
          ctx.stroke();
        }
      }

      // Render ghost trails first (for ghost rule)
      if (currentRule === 'ghost') {
        for (const [key, deadAge] of deadCells.entries()) {
          const { x, y } = parseCellKey(key);
          const screenX = x * cellSize + offsetX;
          const screenY = y * cellSize + offsetY;
          
          if (screenX + cellSize > 0 && screenX < canvas.width &&
            screenY + cellSize > 0 && screenY < canvas.height) {
            const ghostProps = getGhostProperties(false, 0, deadAge);
            
            if (ghostProps.alpha > 0) {
              ctx.globalAlpha = ghostProps.alpha;
              ctx.fillStyle = ghostProps.color;
              
              const actualSize = cellSize * (ghostProps.sizeMultiplier || 1);
              const offset = (cellSize - actualSize) / 2;
              
              if (showGrid) {
                ctx.fillRect(screenX + 1 + offset, screenY + 1 + offset, actualSize - 2, actualSize - 2);
              } else {
                ctx.fillRect(screenX + offset, screenY + offset, actualSize, actualSize);
              }
              
              ctx.globalAlpha = 1;
            }
          }
        }
      }
      
      // Draw living cells
      for (const key of grid.keys()) {
        const { x, y } = parseCellKey(key);
        const screenX = x * cellSize + offsetX;
        const screenY = y * cellSize + offsetY;

        if (screenX + cellSize > 0 && screenX < canvas.width &&
          screenY + cellSize > 0 && screenY < canvas.height) {
          
          let color = '#0f0';
          let sizeMultiplier = 1;
          let alpha = 1;
          let glow = false;
          let glowColor = null;
          
          // Calculate initial cell size and position (may be recalculated for some rules)
          let actualSize = cellSize * sizeMultiplier;
          let offset = (cellSize - actualSize) / 2;
          let cellX = screenX + offset;
          let cellY = screenY + offset;
          let cellWidth = showGrid ? actualSize - 2 : actualSize;
          let cellHeight = showGrid ? actualSize - 2 : actualSize;
          let finalX = showGrid ? cellX + 1 : cellX;
          let finalY = showGrid ? cellY + 1 : cellY;
          
          // Apply current rule
          switch (currentRule) {
            case 'neighborColor':
              const neighborCount = getNeighbors(x, y);
              color = getColorByNeighborCount(neighborCount);
              break;
              
            case 'ageBased':
              const age = cellAges.get(key) || 0;
              const ageProps = getAgeBasedProperties(age);
              color = ageProps.color;
              sizeMultiplier = ageProps.sizeMultiplier;
              // Recalculate size and position
              actualSize = cellSize * sizeMultiplier;
              offset = (cellSize - actualSize) / 2;
              cellX = screenX + offset;
              cellY = screenY + offset;
              cellWidth = showGrid ? actualSize - 2 : actualSize;
              cellHeight = showGrid ? actualSize - 2 : actualSize;
              finalX = showGrid ? cellX + 1 : cellX;
              finalY = showGrid ? cellY + 1 : cellY;
              break;
              
            case 'density':
              const density = calculateLocalDensity(x, y);
              const densityProps = getDensityBasedProperties(density);
              color = densityProps.color;
              alpha = densityProps.alpha;
              break;
              
            case 'heatmap':
              const activity = cellActivity.get(key) || 0;
              const heatProps = getHeatmapProperties(activity);
              color = heatProps.color;
              alpha = heatProps.alpha;
              break;
              
            case 'ghost':
              const ghostAge = cellAges.get(key) || 0;
              const ghostProps = getGhostProperties(true, ghostAge, 0);
              color = ghostProps.color;
              alpha = ghostProps.alpha;
              break;
              

              


              
            case 'classic':
            default:
              color = ruleColors[currentRule]?.cellColor || '#0f0';
              break;
          }
          
          // Size and position already calculated above
          
          // Apply glow effect
          if (glow && cellSize > 5) {
            ctx.shadowColor = glowColor || color;
            ctx.shadowBlur = Math.min(cellSize / 3, 10);
          }
          
          // Set alpha and draw
          if (alpha < 1) {
            ctx.globalAlpha = alpha;
          }
          
          ctx.fillStyle = color;
          ctx.fillRect(finalX, finalY, cellWidth, cellHeight);
          
          // Reset effects
          if (glow) {
            ctx.shadowBlur = 0;
          }
          if (alpha < 1) {
            ctx.globalAlpha = 1;
          }
        }
      }
    }

    function updateStats() {
      const currentPop = grid.size;
      const popChange = generation > 0 ? currentPop - previousPopulation : 0;
      const changeSymbol = popChange > 0 ? '+' : '';

      let stabilityText = '-';
      if (stabilityCounter >= 3) {
        stabilityText = 'STABLE';
      } else if (stabilityCounter > 0) {
        stabilityText = `${stabilityCounter}/3`;
      } else if (generation > 0) {
        stabilityText = 'CHANGING';
      }

      document.getElementById('generation').textContent = generation;
      document.getElementById('initialCells').textContent = initialCellCount;
      document.getElementById('liveCells').textContent = currentPop;
      document.getElementById('popChange').textContent = generation > 0 ? `${changeSymbol}${popChange}` : '0';
      document.getElementById('peakPop').textContent = peakPopulation;
      document.getElementById('births').textContent = birthsThisGen;
      document.getElementById('deaths').textContent = deathsThisGen;
      document.getElementById('totalBirths').textContent = totalBirths;
      document.getElementById('totalDeaths').textContent = totalDeaths;
      document.getElementById('stability').textContent = stabilityText;
    }

    function start() {
      if (!running) {
        running = true;
        lastTime = performance.now();
        requestAnimationFrame(gameLoop);
      }
    }

    function stop() {
      running = false;
    }

    function clear() {
      grid.clear();
      cellAges.clear();
      populationDensityMap.clear();
      cellActivity.clear();
      deadCells.clear();
      particleTrails.clear();
      wavePhases.clear();
      cellDirections.clear();
      animationTime = 0;
      generation = 0;
      initialCellCount = 0;
      peakPopulation = 0;
      totalBirths = 0;
      totalDeaths = 0;
      birthsThisGen = 0;
      deathsThisGen = 0;
      previousPopulation = 0;
      stabilityCounter = 0;
      updateStats();
      draw();
    }

    function randomSeed() {
      clear();
      const cols = Math.floor(canvas.width / cellSize);
      const rows = Math.floor(canvas.height / cellSize);
      const centerX = Math.floor(-offsetX / cellSize);
      const centerY = Math.floor(-offsetY / cellSize);

      for (let i = 0; i < (cols * rows) / 8; i++) {
        const x = centerX + Math.floor(Math.random() * cols) - cols / 2;
        const y = centerY + Math.floor(Math.random() * rows) - rows / 2;
        const key = getCellKey(x, y);
        grid.set(key, true);
        cellAges.set(key, 0);
      }

      initialCellCount = grid.size;
      updateStats();
      draw();
    }

    function gameLoop(currentTime) {
      if (!running) return;

      const deltaTime = currentTime - lastTime;
      const interval = 1000 / speed;

      if (deltaTime >= interval) {
        nextGeneration();
        lastTime = currentTime - (deltaTime % interval);
      } else {
        // Update animations even when not advancing generations
        if ([].includes(currentRule)) {
          animationTime += 0.5;
          draw();
        }
      }

      requestAnimationFrame(gameLoop);
    }

    // Event listeners
    canvas.addEventListener('click', (e) => {
      if (isDragging) return;
      const rect = canvas.getBoundingClientRect();
      const x = Math.floor((e.clientX - rect.left - offsetX) / cellSize);
      const y = Math.floor((e.clientY - rect.top - offsetY) / cellSize);
      toggleCell(x, y);
    });

    canvas.addEventListener('mousedown', (e) => {
      isDragging = true;
      dragStartX = e.clientX;
      dragStartY = e.clientY;
      dragOffsetX = offsetX;
      dragOffsetY = offsetY;
      wrapper.classList.add('grabbing');
    });

    canvas.addEventListener('mousemove', (e) => {
      if (isDragging) {
        offsetX = dragOffsetX + (e.clientX - dragStartX);
        offsetY = dragOffsetY + (e.clientY - dragStartY);
        draw();
      }
    });

    canvas.addEventListener('mouseup', () => {
      isDragging = false;
      wrapper.classList.remove('grabbing');
    });

    canvas.addEventListener('mouseleave', () => {
      isDragging = false;
      wrapper.classList.remove('grabbing');
    });

    canvas.addEventListener('wheel', (e) => {
      e.preventDefault();
      const rect = canvas.getBoundingClientRect();
      const mouseX = e.clientX - rect.left;
      const mouseY = e.clientY - rect.top;

      const worldX = (mouseX - offsetX) / cellSize;
      const worldY = (mouseY - offsetY) / cellSize;

      const zoom = e.deltaY < 0 ? 1.1 : 0.9;
      const newCellSize = Math.max(1, Math.min(100, cellSize * zoom));

      if (newCellSize !== cellSize) {
        offsetX = mouseX - worldX * newCellSize;
        offsetY = mouseY - worldY * newCellSize;
        cellSize = newCellSize;
        draw();
      }
    });

    document.getElementById('startBtn').addEventListener('click', start);
    document.getElementById('stopBtn').addEventListener('click', stop);
    document.getElementById('clearBtn').addEventListener('click', clear);
    document.getElementById('randomBtn').addEventListener('click', randomSeed);
    document.getElementById('controls-toggler').addEventListener('click', () => {
      const controls = document.getElementById('controls');
      controls.classList.toggle('hidden');
      const toggler = document.getElementById('controls-toggler');
      toggler.textContent = controls.classList.contains('hidden') ? '+' : 'x';
      
      // Resize canvas after sidebar animation completes
      resize();
      // setTimeout(() => {
      // }, 300); // Match the CSS transition duration
    });
    document.getElementById('fullscreenBtn').addEventListener('click', () => {
      if (!document.fullscreenElement) {
        document.documentElement.requestFullscreen();
      } else {
        document.exitFullscreen();
      }
    });

    document.getElementById('gridToggle').addEventListener('change', (e) => {
      showGrid = e.target.checked;
      draw();
    });

    // Rule change handling
    const ruleDescriptions = {
      neighborColor: {
        title: 'Neighbor Color Coding',
        description: 'Cells change color based on their neighbor count. Red indicates isolation or overcrowding, green shows stable conditions, and yellow/orange represent moderate crowding.'
      },
      ageBased: {
        title: 'Cell Age & Size',
        description: 'Cells grow larger and change color as they age. Young cells are small and bright green, older cells become larger and shift towards red. Maximum tracked age is 20 generations.'
      },
      density: {
        title: 'Population Density',
        description: 'Cells are colored based on local population density in a 5x5 area. Blue for sparse areas, green for normal, yellow for crowded, orange for dense, and red for overcrowded regions.'
      },
      classic: {
        title: 'Classic Green',
        description: 'Traditional Conway\'s Game of Life appearance with all living cells displayed in bright green. Simple and classic visualization.'
      },
      heatmap: {
        title: 'Activity Heatmap',
        description: 'Shows cell activity levels over time. Blue indicates low activity, transitioning through green, yellow, to red for highly active areas. Activity accumulates and slowly decays.'
      },
      ghost: {
        title: 'Ghost Trail',
        description: 'Living cells appear in cyan, while recently dead cells leave fading ghost trails. Provides visual history of cellular death and creates ethereal trailing effects.'
      }
    };

    function createColorControls(rule) {
      const container = document.getElementById('colorControlsContainer');
      container.innerHTML = ''; // Clear existing controls
      
      const colors = ruleColors[rule];
      if (!colors) return;
      
      const colorLabels = {
        classic: {
          cellColor: 'Cell Color',
          gridColor: 'Grid Color',
          bgColor: 'Background Color'
        },
        neighborColor: {
          neighbor0: '0 Neighbors (Dying)',
          neighbor1: '1 Neighbor',
          neighbor2: '2 Neighbors (Stable)',
          neighbor3: '3 Neighbors (Birth)',
          neighbor4: '4 Neighbors',
          neighbor5: '5 Neighbors',
          neighbor6: '6 Neighbors',
          neighbor7: '7 Neighbors',
          neighbor8: '8 Neighbors (Overcrowded)',
          gridColor: 'Grid Color',
          bgColor: 'Background Color'
        },
        ageBased: {
          youngColor: 'Young Cells',
          oldColor: 'Old Cells',
          gridColor: 'Grid Color',
          bgColor: 'Background Color'
        },
        density: {
          sparseColor: 'Sparse Areas',
          normalColor: 'Normal Density',
          crowdedColor: 'Crowded Areas',
          denseColor: 'Dense Areas',
          overcrowdedColor: 'Overcrowded',
          gridColor: 'Grid Color',
          bgColor: 'Background Color'
        },
        heatmap: {
          coldColor: 'Low Activity',
          warmColor: 'Medium Activity',
          hotColor: 'High Activity',
          gridColor: 'Grid Color',
          bgColor: 'Background Color'
        },
        ghost: {
          aliveColor: 'Living Cells',
          deadColor: 'Ghost Trails',
          gridColor: 'Grid Color',
          bgColor: 'Background Color'
        }
      };
      
      const labels = colorLabels[rule] || {};
      
      // Group colors by category
      const cellColors = Object.keys(colors).filter(key => !['gridColor', 'bgColor'].includes(key));
      const environmentColors = ['gridColor', 'bgColor'].filter(key => colors[key] !== undefined);
      
      // Create cell colors section
      if (cellColors.length > 0) {
        const cellSection = document.createElement('div');
        cellSection.className = 'color-section';
        cellSection.innerHTML = '<h4>Cell Colors</h4>';
        
        cellColors.forEach(colorKey => {
          const control = document.createElement('div');
          control.className = 'color-control';
          control.innerHTML = `
            <label for="${rule}_${colorKey}">${labels[colorKey] || colorKey}:</label>
            <input type="color" id="${rule}_${colorKey}" value="${colors[colorKey]}">
          `;
          cellSection.appendChild(control);
        });
        
        container.appendChild(cellSection);
      }
      
      // Create environment colors section
      if (environmentColors.length > 0) {
        const envSection = document.createElement('div');
        envSection.className = 'color-section';
        envSection.innerHTML = '<h4>Environment</h4>';
        
        environmentColors.forEach(colorKey => {
          const control = document.createElement('div');
          control.className = 'color-control';
          control.innerHTML = `
            <label for="${rule}_${colorKey}">${labels[colorKey] || colorKey}:</label>
            <input type="color" id="${rule}_${colorKey}" value="${colors[colorKey]}">
          `;
          envSection.appendChild(control);
        });
        
        container.appendChild(envSection);
      }
      
      // Add event listeners for all color inputs
      Object.keys(colors).forEach(colorKey => {
        const input = document.getElementById(`${rule}_${colorKey}`);
        if (input) {
          input.addEventListener('input', (e) => {
            ruleColors[rule][colorKey] = e.target.value;
            if (currentRule === rule) {
              draw();
            }
          });
        }
      });
    }

    function updateRuleDescription(rule) {
      const desc = ruleDescriptions[rule];
      const descElement = document.getElementById('ruleDescription');
      descElement.innerHTML = `<h4>${desc.title}</h4><p>${desc.description}</p>`;
      
      // Always show color customization
      const colorCustomization = document.getElementById('colorCustomization');
      colorCustomization.style.display = 'block';
      
      // Create color controls for the current rule
      createColorControls(rule);
      
      // Update selected label styling
      document.querySelectorAll('.rule-option label').forEach(label => {
        label.classList.remove('selected');
      });
      
      // Find the label containing the selected radio button
      const selectedRadio = document.getElementById(`${rule}Rule`);
      if (selectedRadio) {
        const selectedLabel = selectedRadio.closest('label');
        if (selectedLabel) {
          selectedLabel.classList.add('selected');
        }
      }
    }

    document.querySelectorAll('input[name="rule"]').forEach(radio => {
      radio.addEventListener('change', (e) => {
        if (e.target.checked) {
          currentRule = e.target.value;
          updateRuleDescription(currentRule);
          draw();
        }
      });
    });

    document.getElementById('speedInput').addEventListener('input', (e) => {
      speed = Math.max(1, Math.min(60, parseInt(e.target.value) || 10));
      e.target.value = speed;
    });

    // Color picker event listeners are now handled in createColorControls function

    document.addEventListener('keydown', (e) => {
      if (e.code === 'Space') {
        e.preventDefault();
        running ? stop() : start();
      }
    });

    window.addEventListener('resize', resize);

    // === PATTERN DATA ===
    
    const patternsContainer = document.getElementById("patternsContainer");

    patterns.forEach((pattern) => {
      const btn = document.createElement("button");
      btn.textContent = pattern.name;
      btn.addEventListener("click", () => {
        // Get the visible center of the canvas in world coordinates
        const centerX = Math.floor((canvas.width / 2 - offsetX) / cellSize);
        const centerY = Math.floor((canvas.height / 2 - offsetY) / cellSize);

        placePattern(pattern.cells, centerX, centerY);
      });

      patternsContainer.appendChild(btn);
    });

    // === FUNCTION TO PLACE A PATTERN ===
    function placePattern(cells, originX = 0, originY = 0) {
      for (const [dx, dy] of cells) {
        const x = originX + dx;
        const y = originY + dy;
        const key = getCellKey(x, y);
        grid.set(key, true);
        cellAges.set(key, 0);
      }
      initialCellCount = grid.size;
      updateStats();
      draw();
    }


    // Initialize
    resize();
    updateStats();
    updateRuleDescription(currentRule);
  </script>
</body>

</html>
