# KarplusStrong
A Synth written in Pure Data using Karplus-Strong algorithm that is meant to simulate plucked string

Project Purpose

Use this patch in music production is my ultimate goal. Also future plans (or dreams) involve this patch in a workstation app for Raspberry Pi and Android Devices that will emulate Computer-less music production on a computer (that doesn't sound right, i know). But for mow I wnat to use it in my small synth rig on a Raspberri pi with Midi keyboard attached.

TODO:

1. Create a GUI
2. Make computer keyboard play notes on this synth.
3. Create effects rack (od/fuzz/clip, delay, reverb at least)

Dependencies:

Pure Data Pd 0.47.1

Installation

1. Install Pure data on your system
2. Install Ggee externals library or just the moog~ external
3. Run ks-synth.pd file with PD

Included Abstractions

ks.pd - an oscillator with 2 lo pass filters and the Karplus Strong algorithm itself.
pink.pd - a filtered out [noise~] to provide the synth with pink noise source
apkknobs.pd - an abstraction mapping 8 midi knobs (cc 1-8) to outlets.

Synth Architecture

midi note > oscillator > DAC

About the author

I'm a non professional and non commercial musician. I play guitar and now some synths also. When I got my first analog synth I was blown away with what you can do if you don't have to navigate menus for doing stuff. So in this project I will try my best to stick with "One Knob = One Function" concept. (at least for my APK Mini)

