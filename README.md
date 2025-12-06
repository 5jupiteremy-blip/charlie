# Free‑Body Diagrams – Driver Torso & Seat‑Back

This file models the forces that a Formula 1 driver experiences during a hard brake.  
The two vector diagrams are rendered directly in the markdown, so they will appear on GitHub **and** when you open the file in any browser on your computer.

---

## 1️⃣ Driver’s torso (the part that contacts the seat‑back)

<svg width="340" height="300" viewBox="0 0 340 300"
     xmlns="http://www.w3.org/2000/svg"
     font-family="Arial,Helvetica,sans-serif">
  <!-- Arrow definitions -->
  <defs>
    <marker id="arrowRed"   markerWidth="10" markerHeight="10" refX="0" refY="3"
            orient="auto" markerUnits="strokeWidth">
      <path d="M0,0 L0,6 L9,3 z" fill="#d9534f"/>
    </marker>
    <marker id="arrowGreen" markerWidth="10" markerHeight="10" refX="0" refY="3"
            orient="auto" markerUnits="strokeWidth">
      <path d="M0,0 L0,6 L9,3 z" fill="#5cb85c"/>
    </marker>
    <marker id="arrowOrange" markerWidth="10" markerHeight="10" refX="0" refY="3"
            orient="auto" markerUnits="strokeWidth">
      <path d="M0,0 L0,6 L9,3 z" fill="#f0ad4e"/>
    </marker>
    <marker id="arrowGray"   markerWidth="8" markerHeight="8" refX="0" refY="3"
            orient="auto" markerUnits="strokeWidth">
      <path d="M0,0 L0,6 L7,3 z" fill="#777"/>
    </marker>
  </defs>

  <!-- Driver torso block -->
  <rect x="70" y="40" width="200" height="200"
        fill="#e0f7ff" stroke="#0077aa" stroke-width="2"/>
  <text x="170" y="150" text-anchor="middle" font-size="14" fill="#004466">
    Driver Torso
  </text>

  <!-- Forces -->
  <!-- Forward force from seat‑back (red) -->
  <line x1="270" y1="80" x2="340" y2="80"
        stroke="#d9534f" stroke-width="3" marker-end="url(#arrowRed)"/>
  <text x="305" y="70" fill="#d9534f" font-size="12" text-anchor="middle">
    F<sub>seat‑back</sub>
  </text>

  <!-- Backward force from harness (green) -->
  <line x1="70" y1="150" x2="0" y2="150"
        stroke="#5cb85c" stroke-width="3" marker-end="url(#arrowGreen)"/>
  <text x="35" y="140" fill="#5cb85c" font-size="12" text-anchor="middle">
    F<sub>harness</sub>
  </text>

  <!-- Backward force from HANS (orange) -->
  <line x1="70" y1="190" x2="0" y2="230"
        stroke="#f0ad4e" stroke-width="3" marker-end="url(#arrowOrange)"/>
  <text x="35" y="260" fill="#f0ad4e" font-size="12" text-anchor="middle">
    F<sub>HANS</sub>
  </text>

  <!-- Weight (down) -->
  <line x1="170" y1="240" x2="170" y2="280"
        stroke="#777" stroke-width="2" marker-end="url(#arrowGray)"/>
  <text x="185" y="265" fill="#777" font-size="12">W</text>

  <!-- Normal from seat cushion (up) -->
  <line x1="170" y1="40" x2="170" y2="0"
        stroke="#777" stroke-width="2" marker-end="url(#arrowGray)"/>
  <text x="185" y="20" fill="#777" font-size="12">N</text>
</svg>

---

## 2️⃣ Seat‑back (rigid panel attached to the chassis)

<svg width="340" height="260" viewBox="0 0 340 260"
     xmlns="http://www.w3.org/2000/svg"
     font-family="Arial,Helvetica,sans-serif">
  <!-- Arrow definitions (reuse same IDs) -->
  <defs>
    <marker id="arrowRed"   markerWidth="10" markerHeight="10" refX="0" refY="3"
            orient="auto" markerUnits="strokeWidth">
      <path d="M0,0 L0,6 L9,3 z" fill="#d9534f"/>
    </marker>
    <marker id="arrowGreen" markerWidth="10" markerHeight="10" refX="0" refY="3"
            orient="auto" markerUnits="strokeWidth">
      <path d="M0,0 L0,6 L9,3 z" fill="#5cb85c"/>
    </marker>
    <marker id="arrowBlue"   markerWidth="10" markerHeight="10" refX="0" refY="3"
            orient="auto" markerUnits="strokeWidth">
      <path d="M0,0 L0,6 L9,3 z" fill="#337ab7"/>
    </marker>
  </defs>

  <!-- Seat‑back block -->
  <rect x="70" y="40" width="200" height="180"
        fill="#fff3e0" stroke="#d58512" stroke-width="2"/>
  <text x="170" y="130" text-anchor="middle" font-size="14" fill="#8a4b00">
    Seat‑Back
  </text>

  <!-- Forces on seat‑back -->
  <!-- Backward force from driver (red) -->
  <line x1="70" y1="80" x2="0" y2="80"
        stroke="#d9534f" stroke-width="3" marker-end="url(#arrowRed)"/>
  <text x="35" y="70" fill="#d9534f" font-size="12" text-anchor="middle">
    F<sub>driver</sub>
  </text>

  <!-- Forward pull from chassis (green) -->
  <line x1="270" y1="150" x2="340" y2="150"
        stroke="#5cb85c" stroke-width="3" marker-end="url(#arrowGreen)"/>
  <text x="305" y="140" fill="#5cb85c" font-size="12" text-anchor="middle">
    F<sub>chassis</sub>
  </text>

  <!-- Forward force at mounting points (blue) -->
  <line x1="270" y1="40" x2="340" y2="-20"
        stroke="#337ab7" stroke-width="3" marker-end="url(#arrowBlue)"/>
  <text x="305" y="-30" fill="#337ab7" font-size="12" text-anchor="middle">
    F<sub>mounts</sub>
  </text>
</svg>
