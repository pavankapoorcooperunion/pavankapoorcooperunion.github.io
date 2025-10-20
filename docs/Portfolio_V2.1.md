
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="color-scheme" content="light dark">

<script>
  document.title = "Pavan Kapoor — Portfolio";
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
- [Computational Fluid Dynamics Projects](#computational-fluid-dynamics-projects)
  - [Axial Air Compressor for Turbofan Engine](#axial-air-compressor-for-turbofan-engine)
    - [Design Constraints](#design-constraints)
    - [Design parameters](#design-parameters)
    - [Simulation](#simulation)
    - [Results](#results)
  - [Automotive Heat Exchanger](#automotive-heat-exchanger)
- [Class Projects](#class-projects)
  - [Sumo Robot Project](#sumo-robot-project)
    - [Design](#design-1)
    - [Test prints](#test-prints)
    - [3D Printed Chassis](#3d-printed-chassis)
    - [Overmolded Silicone Wheels](#overmolded-silicone-wheels)
    - [Final Robot](#final-robot)
  - [Cookie Cutter Press](#cookie-cutter-press)
    - [Version 2](#version-2)
    - [Version 1](#version-1)
- [CNC Machining Projects](#cnc-machining-projects)
  - [Name Plate Engraving](#name-plate-engraving)
  - [Isogrid Coaster](#isogrid-coaster)
- [Contact](#contact)

# Cooper Union Motorsports: Formula SAE

![Car](Images/car.png)
#### Body/Cockpit/Safety System assembly that I designed (excluding frame)
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



##  Firewall: Electrically and Thermally Insulative, Ballistically Protective

### Materials

The Firewall is made of a sandwich panel of 6 layers of 200 gsm bidirectional basalt fiber with a sheet of Nomex Honeycomb in the middle. It also has a layer of 0.64mm thick 6061 Aluminum facing the tractive system. I used Basalt because it had the highest resistivity and acceptable tensile strength. The Nomex honeycomb adds an air gap that increases the area moment of inertia and the panel’s thermal resistance, improving stiffness and thermal insulation without adding more basalt layers.



### Design

#### CAD

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Firewall/FW1.png" alt="FW1" width="400"/></td>
    <td style="border: none;"><img src="Firewall/FW2.png" alt="FW2" width="400"/></td>
  </tr>
</table>

![FW3](Firewall/FW3.png)

#### Laser-cut plywood prototype
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

#### Post-Processed

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

Harness tab was designed to be able to withstand 15,000 N of tear-out load per tab based on rules from FSAE.

The tabs were designed to be manufactured from rectangular steel tubing so that the bolts were in double shear while being easy and efficient to manufacture since it was milled out of correctly sized tube rather than a solid block of steel. Although 2 tabs cut from 1/8" sheet metal could have been used, it would have been very challenging to weld the inside edge of the tab as required by rules. Used M12 high-strength alloy steel shouldered bolts.

The factor of safety for the harness tab is 2.1.

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="Harness/harness1.jpg" alt="HR1" width="400"/></td>
    <td style="border: none;"><img src="Harness/harness4.png" alt="HR4" width="400"/></td>
  </tr>
  <tr>
    <td colspan="2" style="border: none; text-align: center;"><img src="Harness/harness2.png" alt="HR2" width="500"/></td>
  </tr>
</table>

## Drivetrain & Accumulator Mounting

#### Drivetrain Mounting Fixture
![Fixture](Drivetrain_Accum_Weld/fixture.JPG)

#### Drivetrain Tabs Tack Welded
![Tacked](Drivetrain_Accum_Weld/tack.JPG)

#### My friend and I welding the accumulator Tabs under intense time pressure
![Accum/weld](Drivetrain_Accum_Weld/accumweld.JPG)



# Computational Fluid Dynamics Projects



## Axial Air Compressor for Turbofan Engine 
![](CFD_Air/CAD_1.png)

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
![alt text](CFD_Air/Air_comp_hand.png)

Stage-wise hand calculation to determine stage inlet & outlet area and angles of attack for rotors & stators required to meet the design criteria.


#### Parametric CAD model
Built fully Parametric CAD Model in Onshape with ability to rapidly adjust the following design parameters for each stage:

- Stage inlet and outlet area
- Rotor and stator
  - number of blades 
  - chord
  - camber 
  - angle of attack at base and tip


![CAD1](CFD_Air/CAD_4.png)


<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="CFD_Air/CAD_1.png" alt="wheel1" width="400"/></td>
    <td style="border: none;"><img src="CFD_Air/CAD_7.png" alt="wheel2" width="400"/></td>
  </tr>
  <tr>
    <td style="border: none;"><img src="CFD_Air/CAD_2.png" alt="wheel3" width="400"/></td>
    <td style="border: none;"><img src="CFD_Air/CAD_6.png" alt="wheel4" width="400"/></td>
  </tr>
</table>


### Simulation

#### Mesh

##### Stage 1 Mesh
![Mesh](CFD_Air/mesh_aspect.png)
![Mesh](CFD_Air/mesheq.png)

#### Stage 1 Simulation

<div align="center">

<video src="CFD_Air/S1_press.mp4" autoplay loop muted playsinline width="600" ></video>

<video src="CFD_Air/S1_temp.mp4" autoplay loop muted playsinline width="600"  ></video>

<video src="CFD_Air/S1_stream.mp4" autoplay loop muted playsinline width="600" ></video>
</div>

#### Stage 4 Simulation
<div align="center">

<video src="CFD_Air/S4_press_anim.mp4" autoplay loop muted playsinline width="600" ></video>

<video src="CFD_Air/S4_temp_anim.mp4" autoplay loop muted playsinline width="600" ></video>

<video src="CFD_Air/s4_path_anim.mp4" autoplay loop muted playsinline width="600" ></video>
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

## Automotive Heat Exchanger

[Full report](https://drive.google.com/file/d/1VCqYSP_IjIPGORkPQzzPSxOdVdTBt5YO/view?usp=sharing) for reference until the project is added here.
<br>
[Original Assignment](https://drive.google.com/file/d/1451Hp0TVWpOrE3E7IqUipj_E0lH5_nzk/view?usp=sharing)


# Class Projects

## Sumo Robot Project


### Design

#### Design Constraints
- 10"x 10" x 5" size constraint
- Cost under $200
- Total weight under 5lbs
- 3A max stall current for all motors
- 14V maximum battery
- Only using ATMega328P

#### Design Methodology
- The plan was to maximise grip on the drive wheels. The stall current limitation likely meant most motors would similar torque specs, hence weight and grip would drive which robot would resist pushing.
- To maximise grip we optimized two parameters, the normal force and the friction coefficient between the wheels and the ground.
#### Ground Effect Downforce
- The robot was built to weigh close to 5lbs. We add a fan to suck air from underneath the robot to generate downforce. The idea was to increase the normal force on the robot without exceeding the weight limit of 5lbs since the robot was weighed with the fan turned off.
- Due to the power limitation on the fan motor, the fan did not generate a measurable amount of downforce. It was a cool concept to implement regardless of its effectiveness


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




### Overmolded Silicone Wheels

- To optimize the friction coefficient between the wheels and the ground, I made custom 3D printed wheels with silicone cast tires. I used a soft durometer silicone and designed a wheel rim and mold to cast the silicone around the wheel rim.
- Additionally I designed the chassis so that the rear wheels maintained contact with the ground when the front was lifted (like with a wedge during a match). This can be seen in action in the videos below.
- Initially I designed the battery to be housed in the front to make it harder to lift the front and to balance the weight distribution with the two motors in the back. 
- However, in practice the motors had too much torque and the wheels were slipping. Moving the battery to the back significantly increased the grip on the driving wheels. This made the front end easier to lift, but the trade off was worth it since the driving wheels had much more grip and maintained contact with the ground when the front was lifted.
  

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
    <td style="border: none;"><img src="SUMo/Iso.jpeg" alt="FWP2" width="400"/></td>
  </tr>
 <tr>
 <tr>
    <td colspan="2" style="border: none; text-align: center;"><img src="SUMo/back.jpeg" alt="FWP1" width="400"/></td>
  </tr>
  </tr>
</table>


![final_right](SUMo/Match2.gif)
![Match3](SUMo/match_3.gif)

## Cookie Cutter Press

Designed and built cookie cutter press to make a custom shape cookie cutter. My teammate and I decided to make a cookie cutter in the shape of Monza, which is a racetrack. 

### Version 2
![MFG](MFG/MFG_CC_V2.JPG)
![MFG](MFG/MFG_V2_Result.JPG)

<div align="center">

<video src="MFG/MFG_CC_Press_2x.mp4" autoplay loop muted playsinline width="700"  controls></video>
</div>

### Version 1
![MFG](MFG/MFG_CC_V1.JPG)
![MFG](MFG/MFG_CC_V1_result.JPG)

# CNC Machining Projects

## Name Plate Engraving
![NP1](CNC/NP1.JPG)
![NP2](CNC/NP2.JPG)
![NP3](CNC/NP3.JPG)

## Isogrid Coaster
![AlU_C1](CNC/ALU_C1.JPG)
![AlU_CVid](CNC/CNC_VID.gif)
![AlU_C2](CNC/ALU_C2.JPG)
![AlU_C3](CNC/ALU_C3.JPG)



---

# Contact
- [pavantarunkapoor@gmail.com](mailto:pavantarunkapoor@gmail.com)
- [Linkedin: www.linkedin.com/in/pavankap00r](www.linkedin.com/in/pavankap00r)
- [Resume](https://drive.google.com/file/d/1im8G8flU0TsKoPTkrHuLig8cEKztINLW/view?usp=sharing)






