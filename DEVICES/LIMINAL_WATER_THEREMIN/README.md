# LIMINAL WATER THEREMIN

**Reactive Relics — Experimental Device**

LIMINAL WATER THEREMIN is a contactless electronic instrument developed from the three-electrode sensing system validated in LIMINAL TOUCH.

The device explores the body as a temporary presence within an electrical field. Instead of triggering a sound through physical contact, the proximity of the performer continuously alters the behaviour of the instrument.

The result is a fluid, unstable and responsive sound system with a theremin-like interaction.

---

## CONCEPT

The instrument is designed to react to **presence, proximity and distance**.

The body does not operate the device as a conventional controller. Instead, the body becomes part of the sensing field.

As the performer approaches or moves away from the relic, the electrical response changes continuously and the firmware translates these changes into sound.

No physical contact is required.

---

## HARDWARE

### Microcontroller

* Arduino Nano
* 3 × conductive electrodes
* 3 × analog sensing inputs
* PWM audio output

The three-electrode hardware architecture originates from LIMINAL TOUCH.

### Electrode inputs

```text
E1 → A0
E2 → A1
E3 → A2
```

The three channels provide independent sensing information used by the firmware to shape the instrument's response.

---

## OUTPUT

```text
D2 → TX
D3 → AUDIO / PWM OUT
```

`D3` provides the generated audio signal.

---

## CURRENT FIRMWARE

### LIMINAL_WATER_THEREMIN_V2.2

**Status: STABLE TEST / PERFORMANCE REFERENCE**

V2.2 is the current reference version for testing the instrument.

Its behaviour was validated as a continuous proximity instrument rather than a touch-triggered device.

### Current behaviour

* Continuous response to body proximity
* No physical contact required
* E2 / A1 controls pitch
* E3 / A2 controls modulation
* Large distance produces a rising pitch response
* At extreme distance the pitch can enter a high / blip-like region

The response is intentionally non-linear and contributes to the unstable, organic character of the instrument.

---

## INTERACTION

```text
BODY
  │
  ▼
ELECTRICAL FIELD
  │
  ▼
3 ELECTRODES
  │
  ▼
ANALOG SENSING
  │
  ▼
FIRMWARE
  │
  ▼
PITCH + MODULATION
  │
  ▼
AUDIO
```

The performer therefore does not simply "play" the instrument.

The instrument continuously measures the changing relationship between itself and the body.

---

## GENEALOGY

```text
LIMINAL TOUCH
      │
      │  validated three-electrode sensing
      ▼
LIMINAL WATER THEREMIN
      │
      ├── V1
      ├── V2
      └── V2.2
            │
            ▼
      current stable reference
```

LIMINAL WATER THEREMIN is the first major development in the instrumentarium where the three-electrode sensing system becomes a **continuous spatial instrument**.

---

## DEVELOPMENT STATUS

**V2.2 — STABLE TEST / PERFORMANCE REFERENCE**

This version should be treated as the current reference configuration.

Further development may explore:

* response curves
* pitch range
* modulation behaviour
* distance sensitivity
* inertia / smoothing
* electrode geometry
* physical construction
* acoustic character

Experimental changes should be developed as new versions rather than modifying the V2.2 reference.

---

## RELATED DEVICES

* [LIMINAL TOUCH](../LIMINAL_TOUCH/)
* LIMINAL WATER THEREMIN V2.2

---

## NOTES

LIMINAL WATER THEREMIN is part of the Reactive Relics instrumentarium: a collection of experimental objects situated between electronic instrument, sensing system, ritual artefact and speculative technology.
