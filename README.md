# 🤖 Best Hand: Bionic Hand Design and Simulation

3D design and simulation of a bionic hand. The mechanical parts are designed and assembled in **SolidWorks**, and the assembly is exported to **MATLAB/Simulink** to simulate the movement of the fingers and joints.

## Objectives

- Design the mechanical parts of a bionic hand in SolidWorks (palm, finger links, servo motor)
- Assemble the parts into a complete hand model
- Export the assembly to MATLAB/Simulink (Simscape Multibody) to build a simulation model
- Study the movement of the joints as a first step toward robotic control of the hand

## Tools

- **SolidWorks:** 3D part design and assembly
- **MATLAB / Simulink (Simscape Multibody):** modeling and motion simulation
- **STEP:** neutral CAD format, so the parts can be opened in other CAD software

## Repository contents

All files are in the [`Best Hand`](./Best%20Hand/) folder.

| File | Description |
|---|---|
| `biyonikEl.SLDASM` | Full assembly of the bionic hand |
| `ElAya.SLDPRT` | Palm |
| `basLinki.SLDPRT`, `linki1_` to `linki4_.SLDPRT` | Finger links |
| `ServoluMotor.SLDPRT` | Servo motor |
| `*.STEP` | STEP exports of the parts |
| `BestHand.slx` | Simulink simulation model |
| `biyonikEl.xml`, `biyonikEl_DataFile2.m` | Data exported from SolidWorks and used by the Simulink model |

## How to run the simulation

1. Open MATLAB and go to the `Best Hand` folder.
2. Run `biyonikEl_DataFile2.m` to load the model data.
3. Open `BestHand.slx` and click **Run**. The 3D view of the hand opens in the Mechanics Explorer.

Requirements: MATLAB with Simulink and Simscape Multibody.

## Next steps

- Add joint control (servo position commands) to the Simulink model
- Compare the simulated movement with a physical prototype
