
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="color-scheme" content="light dark">

<script>
  document.title = "Pavan Kapoor — Axial Air Compressor CFD";
</script>



<style>
/* Compact centered layout */
body { max-width: 720px; margin: 24px auto 72px; padding: 0 16px; font: 16px/1.65 -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif; color:#0f172a; }
h1,h2{border-bottom:2px solid #e5e7eb;padding-bottom:.3em}
img { display:block; margin:10px auto; max-width:100% !important; height:auto !important; border-radius:4px; }

/* Table-based gallery that doesn't rely on CSS grid support */
table.gallery { width:100%; border-collapse:collapse; margin:12px 0; }
table.gallery td { padding:6px; border:none; text-align:center; vertical-align:top; }
table.gallery img { width:100% !important; height:auto !important; border-radius:6px; }


/* --- dark mode overrides --- */
@media (prefers-color-scheme: dark) {
  html, body { background:#242424 ; color:#e5e7eb; }
  h1,h2,h3,h4,h5,h6 { color:#f8fafc; }
  a { color:#60a5fa; }
  a:visited { color:#93c5fd; }
  a:hover, a:focus { color:#bfdbfe; }

  figcaption, small, .muted { color:#94a3b8; }
  h1, h2 {
    border-bottom: 2px solid #7a7a7a !important;  /* try #4a4a4a, #585858, or #6b6b6b */
    padding-bottom: .35em !important;
  }
  hr {
    background: #4a4a4a !important;
    height: 2px; border: 0;
  }

  /* code */
  pre { background:#0f172a; border:1px solid #1f2937; }
  :not(pre)>code { color:#e5e7eb; background:#0f172a; border:1px solid #1f2937; }

  /* tables / gallery text */
  table td, table th { color:#e5e7eb; }

  /* blockquote */
  blockquote { color:#e5e7eb; background:#111827; border-left-color:#60a5fa66; }
}

.video-container {
    display: flex;
    flex-direction: column;
    align-items: center;    /* Center horizontally */
    justify-content: center;
    margin: 0 auto;
    max-width: 100%;        /* Keep within page width */
  }

.video-container video {
    width: 100%;            /* Make responsive */
    max-width: 800px;       /* Limit size on large screens */
    height: auto;           /* Maintain aspect ratio */
    border-radius: 8px;     /* Optional: rounded corners */
  }



.back-link { margin: 0 0 22px; }
.back-link a { font-size: 0.9rem; text-decoration: none; }
.back-link a:hover { text-decoration: underline; }
</style>
<p class="back-link"><a href="../index.html">&larr; Back to Projects</a></p>


# Axial Air Compressor CFD
### Axial Air Compressor for Turbofan Engine

![](../CFD_Air/CAD_1.png)

Designed and simulated a multi-stage axial compressor capable of achieving a 20:1 pressure ratio at 40,000 ft.  
Simulations were performed in ANSYS Fluent using detailed stage-by-stage geometry and validated at both altitude and sea-level conditions.

### Design Constraints
- Achieve 20:1 pressure ratio
- Maximum altitude of 40,000 ft
- Outer diameter between 5 ft and 6 ft
- Maximum RPM of any stage < 50,000 rpm


### Design parameters
<div align="center">


| Parameter                  |  Value | Unit |
|---------------------------|------:|:----|
| Rotational speed          |  2500 | rpm |
| Outer Diameter            |  5.96 | ft  |
| Length                    |  23.4 | ft  |
| Maximum blade length      |  25.8 | in  |
| Minimum blade length      |   3.2 | in  |
| Dry Mass                  | 11000 | lbm |
| Blade/Vane shape          | NACA 9506 | - |
| Power at 40k              |  1087 | HP  |
| Compression Ratio 40K     |    22 | —   |
| Power at STP              |  4902 | HP  |
| Compression Ratio STP     |    22 | —   |

</div>

<br><br>

#### Hand Calculations
![alt text](../CFD_Air/Air_comp_hand.png)

Stage-wise hand calculation to determine stage inlet & outlet area and angles of attack for rotors & stators required to meet the design criteria.


#### Parametric CAD model
Built fully Parametric CAD Model in Onshape with ability to rapidly adjust the following design parameters for each stage:

- Stage inlet and outlet area
- Rotor and stator
  - number of blades 
  - chord
  - camber 
  - angle of attack at base and tip


![CAD1](../CFD_Air/CAD_4.png)


<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="../CFD_Air/CAD_1.png" alt="wheel1" width="400"/></td>
    <td style="border: none;"><img src="../CFD_Air/CAD_7.png" alt="wheel2" width="400"/></td>
  </tr>
  <tr>
    <td style="border: none;"><img src="../CFD_Air/CAD_2.png" alt="wheel3" width="400"/></td>
    <td style="border: none;"><img src="../CFD_Air/CAD_6.png" alt="wheel4" width="400"/></td>
  </tr>
</table>


### Simulation

#### Mesh

##### Stage 1 Mesh
![Mesh](../CFD_Air/mesh_aspect.png)
![Mesh](../CFD_Air/mesheq.png)

#### Stage 1 Simulation

<div class="video-container">
  <video src="../CFD_Air/S1_press.mp4" autoplay loop muted playsinline></video>
<br>
  <video src="../CFD_Air/S1_temp.mp4" autoplay loop muted playsinline></video>
<br>
  <video src="../CFD_Air/S1_stream.mp4" autoplay loop muted playsinline></video>
</div>

#### Stage 4 Simulation

<div class="video-container">
  <video src="../CFD_Air/S4_press_anim.mp4" autoplay loop muted playsinline></video>
  <br>
  <video src="../CFD_Air/S4_temp_anim.mp4" autoplay loop muted playsinline></video>
  <br>
  <video src="../CFD_Air/S4_path_anim.mp4" autoplay loop muted playsinline></video>
</div>

### Results
- Achieved total 20 : 1 compression ratio across 17 stages   
- Average stage efficiency of 82%
- Pressure ratio and efficiency validated against hand calculations
- Turbulence modeling, residual analysis, and mesh-independence verification  

  
<div align="center">
<br><br>
  
*Table 1: Performance metrics for maximum operating altitude.*

| 40,000 Feet       | Inlet | Outlet | Unit |
|----------------------|-----:|------:|:-----|
| Pressure     |  2.7 |   103 | psi  |
| Temperature  | -69.7|  1592 | F    |
<br><br>

*Table 2: Performance metrics at sea level.*

| Sea level        | Inlet | Outlet | Unit |
|----------------------|-----:|------:|:-----|
| Pressure     | 14.7 |   223 | psi  |
| Temperature  | 59.0 |  1253 | F    |
</div>
 
<br><br>

More information about this project in the [full report](https://drive.google.com/file/d/1QVX39FOOw6npelVQ_BAIDXQUUlno0JuK/view?usp=drive_link)
<br>
[Original Assignment](https://drive.google.com/file/d/12JTfVGm5Dggs_krdk6svhqtvWRtSXwW-/view?usp=sharing)
