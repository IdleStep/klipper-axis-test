# klipper-axis-test -- Axis & CoreXY Motor Torture Test

A Klipper (or Kalico) macro for testing printer motion systems,
including full axis testing and isolated CoreXY motor diagnostics.

------------------------------------------------------------------------

## Features

-   Tests X, Y, Z axes
-   Isolates CoreXY motors (A & B)
-   Configurable axis, cycles, amplitude, and speed

------------------------------------------------------------------------

## Installation

   1. Add the `axis_test.cfg` macro file to your Klipper configuration directory, then include it in your `printer.cfg`:
   ```ini
   [include axis_test.cfg]
   ```
   2.  Restart Klipper.

------------------------------------------------------------------------

## Usage

AXIS_TEST AXIS=`<X|Y|Z|A|B>` AMP=`<mm>` CYCLES=`<count>` SPEED=`<mm/min>`

------------------------------------------------------------------------

## Parameters

AXIS: Which axis to test. Default = `Z`

AMP: Movement distance from center in mm. Default = `1`

CYCLES: Number of oscillations. Default = `100`

SPEED: Movement speed in mm/min. Defaults: - X/Y/A/B = `6000` - Z = `600`

------------------------------------------------------------------------
