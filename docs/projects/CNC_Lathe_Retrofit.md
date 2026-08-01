
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="color-scheme" content="light dark">

<script>
  document.title = "Pavan Kapoor — CNC Lathe Retrofit";
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
<p class="back-link"><a href="/">&larr; Back to Projects</a></p>


# CNC Lathe Retrofit
### Design and Fabrication Project

ME 311: Mechanical Design, The Cooper Union — team project with Maria Alvarado, Liki Hamakiotes, Santiago Helbig, Spencer Kirsch, and Asmi Shirsat, advised by Professor Estuardo Rodas.

A second-operation Hardinge lathe was sitting idle in the student machine shop, so our team retrofitted it into a functional 2-axis CNC lathe: a motorized X-Z gantry in place of the manual carriage, a custom control system, and (by my teammates) an 8-station automatic tool changer. Retrofitting kept the machine's existing mechanical precision and let us build a CNC that students could run independently, at a fraction of the cost of a new machine. I designed the X-Z carriage and drove the general architecture decisions for the automation system.

![Lathe mid-retrofit, on the bench](../Lathe/nice_pic.JPG)

### Starting Point

![Manual Hardinge lathe before retrofit](../Lathe/Lathe_init.JPG)

The donor machine: a manual Hardinge toolroom lathe with hand-crank cross-slide and carriage controls and no electronic motion control.

### X-Z Carriage & System Architecture

I designed the motorized X-Z carriage — the linear rail and ball-screw stages, stepper motor mounts, and tool post interface — and drove the core architecture decisions for the retrofit: how the new carriage would mount to and reuse the existing lathe bed and headstock, motor and driver sizing, and the layout of the control electronics housed in the original cabinet.

This machine started life as a second-operation lathe, so unlike a toolroom lathe there was no existing leadscrew or carriage travel along Z to repurpose — no real Z axis existed at all. That motion had to be designed from scratch and built directly into the original bed casting, rather than just motorizing an axis that was already there.

Motion is fully closed-loop: the X, Z, and turret-index axes run on closed-loop stepper motors and drivers, and the original AC induction spindle motor was replaced with a closed-loop AC servo (17-bit absolute encoder) driving the spindle through a timing belt — giving position feedback on every axis, including the spindle, rather than open-loop step-and-hope motion.

The first CAD pass was kept deliberately simple, just enough to work out how the linear rails and ball screws would mount to the lathe and how the X and Z carriages would interface with each other. After a consultation with the machine shop technician, I reworked the layout around one key change: mounting the linear rails upside down. That let the Z-carriage sit much lower and more compactly, and let the large cross-slide plate double as a chip/debris cover for the rails underneath. I also went from two bearing blocks to four per axis to cut down the moment load on the rails, and thickened the mounting plates to 0.5" steel for stiffness. Final travel came out to 14" in Z and 8" in X.

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="../Lathe/CAD.png" alt="X-Z carriage CAD, no tool changer" width="400"/></td>
    <td style="border: none;"><img src="../Lathe/CAD2.png" alt="X-Z carriage CAD with tool changer installed" width="400"/></td>
  </tr>
</table>

### Modifying the Lathe Bed

The X and Z carriage plates were CNC milled by the shop technician; mounting holes for the motor mounts and rail blocks were drilled and tapped directly into the lathe bed and tailstock area on a manual mill, squaring off the original bed surfaces to accept the new hardware.

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="../Lathe/Lathebed_mod1.JPG" alt="Lathe bed set up for milling" width="400"/></td>
    <td style="border: none;"><img src="../Lathe/Lathebed_mod3.JPG" alt="Drilling and tapping mounting holes in the lathe bed" width="400"/></td>
  </tr>
</table>

### Machined Components

The ball nut housings that couple each axis's ball screw to its carriage plate — machined to hold the ball nut rigidly while leaving clearance for the screw to pass through.

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="../Lathe/ball-nut-x.JPG" alt="X-axis ball nut housing halves" width="400"/></td>
    <td style="border: none;"><img src="../Lathe/ball-nut-x2.JPG" alt="Ball nut housing" width="400"/></td>
  </tr>
</table>

### Assembly

Linear rails were installed and trammed straight and parallel to within 0.001" across their length before anything else went on top — critical for keeping the axes from binding under load.

![Z-axis linear rails installed and trammed](../Lathe/Z-axis-tram.jpeg)

Early stage of final assembly, X-Z interface plate mounted on the carriage before the tool changer went on:

![Partial assembly on the lathe](../Lathe/partial_assembly.JPG)

Fully assembled X-Z gantry with the tool changer installed, mounted on the lathe:

![Full X-Z assembly with tool changer, mounted on the lathe](../Lathe/full_assem2.JPG)

### Tool Changer

The 8-station turret tool changer was designed and built by my teammates, not me — but it's too cool not to show. It indexes between tools using a ratchet-and-pawl mechanism on the back of the turret plate, driven by its own motor housing.

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="../Lathe/Tool_changer.JPG" alt="8-station turret tool changer loaded with tools" width="400"/></td>
    <td style="border: none;"><img src="../Lathe/Better_toolchanger_image_web.JPG" alt="Tool changer mounted on the finished machine" width="400"/></td>
  </tr>
</table>

### First Part Machined

The first part cut on the finished machine:

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;"><img src="../Lathe/First_machined_part.JPG" alt="First part machined on the retrofitted lathe" width="400"/></td>
    <td style="border: none;"><img src="../Lathe/First_machined_part2.JPG" alt="First machined part held up to the spindle" width="400"/></td>
  </tr>
</table>

### Final Build

The finished machine — nicknamed "Spindlerella" — keeps the original Hardinge headstock and spindle while adding fully motorized X and Z axes and the automatic tool changer, shown here on display at Cooper Union's end-of-year show.

![Finished CNC lathe retrofit on display](../Lathe/Lathe_Final_pic2_web.JPG)

