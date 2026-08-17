# LIMINAL TOUCH

**Reactive Relics — Experimental Device**

LIMINAL TOUCH is a proximity and touch-sensitive electronic relic developed as part of the Reactive Relics instrumentarium.

The device explores the relationship between **body, electrical field, presence and sound**, using a three-electrode sensing system connected to an Arduino Nano.

It became the hardware and firmware basis for subsequent experiments with continuous body interaction, including **LIMINAL WATER THEREMIN**.

---

## FUNCTION

LIMINAL TOUCH detects changes produced by the presence and interaction of the body around three conductive electrodes.

The three sensing channels provide independent information that can be interpreted by the firmware to create interactive behaviour.

The device was developed as an experimental sensing platform rather than as a conventional controller.

---

## HARDWARE

### Microcontroller

* Arduino Nano
* 3 × conductive electrodes
* Analog sensing through three independent inputs
* Digital serial / audio outputs

### Electrode inputs

```text
E1 → A0
E2 → A1
E3 → A2
```

The three electrodes constitute the core sensing system of the device.

---

## OUTPUTS

```text
D2 → TX
D3 → AUDIO / PWM OUT
```

The digital outputs are used by the firmware for communication and sound generation in the related instrument configurations.

---

## FIRMWARE

### Stable test version

`LIMINAL_TOUCH_V1_1_TEST_750`

This version is retained as a stable reference for the three-electrode sensing hardware.

It provides the validated basis for reading and detecting changes from the three electrode channels.

---

## STATUS

**STABLE — HARDWARE REFERENCE**

The LIMINAL TOUCH sensing system is considered a validated hardware basis for further Reactive Relics devices.

---

## GENEALOGY

```text
LIMINAL TOUCH
      │
      └── 3-electrode sensing system
                │
                ▼
      LIMINAL WATER THEREMIN
                │
                └── continuous proximity interaction
```

LIMINAL TOUCH is therefore not only an individual device, but also a technological ancestor within the Reactive Relics instrumentarium.

---

## NOTES

This document describes the current validated configuration.

Experimental firmware, alternative mappings and later developments should be documented as separate versions rather than replacing the original stable reference.
