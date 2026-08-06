# [PBL 2026] Campus Fire Outdoor Evacuation Plan Design

<img src="logo_black.png" width = 60%>

---

## Project Information

### Campus Fire Outdoor Evacuation Plan Design: *Taking Beijing 101 Middle School as an Example*

**Authors:** Lambert Yuxiang Chen 陈禹翔¹, Blake Bo Peng 彭博¹

**Directors:** Sarah Hongjing Shi 史红静¹ @AP Calculus BC, Jessica Jingfei Hou 侯静菲¹ @AP Chemistry, Yutong Zhang 张雨桐¹

&nbsp;&nbsp;&nbsp;&nbsp; ¹ Beijing 101 High School International Department.

**Subjects:** AP Calculus BC, AP Chemistry, Geography, Computer Science and Engineering

## Abstract

Campus fire evacuation plans usually focus on leaving buildings as quickly as possible, while the outdoor movement of toxic combustion products is often treated only qualitatively. This study proposes a GIS-based method for designing safer outdoor evacuation routes during campus fire emergencies by coupling hazardous-gas generation, wind-driven diffusion, and route optimization. Taking Beijing 101 Middle School as the study area, the campus is represented by a metric road-network graph built from processed node and edge CSV data. Model 1 estimates the time-dependent release of representative hazardous gases, including CO, HCN, and HCl, from combustible material mass and gas-generation rates. Model 2 converts these releases into source terms and solves a two-dimensional advection--diffusion equation with wind, attenuation, open boundaries, and a finite-difference grid. Model 3 samples the resulting time-dependent concentration fields along evacuation paths, converts toxic exposure into an FED-based cost, and combines this exposure with route length and the narrowest road width. Assembly-point capacity is also considered, so routes can be replanned when a destination becomes full. A Python simulation program implements the complete workflow, visualizes two-dimensional and three-dimensional gas fields, and displays evacuation routes for all building nodes. The case study shows that the safest route may differ from the geometric shortest route when the plume direction, departure time, road bottlenecks, and destination capacity are considered together. Therefore, the proposed framework provides a practical way to transform campus GIS data and fire-gas diffusion simulation into a quantitative outdoor evacuation plan.

**Keywords:** Campus fire evacuation; Hazardous gas diffusion; Wind-driven advection-diffusion; FED exposure; GIS road network; Route optimization.

## Repository Description

```text
./
|-- Research Proposal_CH&EN.pdf   # Research proposal slides
|-- Midterm - stage 1.pdf         # Midterm 1st report slides
|-- Midterm - stage 2.pdf         # Midterm 2nd report slides
|-- Essay.pdf                     # Final essay content
|-- Essay_Full_length.pdf         # Final essay with full length
|-- Poster.pdf                    # Final poster
|-- Poster.png                    # Final poster
|-- Poster - v2.pdf               # Final poster, 6.26 Version
|-- Poster - ICBS.pdf               # Poster for ICBS High School Exhibition
|-- logo_black.png                # logo of Beijing 101 School
`-- RAEDME.md                     # This markdown document
```

## Simulation Program

This project contain an simulation program, which can be obtain from [cyx728/Campus-Gas-Diffusion-Studio.Simulation-Program-qt](https://github.com/cyx728/Campus-Gas-Diffusion-Studio.Simulation-Program-qt) on GitHub.