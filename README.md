# Semesterprojekt i autonome robotter

Automatiseret sorteringssystem der kombinerer en UR5-robotarm med en ATmega644 mikrokontroller og en specialbygget griber. Projektet inkluderer brugergrænseflade i C++, længdemåling via griberens bevægelse og kommunikation via MODBUS og RS232.

---

## Projektoversigt

### Robotprogrammering i C++  
UR5-robotten modtager instruktioner fra GUI’en og udfører afhentning og sortering baseret på objektets længde, estimeret via en timer koblet til griberens lukketid.

### Griberdesign  
Griberen er bygget med en bevægelig finger styret af en gevindstang og motor. Lukning aktiveres via RS232-signal fra ATmega644 og bekræftes gennem strømtrækdetektion.

### Brugergrænseflade (GUI)  
C++ GUI udviklet med wxWidgets muliggør manuel og automatisk styring af robot og griber. Visualisering af fejl og antallet af sorterede klodser er inkluderet.

### Hardware og elektronik  
- Specialdesignet griber printet i PLA  
- ATmega644 styrekreds med RS232 og strømføling  
- PCB med kredsløb til motorstyring og kommunikation

---

## Inkluderede filer

- PRO2_Gruppe5_Rapport.pdf – Fuld rapport med metode, software, hardware og test  
- C++ code/ – GUI og backend til UR5, inkl. `panel.cpp`, `main.cpp`, makefile  
- Assembly code/ – Assemblyprogram til ATmega644 for styring af motor og respons  
- 644Board-Schematic.PDF – Diagram over kredsløb og kommunikationsinterface  
- Gripper_peter_done.iam – 3D CAD-fil (Inventor) af griberen  
- Demo video – [Se demo på YouTube](https://www.youtube.com/watch?v=OvQ3HG4hXTY)

---

## Udførte eksperimenter

- Test af sortering af tre klodsetyper (kort, mellem, lang)  
- Måling af responstid og fejlrate ved forskellige timergrænser  
- Evaluering af GUI-funktionalitet og stabilitet  
- Analyse af ujusterede klodser og konsekvens for systemet

---

## Kompetencer

- Programmering af GUI og robotstyring i C++  
- Udvikling af brugergrænseflade med wxWidgets og MODBUS  
- Assemblyprogrammering til mikrokontroller  
- Design og konstruktion af funktionel griber i 3D  
- Integration af mekanik, elektronik og software  
- Teknisk dokumentation og samarbejde i tværfagligt team

---

## Bidragsydere

- Anas Butt Hussain  
- Robin Hansen  
- Peter Jøker Trachsel  
- Alan Rashid  
- Thomas Vilholm  
- Jakub Hubert Rudowski  
- Patrick Ørsted Povey Andersen

---

## Intention

Dette projekt blev afleveret som en del af faget "Basic Robot Automation" på Syddansk Universitet og deles her med det formål at fremvise færdigheder inden for robotteknologi, elektronik og systemintegration i en professionel kontekst.
