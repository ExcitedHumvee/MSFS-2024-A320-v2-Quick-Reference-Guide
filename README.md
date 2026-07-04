# ✈️ MSFS 2024: A320neo v2 Quick Reference Guide

## ⌨️ KEYBOARD & CAMERA CONTROLS
*Note: Some of these appear to be your custom bindings.*

**Camera Controls:**
*   `Backspace`: Toggle Outside / Inside view
*   `Shift + C`: Enter plane
*   `Shift + Q/W/E/A/S/D`: Translate (move) camera
*   `Shift + Space`: Reset view
*   `Arrows` / `Right-Click Drag`: Look around
*   `Middle Mouse Click`: Lock view around
*   `Shift + 1-9`: Toggle instrument views

**Custom Camera Views (Recommended Setup):**
*   `Shift + F5` (or chosen key): **Save** custom camera view
*   `Shift + F1 - F4`: **Load** custom camera view
    *   *F1:* Landing View (over the dash)
    *   *F2:* Overhead Panel
    *   *F3:* Main Panel (PFD, ND, MCDU, FCU)

**Aircraft Controls:**
*   **Pitch/Roll:** Numpad `4`, `8`, `6`, `2`
*   **Yaw:** Numpad `0`, `.` (decimal)
*   **Trim:** Numpad `7` (nose down), `1` (nose up)
*   **Throttle:** `F2` (Decrease/Reverse), `F3` (Increase)
*   **Brakes:** `Space` | **Parking Brake:** `Ctrl + Space`
*   **Flaps:** `V` (Decrease/Up) | `B` (Increase/Down)
*   **Landing Gear:** `/`
*   **Spoilers:** `/` (Standard binding)
*   **EFB (Tablet):** `Tab`
*   **Engine Auto-Start:** `Ctrl + E`
*   **Afterburner:** `Ctrl + R x2`

