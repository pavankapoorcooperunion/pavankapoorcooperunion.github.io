
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="color-scheme" content="light dark">


<style>
/* Compact centered layout */
body { max-width: 720px; margin: 24px auto 72px; padding: 0 16px; font: 16px/1.65 -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif; color:#0f172a; }
h1,h2{border-bottom:1px solid #e5e7eb;padding-bottom:.3em}
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
  h1,h2 { border-bottom-color:#1f2937; }
  hr { background:#1f2937; height:1px; border:0; }

  /* code */
  pre { background:#0f172a; border:1px solid #1f2937; }
  :not(pre)>code { color:#e5e7eb; background:#0f172a; border:1px solid #1f2937; }

  /* tables / gallery text */
  table td, table th { color:#e5e7eb; }

  /* blockquote */
  blockquote { color:#e5e7eb; background:#111827; border-left-color:#60a5fa66; }
}


</style>


# Pavan Kapoor: Mechanical Engineering Portfolio

- [Pavan Kapoor: Mechanical Engineering Portfolio](#pavan-kapoor-mechanical-engineering-portfolio)
- [Cooper Union Motorsports: Formula SAE](#cooper-union-motorsports-formula-sae)
  - [Nosecone](#nosecone)
    - [Mold Manufacturing](#mold-manufacturing)
    - [Infusion Layup Setup](#infusion-layup-setup)
    - [Resin Infusion](#resin-infusion)
    - [Post-Processing](#post-processing)
    - [Post-Vinyl](#post-vinyl)
  - [Firewall: Electrically and Thermally Insulative, Ballistically Protective](#firewall-electrically-and-thermally-insulative-ballistically-protective)
    - [Materials](#materials)
    - [Design](#design)
    - [Lower Firewall Manufacturing](#lower-firewall-manufacturing)
    - [Upper Firewall Manufacturing](#upper-firewall-manufacturing)
  - [Anti-Intrusion Plate and Impact Attenuator](#anti-intrusion-plate-and-impact-attenuator)
    - [AIP Welding](#aip-welding)
    - [Impact Attenuator Adhesion](#impact-attenuator-adhesion)
  - [Harness Tabs](#harness-tabs)
  - [Drivetrain \& Accumulator Mounting](#drivetrain--accumulator-mounting)
- [Class Projects](#class-projects)
  - [3 Month Sumo Robot Project](#3-month-sumo-robot-project)
    - [CAD](#cad-1)
    - [Test prints](#test-prints)
    - [3D Printed Chassis](#3d-printed-chassis)
    - [Custom Silicone wheels](#custom-silicone-wheels)
    - [Final Robot](#final-robot)
- [CNC Machining Projects](#cnc-machining-projects)
  - [Name Plate Engraving](#name-plate-engraving)
  - [Weight-Efficient Coaster](#weight-efficient-coaster)
- [Contact](#contact)

# Cooper Union Motorsports: Formula SAE

![Car](Images/car.png)

#### Body/Cockpit/Safety System Assembly that I Desgined(Excluding frame)

![Assembly](Images/ASSEM.png)

## Nosecone

### Mold Manufacturing

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Nosecone/NC1.JPG" alt="NC1" width="400"/></td>
    <td style="border: none;"><img src="Nosecone/NC2.JPG" alt="NC2" width="400"/></td>
  </tr>
  <tr>
    <td style="border: none;"><img src="Nosecone/NC3.JPG" alt="NC3" width="400"/></td>
    <td style="border: none;"><img src="Nosecone/NC4.JPG" alt="NC4" width="400"/></td>
  </tr>
</table>

### Infusion Layup Setup

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Nosecone/NC5.JPG" alt="NC5" width="400"/></td>
    <td style="border: none;"><img src="Nosecone/NC6.JPG" alt="NC6" width="400"/></td>
  </tr>
</table>

### Resin Infusion

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Nosecone/NC7.JPG" alt="NC7" width="400"/></td>
    <td style="border: none;"><img src="Nosecone/NC8.JPG" alt="NC8" width="400"/></td>
  </tr>
</table>

### Post-Processing

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Nosecone/NC9.JPG" alt="NC9" width="400"/></td>
    <td style="border: none;"><img src="Nosecone/NC10.JPG" alt="NC10" width="400"/></td>
  </tr>
</table>

![NC11](Nosecone/NC11.JPG)

### Post-Vinyl

![NC12](Nosecone/NC12.JPG)

## Firewall: Electrically and Thermally Insulative, Ballistically Protective

### Materials

The Firewall is made of a sandwich panel of 6 layers of 200 gsm bidirectional basalt fiber with a sheet of Nomex Honeycomb in the middle. It also has a layer of 0.64mm thick 6061 Aluminum facing the tractive system. I used Basalt because it had the highest resistivity and acceptable tensile strength. The Nomex Honeycomb adds an air gap which improves the area moment of interia and the thermal resistivity of the panel leading to greater stiffness and themral insulation without adding more layers of basalt.

### Design

#### CAD

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Firewall/FW1.png" alt="FW1" width="400"/></td>
    <td style="border: none;"><img src="Firewall/FW2.png" alt="FW2" width="400"/></td>
  </tr>
</table>

![FW3](Firewall/FW3.png)

#### Lasercut Plywood prototype

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Firewall/FWP1.JPG" alt="FWP1" width="400"/></td>
    <td style="border: none;"><img src="Firewall/FWP2.JPG" alt="FWP2" width="400"/></td>
  </tr>
  <tr>
    <td colspan="2" style="border: none; text-align: center;"><img src="Firewall/FWP3.JPG" alt="FWP1" width="400"/></td>
  </tr>
</table>

### Lower Firewall Manufacturing

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Firewall/FW4.JPG" alt="FW4" width="400"/></td>
    <td style="border: none;"><img src="Firewall/FW5.jpeg" alt="FW5" width="400"/></td>
  </tr>
  <tr>
    <td style="border: none;"><img src="Firewall/FW6.jpeg" alt="FW6" width="400"/></td>
    <td style="border: none;"><img src="Firewall/FW7.JPG" alt="FW7" width="400"/></td>
  </tr>
</table>

#### Post Processed

![Firewall](Firewall/FW8.JPG)

### Upper Firewall Manufacturing

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Firewall/UFW_1.JPG" alt="UFW1" width="400"/></td>
    <td style="border: none;"><img src="Firewall/UFW_2.JPG" alt="UFW2" width="400"/></td>
  </tr>
  <tr>
    <td style="border: none;"><img src="Firewall/UFW_3.JPG" alt="UFW3" width="400"/></td>
    <td style="border: none;"><img src="Firewall/UFW4.JPG" alt="UFW4" width="400"/></td>
  </tr>
</table>

#### Post Processed

![UF4](Firewall/UFW5.JPG)

---

## Anti-Intrusion Plate and Impact Attenuator

### AIP Welding

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="IA_AIP/IA1.JPG" alt="FWP1" width="400"/></td>
    <td style="border: none;"><img src="IA_AIP/IA2.JPG" alt="FWP2" width="400"/></td>
  </tr>
</table>

### Impact Attenuator Adhesion

![AIP](IA_AIP/AIP.JPG)

---

## Harness Tabs

Harness tab was designed to be able withstand 15,000N of tearout load per tab based on rules from FSAE.

The tabs were designed to be manufactured from rectangular steel tubing so that the bolts were in double shear while being easy and efficient to manufacture since there it was milled out of correctly sized tube rather than a solid block of steel. Although 2 tabs cut from 1/8" sheet metal could have been used, it would have been very challenging to weld the inside edge of the tab as required by rules. The hardware is M12 high-strength alloy steel shouldered bolts.

The factor of safety for the harness tab is 2.1.

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Harness/harness1.jpg" alt="HR1" width="400"/></td>
    <td style="border: none;"><img src="Harness/harness4.png" alt="HR4" width="400"/></td>
  </tr>
  <tr>
    <td colspan="2" style="border: none; text-align: center;"><img src="Harness/harness2.png" alt="HR2" width="400"/></td>
  </tr>
</table>

## Drivetrain & Accumulator Mounting

#### Drivetrain Mounting Fixture

![Fixture](Drivetrain_Accum_Weld/fixture.JPG)

#### Drivetrain Tabs Tack Welded

![Tacked](Drivetrain_Accum_Weld/tack.JPG)

#### My Friend and I welding the Accumalator Tabs under intense time pressure

![Accum/weld](Drivetrain_Accum_Weld/accumweld.JPG)

# Class Projects

## 3 Month Sumo Robot Project

### CAD

![CAD1](SUMo/CAD1.png)
![CAD2](SUMo/CAD2.png)

### Test prints

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="SUMo/test1.JPG" alt="wheel1" width="400"/></td>
    <td style="border: none;"><img src="SUMo/test2.JPG" alt="wheel2" width="400"/></td>
  </tr>
</table>

### 3D Printed Chassis

![print](SUMo/Printvid.gif)

### Custom Silicone wheels

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="SUMo/Wheel1.JPG" alt="wheel1" width="400"/></td>
    <td style="border: none;"><img src="SUMo/Wheel2.JPG" alt="wheel2" width="400"/></td>
  </tr>
  <tr>
    <td style="border: none;"><img src="SUMo/Wheel3.JPG" alt="wheel3" width="400"/></td>
    <td style="border: none;"><img src="SUMo/Wheel4.JPG" alt="wheel4" width="400"/></td>
  </tr>
</table>

![final_wheel](SUMo/Wheel5.JPG)

### Final Robot

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="SUMo/top2.jpeg" alt="FWP1" width="400"/></td>
    <td style="border: none;"><img src="SUMo/back.jpeg" alt="FWP2" width="400"/></td>
  </tr>
 <tr>
 <tr>
    <td colspan="2" style="border: none; text-align: center;"><img src="SUMo/Iso.jpeg" alt="FWP1" width="400"/></td>
  </tr>
  </tr>
</table>

![final_right](SUMo/Match2.gif)

# CNC Machining Projects

## Name Plate Engraving

![NP1](CNC/NP1.JPG)
![NP2](CNC/NP2.JPG)
![NP3](CNC/NP3.JPG)

## Weight-Efficient Coaster

![AlU_C1](CNC/ALU_C1.JPG)
![AlU_CVid](CNC/CNC_VID.gif)
![AlU_C2](CNC/ALU_C2.JPG)
![AlU_C3](CNC/ALU_C3.JPG)

---

# Contact

- [pavantarunkapoor@gmail.com](mailto:your.email@example.com)
