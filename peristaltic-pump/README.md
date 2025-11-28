# MicroLab Peristaltic Pump

These files are 3D part designs that can be printed and used to build an essential component of 

v0.1-alpha - interfacing with Pumps Box not yet complete.

## What is a Peristaltic Pump?

Peristaltic pumps are a type of pump that compresses a tube using rollers. The rollers move across the surface of the tube, squeezing it and forcing small amounts of liquid through with each turn of the pump head. You know how you can get the last bits of toothpaste out of the toothpaste tube by squeezing it between your hand and the edge of your bathroom sink? It's like that.

This style of pump is named after peristalsis, which is the coordinated contractions that help move food through your intestines. Peristaltic pumps allow fluids to be pumped without ever coming into contact with the mechanical parts of the pump. The tubes can be easily replaced, which mains the pumps easy to maintain.

## Pumps in the MicroLab

The MicroLab uses a series of three pumps driven by stepper motors as part of the Pumps Box in the Reactor Unit. These pumps inject chemicals into the reaction chamber. The current designs recommended off-the-shelf peristaltic pumps but these are often hard to source. This pump is a DIY, open-source alternative. You can also use the [syringe pumps](https://github.com/FourThievesVinegar/microlab-parts/tree/master/syringe-pump)

## Building a MicroLab Peristaltic Pump

### The Printed Parts

First, you will need the printed parts files in the `files-STL` directory. The `images` directory contains renders of the various parts and their assembly.

### Tools

You will also need the following tools:

- soldering iron
- drill with various bits (optional but recommended)
- 2 wrenches (or a wrench with a drill with hex head attachments)

### Parts / BOM

#### Electronics

- 1x Nema17 stepper motor, 5mm shaft with fiduciary notch in shaft

#### Fasteners

- 7x M3 heat-set inserts. McMaster Carr: 94180A331 , https://www.mcmaster.com/products/heat-set-inserts/ . $20.44/100 ct
- 4x M3x32 screws (or longer)
- 4x M3x6 screws
- 3x M3x4 screws
- 6x 608 skate bearings
- 6x M8 nylock nuts
- 3x M8x? buttonhead bolt

#### Tubes
- 3/8"OD,1/8"ID latex tubing 
  - We are working on designs for tougher silicone tubes. The FreeCAD file is parameterized, so you should be able to modify the pump to work with different tube sizes if you want to.

### Preparation

#### To Begin

Print models on 3d printer. Use 30% infill or higher. Average quality settings are perfectly fine here.

#### Cleanup of printed parts

Once parts are done, carefully ream the M3, M5, and M8 holes with a drill so that the respective screws can go in without friction.

- M3 holes are the outer 4 holes, and the 4 holes connecting the stepper to the printed frame.
- M5 hole is on the bearing holder parts where the stepper shaft interfaces. (Note, if you have a 8mm stepper shaft, you can drill this part out to 8mm. Be careful and slow if you do)
- M8 holes are the bearing holder parts that hold the 608 bearings.

### Assembly

#### Stepper Base Heat-set Inserts

- Pump Base printed part
- 4x M3 heat-set inserts

On the Pump Base part, on the flat side, the outer 4 holes have a recess in them that looks like they are for a screw head. These are for heat-set inserts.
Carefully press in an insert on each outer hole of the stepper base using the tip of a hot soldering iron. To remove the soldering iron, twist while removing.
After they have cooled, remove any melted plastic debris that may have ben pushed.

#### Bearing Holder Heat-set Inserts

- Bearing Holder Bottom printed part
- 3x M3 heat-set inserts

Insert 3x M3 heat set inserts into the Bearing Holder Bottom. Carefully put on a heat-set insert on the tip of the soldering iron. Make sure the larger flat head is facing towards the soldering iron handle. Carefully press in an insert on each side of the Bearing Holder Bottom. To remove the iron, twist while gently pulling it out.
After they have cooled, remove any melted plastic debris that may have ben pushed.

#### Attach the Stepper Motor to the Pump Base

- Stepper motor
- Pump Base printed part
- 4x M3x6 screws.

Affix the stepper to the base using the M3x6 screws. Note: the M3 heat-set inserts should be on the bottom.

#### Assemble the Bearing Holder

- Bearing Holder Bottom printed part
- Bearing Holder Top printed part
- 6x 608 bearings
- 6x M8 nylock nuts
- and 3x M8x? buttonhead bolts.

Note on the 2 Bearing Holder parts: on one side there is an indentation around where the bearings will go. This is a built-in spacer to allow the bearings to freely rotate when tightened.

Put the Bearing Holder with the hexagonal shape on a table with the hex pointed up. Put the button M8 screws through it so that the screw shafts are pointing up. Then put 2x 608 bearings on each screw.

Put the Bearing Holder Top on, making sure the indentation is facing towards the bearings. Finger-tighten the nylock nuts, and then use 2 wrenches to tighten completely. The bearings should freely spin.

If the bearings do not completely spin freely, very carefully untighten the respective nylock to provide just enough room for them to spin.

#### Mounting the Bearing Holder

- Bearing Holder Assembly
- Stepper Motor + Pump Base Assembly

Place the Bearing Holder assembly on the stepper shaft. Make sure to provide a small amount of clearance at the bottom, so that the bearing holder doesnt collide with the stepper base or screws. Insert an M3x4 screw into the screw hole on the hexagonal Bearing Holder part. Align the screw with the notch in the stepper shaft. When properly tightened, it should be possible to rotate the stepper shaft by turning the Bearing Holder.

#### Completing the Assembly

- Rocker Insert printed part
- Rotating Insert printed part
- Top Plate printed part

Align the respective inserts on the screw holes. Put top plate on top. Insert a M3x32 screw through the Top Plate, Rocker Insert, and Stepper Base. Screw down to finger tight.
Align the Rotating Insert with the round groove in the Rocker Insert. Insert a M3x32 screw there and screw to finger tight.

Now, you can rock the rotating AND rocker inserts back and forth in order to easily load or change peristaltic tubing.

To close up, put the remaining screws in and tighten them.