---
**Video:** [A320neo v2 Tutorial](https://www.youtube.com/watch?v=d0spDi0o29Y&list=PLfHYROeW-buoSLKWsTKrWyaxiAQ4LxtJ9&index=2)

## 📋 FLIGHT BRIEFING (Example Flight)
*   **Aircraft:** A320neo v2 (Select a **Gate**, not a runway)
*   **Departure:** EGSS (Stansted) - Medium Gate
*   **Arrival:** EIDW (Dublin) - Medium Gate
*   **Routing:** Runway 22 | **SID:** UTAV1R | **STAR:** ABL14L | **Appr:** ILS 28L

---

## 🛫 STANDARD OPERATING PROCEDURES (SOP)

### 1. Pre-Flight & Cold/Dark Setup
*   **Exterior:** Go to outside camera and remove Engine Covers and Chocks.
*   **Overhead Panel** (Use your `Shift+F2` view):
    *   **BAT 1 & 2:** ON
    *   **EXT PWR:** ON (if available, lights will come on)
    *   **Strobes:** AUTO
    *   **Nav Lights:** 2
    *   **Crew Oxygen:** ON
    *   **Emergency Exit Lights:** ARM
    *   **ADIRS (1, 2, 3):** Turn all three to NAV
*   **APU Start:**
    *   **APU Master Switch:** ON
    *   **APU Start:** ON (Wait a few seconds, PFD will come on. Check lower ECAM to watch APU start).
*   **Displays:** Adjust brightness for PFD, ND, ECAM, and MCDU.
*   **EFB Tablet (`Tab`):** 
    *   Go to Options -> Set *IRS Align Time* to "Instant".

### 2. EFB Payload & Fuel
*   In the Tablet, enter your load: **Pax:** 130 | **Cargo:** 3243 | **Fuel:** 5109
*   Click **Apply Load** (Wait ~40 minutes in real-time, or skip ahead).
*   Go to **Takeoff** tab -> Press **Sync**.
*   Enter config weight (from Payload live gross weight) -> Press **Calculate**.
*   Click **Send to FMGS**.

### 3. MCDU (FMC) Setup
*   **INIT Page:**
    *   Clear any messages. 
    *   Type `EGSS/EIDW` and insert into **FROM/TO**. 
    *   *(Note: Fill out all mandatory orange boxes using sideways arrows to change pages).*
*   **F-PLN (Flight Plan) Page:**
    *   **Departure:** EGSS -> Rwy 22 -> SID: UTAV1R.
    *   **Arrival:** EIDW -> ILS 28L (Ensure it's the green active ILS, not white LOC) -> STAR: ABL14L.
    *   **Clear Discontinuities:** Press `CLR`, then click on the discontinuity.
    *   **Check Route:** Set ND dial to **PLAN**. Scroll through the flight plan using the up/down arrows on MCDU to ensure the route connects smoothly.
*   **PERF (Performance) Page:**
    *   Confirm Takeoff data, then go to NEXT PHASE until you reach the **APPR (Approach)** page.
    *   Enter Weather: QNH **997**, Temp **16**, Wind **160/5**.
    *   Enter DH (Decision Height/Radio): **105** feet.

    *   💡 How to program Transition Altitude: On the PERF TAKEOFF and PERF APPR pages, there is a field labeled "TRANS ALT" or "TRANS FL". Type the altitude (e.g., 6000) and click the button next to it. When climbing/descending past this, your PFD altimeter will flash, prompting you to press your Altimeter calibrate key (, or B) to switch between STD and QNH.

    *   🔄 How to Re-Init / Redo a Flight Plan: If you mess up your route or are doing a second flight, go to the INIT page. Type EGSS/EIDW (or your new airports) and press the button next to FROM/TO. It will ask you to confirm. This instantly wipes the old flight plan so you can start fresh!

### 4. FCU (Autopilot Panel) & Pushback
*   **Flight Directors (FD 1 & 2):** ON
*   **Altitude:** Dial to **34000**, push knob UP to set to **Managed** mode (dot appears).
*   **Seatbelts:** ON
*   **EXT PWR:** OFF (and disconnect GPU in EFB).
*   **Pushback:** Start pushback. Control steering with brakes. Make sure to stop pushback when aligned on taxiway else theres errors.

### 5. Engine Start & Taxi
*   **Beacon Lights:** ON
*   **Fuel Pumps:** All ON
*   **APU Bleed:** ON
*   **Engine Start:** 
    *   Turn Ignition knob to **IGN/START**.
    *   Flick Engine 1 & 2 Master switches up (forward).
    *   Monitor ECAM until engines stabilize.
*   **After Start:**
    *   Ignition knob to **NORM**.
    *   APU Bleed: OFF | APU Master: OFF.
    *   **Flaps:** Set 1.
    *   **Spoilers:** ARM (pull lever up).
    *   **Autobrake:** MAX.
    *   **TCAS:** AUTO / Mode to TA.
    *   **ALT RTPG:** ON.
    *   **WXR / PWS:** 1.
    *   **Taxi Lights:** ON.

### 6. Takeoff & Climb
*   **Before Line Up:** Strobes ON, TO (Takeoff) Lights ON.
*   **Takeoff Roll:** Advance throttle to **TOGA**.
*   **Liftoff:** At positive rate of climb (~3 degrees nose up), **Gear UP**.
*   **Climb:** Retract Flaps as speed increases.
*   **Autopilot:** Turn AP1 ON. Turn A/THR (Auto-Thrust) ON.
*   ⚠️ **CRITICAL:** When the PFD flashes "LVR CLB", pull your throttle back slightly from TOGA into the **CL (Climb) detent**. The Autopilot cannot manage speed if you leave it in TOGA!
*   **Altimeter:** Press `,` (or `B`) to set standard pressure when passing Transition Altitude.

### 7. Cruise & Descent
*   Check PFD: Ensure it shows **ALT CRUZ** (not just ALT).
*   **Descent Prep:** Verify your APPR data is correct in the MCDU PERF page. 
*   **Initiate Descent:** When ATC clears you to descend, dial your FCU altitude down to your cleared altitude (or initial approach altitude, like 2000ft OR 100ft) and press the knob to begin the descent.

### 8. Approach & Landing
*   **Lights & Setup:** Landing Lights ON. Ground Spoilers ARMED.
*   **Radios:** Check MCDU Radio/Nav page to ensure ILS frequency is tuned.
*   **FCU Setup:** Turn on the **LS** button (next to FD). Set ND knob to **LS mode**.
*   **Flaps:** Flaps 1 as speed bleeds off.
*   **Final Approach:** 
    *   Gear DOWN.
    *   Flaps to FULL (incrementally).
    *   Press **APPR** (Approach) button on the FCU.
    *   *For Autoland:* Turn on **AP2** (so AP1 and AP2 are both active).
*   **Touchdown:** 
    *   Retard throttle to idle at "Retard" callout.
    *   Engage Reversers (`F2`).
    *   Spoilers will deploy automatically (if armed).

### 9. Post-Landing / Vacating Runway
*   Disengage reversers at 60 knots.
*   Turn OFF Landing Lights.
*   Turn OFF Strobe Lights.
*   Turn **APU Master & Start** ON (to provide power at the gate).
*   Taxi to gate, engage Parking Brake (`Ctrl + Space`), and shut down engines.