# Class D Audio Amplifier

This project involves the design and implementation of a 2-layer PCB for a *Class D audio amplifier* using a *half-bridge topology* and integrated *Bluetooth streaming* via the *MHM-28 module*. The amplifier is capable of driving a speaker with high efficiency using Pulse Width Modulation (PWM), with clean audio recovery using an LC filter.

## 🔧 Features

* Class D half-bridge topology for efficient audio amplification
* Bluetooth audio streaming using MHM-28 module
* PWM generation with TLC555 timer
* Signal conditioning and dead-time control using LM393 and 74HC04
* Gate driving with IRS2113 for high-side and low-side MOSFET control
* LC filter output for analog audio reconstruction
* 2-layer PCB designed in KiCad

## 📐 System Architecture

| Module           | Description                                             |
| ---------------- | ------------------------------------------------------- |
| TLC555 Timer     | Triangle waveform generator for PWM modulation          |
| LM393 Comparator | Converts audio to PWM by comparing input with reference |
| IRS2113          | High/low-side MOSFET driver for half-bridge control     |
| IRLZ44N MOSFETs  | Power stage switches                                    |
| LC Filter        | Reconstructs analog signal from PWM output              |
| MHM-28 Module    | Bluetooth V4.0 A2DP module for wireless audio           |
| LM7805 / LM7812  | Linear regulators for 5V and 12V power rails            |

## 📊 Technical Specifications

| Parameter         | Value                      |
| ----------------- | -------------------------- |
| Supply Voltage    | 12V                        |
| PWM Frequency     | \~200 kHz                  |
| LC Filter Cutoff  | \~38.6 kHz                 |
| Output Power      | \~10–20 W                  |
| Efficiency        | >90%                       |
| PCB Size          | 2-layer board              |
| Bluetooth Support | Yes (MHM-28, stereo input) |

## 🔋 Power Supply

* LM7805: 5V logic rail
* LM7812: 12V gate driver rail
* Capacitive decoupling at regulator input/output

## 📡 Bluetooth Audio Interface

The MHM-28 module supports:

* Bluetooth V4.0 with A2DP
* Stereo analog output
* Easy pin-header integration
* Direct input to comparator stage

## 🎯 Applications

* Portable wireless audio systems
* DIY speaker projects
* Embedded systems with audio output
* Energy-efficient signal amplification

## 🧠 Learnings

* Class D amplifier design theory
* PWM signal processing and dead-time logic
* High-frequency PCB layout techniques
* Filter design and frequency response analysis
* Bluetooth module integration

