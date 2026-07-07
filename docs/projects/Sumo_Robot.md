
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="color-scheme" content="light dark">

<script>
  document.title = "Pavan Kapoor — Sumo Robot Project";
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
<p class="back-link"><a href="../Projects.html">&larr; Back to Projects</a></p>


# Sumo Robot Project


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


![CAD1](../SUMo/CAD1.png)
![CAD2](../SUMo/CAD2.png)

### Test prints

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="../SUMo/test1.JPG" alt="wheel1" width="400"/></td>
    <td style="border: none;"><img src="../SUMo/test2.JPG" alt="wheel2" width="400"/></td>
  </tr>
</table>

### 3D Printed Chassis

![print](../SUMo/Printvid.gif)




### Overmolded Silicone Wheels

- To optimize the friction coefficient between the wheels and the ground, I made custom 3D printed wheels with silicone cast tires. I used a soft durometer silicone and designed a wheel rim and mold to cast the silicone around the wheel rim.
- Additionally I designed the chassis so that the rear wheels maintained contact with the ground when the front was lifted (like with a wedge during a match). This can be seen in action in the videos below.
- Initially I designed the battery to be housed in the front to make it harder to lift the front and to balance the weight distribution with the two motors in the back. 
- However, in practice the motors had too much torque and the wheels were slipping. Moving the battery to the back significantly increased the grip on the driving wheels. This made the front end easier to lift, but the trade off was worth it since the driving wheels had much more grip and maintained contact with the ground when the front was lifted.
  

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="../SUMo/Wheel1.JPG" alt="wheel1" width="400"/></td>
    <td style="border: none;"><img src="../SUMo/Wheel2.JPG" alt="wheel2" width="400"/></td>
  </tr>
  <tr>
    <td style="border: none;"><img src="../SUMo/Wheel3.JPG" alt="wheel3" width="400"/></td>
    <td style="border: none;"><img src="../SUMo/Wheel4.JPG" alt="wheel4" width="400"/></td>
  </tr>
</table>

![final_wheel](../SUMo/Wheel5.JPG)

### Final Robot
<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="../SUMo/top2.jpeg" alt="FWP1" width="400"/></td>
    <td style="border: none;"><img src="../SUMo/Iso.jpeg" alt="FWP2" width="400"/></td>
  </tr>
 <tr>
 <tr>
    <td colspan="2" style="border: none; text-align: center;"><img src="../SUMo/back.jpeg" alt="FWP1" width="400"/></td>
  </tr>
  </tr>
</table>


![final_right](../SUMo/Match2.gif)
![Match3](../SUMo/match_3.gif)
