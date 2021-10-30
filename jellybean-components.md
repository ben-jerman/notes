# 1. Introduction

## Pre-ramble

In my experience, the most daunting obstacle when starting a new hardware project wasn't the system design, requirement definitions or software architecture - it was the headache of choosing the correct components (out from hundreds of thousands of possibilities) to do the job you want of them.

A lot of this comes with experience - the more HW projects you make, the larger your knowledge of coomponent selection will be. You won't need to dig around the catalogues of major distributors to find the exact part you need (and sometimes hope desperately that's in stock) because you'll just pull the design from some previous project and the parts from your shelf.

For someone just starting out, though - that can be a completely different story.

Also, a form of GAS (gear acquisition syndrome - much to the chagrin of their significant others) is common with all EE's, either hobbyists or professional. But for some, having entire rooms, garages, sheds or sections of the house dedicated to the stacks of components to keep on hand just isn't feasible. For those people, having huge boxes filled with 20-year old PIC 16F84A's and venerable 555s or 741's on the off chance you'll need them someday pretty much sucks.

Falling into that second category, I think having a living catalogue of components for most common jobs, ones that are modern and up-to-date, would be a life-saver. Instead of having hundreds of different items in stock, gathering dust, have only tens and still be able to do 80% of everything you want on a whim.  

For the other 20%? What can I say. Dig deep into the filters of Digikey, Mouser or Farnell. Read a book an comb through datasheets. Sacrifice a chicken. It just comes with the territory ;)

## Who is this meant for?

The information gathered here will probably be most of use to hobbyists, students or beginners, but I hope that even seasoned EE's will find some useful stuff as well. And if there are any seasoned EE's reading this and vehemently disagreeing with the options presented below? I'd be really glad if you contact me and help me improve this for everyone.

# 2. How do we go about it?

## What should we focus on?

We should focus on the most common things you need to do with your electronics. Once you have that down and you won't need to use most of your energy to think about how to design a switching power supply because you only have 24V available and everything you want to do needs only 3.3, you can spend that energy on the parts of the circuit which are actually "special".

That being said, there need to be some constraints in order to prevent bloat:

1. Most components shall be SMT. SMT production techniques are now widely and cheaply available even to hobbyists (I'd argue that they're even easier than THT most of the time) and their multiple benefits are too great to be ignored. Still, if the component is only available in THT or it makes sense from an engineering perspective (e.g. for mechanical reasons) then THT is not an issue.
2. The components need to be widely available. Granted, it's 2021Q4 and the component shortage is still raging all over the place, so some leeway will be required here.
3. The components need to be reasonably cheap. Some manufacturers make amazing IC's which can do *exactly* what you need them to and make you coffee at the same time, but cost like 15$ a pop (looking at you Maxim). Not much use as a "jellybean" part.

# 3. You talk a lot.

I know. Let's get into it then:

I often need to...

* Connect wires to the PCB
* Use USB on my designs
* Power logic-level (3.3/5V) IC's from a higher voltage
* Power split-supply OP-amps from a single-ended PSU
* Add wireless connectivity
* Add Ethernet (wired) connectivity
* Signal things with blinking LED's
* Use a MCU
* Use a Op-amp for Audio signal conditioning
* Use an op-amp for general signal conditioning (up to 12 volts)
* Switch large loads with a MCU