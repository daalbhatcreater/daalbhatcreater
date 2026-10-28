# Rudra Vichpuriya

**Electrical Engineering, B.Tech 2023-27, Netaji Subhas University of Technology, Delhi**

I design and check electrical power systems the way they are built in industry: load schedules, fault levels, switchgear ratings, protection settings and power quality, each worked to the relevant IEC and IEEE standards and verified against hand calculations or a second tool. On the electronics side, I build pipelined processors in Verilog and verify them against reference models.

- Intern, Grid Management Division, **Central Electricity Authority** (Ministry of Power), May-Jul 2026: regional demand-supply balance, grid frequency profiles, inter-regional transfers and congestion.
- Technical visit, **National Load Despatch Centre** (Grid-India), May 2026: real-time dispatch, SCADA telemetry, renewable integration.

---

## Power systems and electrical design

| Project | What it does | Key result |
|---|---|---|
| [**Data centre 2N LV distribution**](https://github.com/daalbhatcreater/datacentre-2n-lv-distribution) | 1 MW data hall with duplicated A/B paths: transformers, generators, UPS, battery, PDUs, switchgear, SLD, and a second-by-second simulation of the utility-to-generator changeover | On generator 14.7 s after a utility failure; the B side carries all 1 MW if a generator fails to start |
| [**Short-circuit & selectivity study**](https://github.com/daalbhatcreater/lv-short-circuit-selectivity-study) | IEC 60909 fault levels for a 2000 kVA system, breaker duty (Icu, Icm, Icw), trip curves with tolerance bands and selectivity limits | 40.5 kA at the main LV bus, within 0.6 % of pandapower |
| [**11/0.415 kV industrial substation**](https://github.com/daalbhatcreater/mv-lv-industrial-substation) | Load list to relay settings: transformer sizing, VCB selection, MV cable fault withstand, IDMT grading checked across the full current range | HV-side faults cleared in 0.09 s, at least 0.3 s grading margin everywhere |
| [**APFC & harmonic filter design**](https://github.com/daalbhatcreater/apfc-harmonic-filter-design) | APFC sizing with a 24-hour relay simulation, harmonic penetration study, detuned steps and 5th/7th tuned filters | pf 0.70 to 0.99 over a day; current TDD 11.2 % to 5.4 % (IEEE 519-2022) |
| [**VFD V/f motor control**](https://github.com/daalbhatcreater/vfd-induction-motor-vf-control) | Dynamic dq model of a 15 kW induction motor, DOL vs V/f starting, switching-level PWM inverter, fan and pump energy analysis | Starting current 6.65x rated on DOL vs 1.09x on the drive; 40 % fan energy saving |
| [**LV cable sizing calculator**](https://github.com/daalbhatcreater/lv-cable-sizing-calculator) | IEC 60364-5-52 sizing with derating, voltage drop, motor starting and fault withstand; reports the governing criterion | Matches all 12 hand-calculated validation cases |

<table>
  <tr>
    <td width="50%"><a href="https://github.com/daalbhatcreater/datacentre-2n-lv-distribution"><img src="https://raw.githubusercontent.com/daalbhatcreater/datacentre-2n-lv-distribution/main/drawings/sld.png" alt="2N data centre single-line diagram"></a><br><sub>2N data centre single-line diagram, generated from the sizing model</sub></td>
    <td width="50%"><a href="https://github.com/daalbhatcreater/mv-lv-industrial-substation"><img src="https://raw.githubusercontent.com/daalbhatcreater/mv-lv-industrial-substation/main/results/protection_tcc.png" alt="11 kV protection coordination curves"></a><br><sub>11 kV relay grading over the LV incomer</sub></td>
  </tr>
  <tr>
    <td width="50%"><a href="https://github.com/daalbhatcreater/apfc-harmonic-filter-design"><img src="https://raw.githubusercontent.com/daalbhatcreater/apfc-harmonic-filter-design/main/results/frequency_scan.png" alt="Harmonic frequency scan"></a><br><sub>Frequency scan: plain capacitors resonate near the 6th harmonic, filters don't</sub></td>
    <td width="50%"><a href="https://github.com/daalbhatcreater/vfd-induction-motor-vf-control"><img src="https://raw.githubusercontent.com/daalbhatcreater/vfd-induction-motor-vf-control/main/results/dol_vs_vf_start.png" alt="DOL versus V/f motor start"></a><br><sub>Direct-on-line versus V/f drive start of a 15 kW fan motor</sub></td>
  </tr>
</table>

## Digital design and computer architecture

| Project | What it does | Key result |
|---|---|---|
| [**RV32I pipelined core**](https://github.com/daalbhatcreater/rv32i-pipelined-core) | 3-stage RISC-V (RV32I) core in synthesizable Verilog with WB-to-EX forwarding, verified instruction by instruction against a Python ISS, built for a Lattice ECP5 FPGA | 201/201 tests pass, 94 844 instructions trace-compared; 41.3 MHz on ECP5 |
| [**16-bit RISC pipeline**](https://github.com/daalbhatcreater/risc16-pipeline) | Custom 16-bit ISA on a classic 5-stage pipeline with forwarding, load-use stall and branch flush | Hazard detection and forwarding units, simulated in Icarus Verilog |

## Skills

**Power systems**: single-line diagrams, load schedules, transformer and DG sizing, LV switchboards (ACB, MCCB, busbars), MV switchgear (VCB), UPS and battery sizing, ATS schemes, short-circuit studies, protection coordination (IDMT, LSI), cable sizing, power factor correction, harmonic analysis and filter design, motor starting and drives

**Standards**: IEC 60909, IEC 60364-4-41/-4-43/-5-52, IEC 60947-2, IEC 60898-1, IEC 61439, IEC 60076-5, IEC 62271-100, IEC 60255-151, IEEE 519-2022, IEEE 18

**Electronics**: Verilog, pipelined CPU design, RISC-V, FPGA flow (Yosys, nextpnr), Icarus Verilog, Verilator, GTKWave, LTspice

**Tools**: Python (NumPy, SciPy, pandas, pandapower, Matplotlib), MATLAB & Simulink, MS Excel, draw.io, MS Project

---

Open to graduate roles in power distribution design, protection and power systems studies, and digital design.
Email: rudra.vichpuriya.ug23@nsut.ac.in
