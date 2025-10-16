# Omega Radio

Hello, **PY6FX – Fábio** here.

**Omega Radio** is an HF transceiver for amateur radio bands, designed to use the most accessible components possible—avoiding SMD parts whenever feasible and relying on them only in pre-assembled modules.  

The **receiver** is a tunable super-heterodyne *upconverter* with an IF around **70 MHz**, where an SDR *dongle* is connected. This intermediate frequency has proven ideal for these rather limited devices.  

On **transmission**, two simple and inexpensive **IRFP250** MOSFETs operate in a *push-pull* configuration at the final amplification stage. Since these transistors were not designed for HF, their input impedance is quite irregular, requiring an *inter-stage coupler* between the driver and them. The goal is to achieve about **50 W** on all amateur HF bands.  

The **main control and signal generation** are handled by a **Raspberry Pi Pico**, with a **Si5351** providing both **DDS** and **BFO** functions.  

The name *Omega Radio* refers both to the **survivalist spirit** and to the science-fiction classic *Omega Men*.  

---

## License and Usage

This is an **open-source project**, under **continuous development**, made available **for educational and experimental purposes**.  
Its use, modification, and reproduction are **free**, provided there is **no commercial intent** and **proper credit is given to the original author (PY6FX – Fábio)**.  

The project **comes with no guarantees of performance or safety** and should be used **at the builder’s own risk**.  

---

## Getting Started

You can clone the project with:

```bash
git clone https://github.com/USERNAME/Omega-Radio.git
```

Then open the `.kicad_pro` file in **KiCad 7 or later**:

```
File → Open Project → Omega Radio.kicad_pro
```

All schematic and symbol libraries are included in the repository.  
If KiCad reports missing symbols, ensure that the project’s local library paths are enabled in **Preferences → Manage Symbol Libraries**.

