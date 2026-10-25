This is my journal for the project. I didn't know I was meant to journal at first, so the first journal is quite long, I thought lapse was all that was needed as that is what I had been told. The first journal is a few sessions lumped into one.

# Journal 1 - 25h
## CAD
To outline what the project will look like, it will be an airliner style rc plane. The main elements of the project are the plane CAD, with things like engines, control surfaces etc, then a PCb flight controller, software, and a remote control.
The propulsion method i'm going with is an EDF, which produces a lot of thrust. I'm using QF2611 50mm EDFs, which should be sufficient.

<img width="220" height="220" alt="image" src="https://github.com/user-attachments/assets/d15a4cf3-aa4a-4cb7-98be-f3c88cebd6a5" />

Based on it being a twin engine plane, and each EDF making around 800g thrust, the total thrust is probably about 1.5kg, which is heaps.
I found dimension sheets of the EDF and added them as a canvas in Fusion. I started sketching the EDF.

<img width="553" height="501" alt="image" src="https://github.com/user-attachments/assets/c24f18b0-aeb8-4dce-bfd2-e022268782a5" />

<img width="731" height="655" alt="image" src="https://github.com/user-attachments/assets/1f8dad94-1f51-46b4-b6e8-21f297763f56" />
<img width="576" height="536" alt="image" src="https://github.com/user-attachments/assets/238befa7-1728-41e0-8d44-4df61328615a" />
<img width="438" height="469" alt="image" src="https://github.com/user-attachments/assets/959ef932-baba-4e73-bb20-9c76039ef34e" />

There are three threaded holes at the rear of the motor that I will use to mount the EDF, as glue would be weakened by vibrations.

<img width="603" height="556" alt="image" src="https://github.com/user-attachments/assets/f35a168f-065d-4768-a355-2a49a0f61496" />
<img width="816" height="613" alt="image" src="https://github.com/user-attachments/assets/b2374c40-b4b9-4285-86f9-73841f692693" />

I made my own model of the fan is this bit doesn't need to exactly replicate the EDF, as no parts really rely on it.

<img width="692" height="631" alt="image" src="https://github.com/user-attachments/assets/8610078b-66e4-463c-b86c-710e50904656" />
<img width="772" height="700" alt="image" src="https://github.com/user-attachments/assets/04429cb9-645b-413f-9a36-6ab3e88024bc" />
<img width="441" height="434" alt="image" src="https://github.com/user-attachments/assets/31f92e35-7589-42a2-afea-02d5fa781fac" />

Now with the engine made, I started working on the nacelle, which will be 3d printed. This is the piece that secures the engine and will be mounted to the wing.
I built a cylinder with a 54mm hole to suit the EDF, then filleted it and sketched curves to match a real engine shape, and used the revolve tool to make it. I added spokes to a flat pieces to mount to the three threaded holes on the motor, lining up the spokes with the spokes of the EDF.

<img width="584" height="236" alt="image" src="https://github.com/user-attachments/assets/c72fe792-889c-4712-94df-bfd37968b2e5" />

I reduced the diameter of the exhaust hole so that I could get a nice shaped curve throughout the engine.
<img width="434" height="328" alt="image" src="https://github.com/user-attachments/assets/5da46ed3-9023-40e4-ab03-a8db83dff93c" />

I then started making the engine pylon, which goes to the wing. This has to be hollow for the EDF wires.
<img width="577" height="491" alt="image" src="https://github.com/user-attachments/assets/ff50bf05-db59-490c-82b1-97073ae28080" />
<img width="483" height="466" alt="image" src="https://github.com/user-attachments/assets/e660cbfb-3fce-4837-b38c-47cd57d2b500" />

I worked on the wing. First I need to outline some specs. I will use a 28 degree wing sweep (angle of wing from being 90 degrees from fuselage), with 3 degree angle (incline). My plane is tom make profiles and then loft between them.
I made a sketch of the root, with a hollow section for cabling etc.

<img width="1144" height="446" alt="image" src="https://github.com/user-attachments/assets/e8cab51b-b28e-4c1d-ab20-32f0987f8ef6" />

I tried a few different ways to sketch rails for the wing but it wasn't working with the sweep and incline, so instead I used trigonometry to find the point of the wing tip and sketch a profile around that point.

<img width="649" height="225" alt="image" src="https://github.com/user-attachments/assets/9d48019a-a5c9-424f-8eb9-85017631b517" />

Then I could draw a line between corresponding points.

<img width="898" height="473" alt="image" src="https://github.com/user-attachments/assets/058f4a0a-8194-41de-b077-9571b4e057ae" />

<img width="954" height="324" alt="image" src="https://github.com/user-attachments/assets/afb74eca-8a70-418a-9f0c-9615aaf9763c" />

Then I added washout (twist) in the wing of 2 degrees. I made the mid wing profile:

<img width="938" height="441" alt="image" src="https://github.com/user-attachments/assets/406cbabf-9baf-40f3-a298-3edb63e5b696" />

I lofted the wing.

<img width="769" height="562" alt="image" src="https://github.com/user-attachments/assets/39a8a4a5-066d-48fd-ba58-e910a1597bd6" />

For the flight control surfaces on the wing, there are flaps, and ailerons. One of the flaps might be a flaperon (hybrid of both). I messed about making a sketch trying to split the body.
I was stuck on whether the aileron should be3 perpendicular to flight direction, or wing leading edge. In the end I decided on flight direction, so I made a sketch to split the aileron. This gave me a wedge shape. I thought about how to control the aileron, fitting a servo would be hard. My plan is to mount a servo in the fuselage, and have it pull cables that run through the wing to the aileron. I sketched out two cylinders on the aileron for the cable to loop around. I need a way to make the aileron pivot without colliding with the wing.

<img width="623" height="597" alt="image" src="https://github.com/user-attachments/assets/c9283f3d-09e3-4e14-a6fb-b06172a52512" />

I added a 90 degree bend shape with holes to route the cables, thick enough for a cover to stop the metal wearing away the 3d print. In between the swept holes, there is a hole for a 2mm dowel that the aileron arms pivot around, making the aileron move without hitting the wing.

<img width="580" height="377" alt="image" src="https://github.com/user-attachments/assets/5b8408f9-f16c-4c16-a92b-16e2065b7242" />

<img width="712" height="559" alt="image" src="https://github.com/user-attachments/assets/fb87b24b-b8d8-49d5-8d2d-9d5d33c0c928" />

for the flaps I took the same sort of process, but I won't use the cabling system. I will find another way.
I separated them into flaps, the inboard one is slotted fowler flap. I am yet to work out the motion mechanism.

Next I made the fuselage. I took a canvas of a boeing 777, and matched it with that. For the nose, I used lines depicting the height to make circles matching the gradual slope and change of the nose, same with the tail end. I extruded a tail shape and filleted to match. I made horizontal stabilisers using the same process as the wing, though these are still being worked on. Then I added a central bulge where the wing will meet the fuselage.

<img width="921" height="645" alt="image" src="https://github.com/user-attachments/assets/ed9b332c-9a60-48cb-aa77-a3a4eb5bc388" />

<img width="721" height="783" alt="image" src="https://github.com/user-attachments/assets/531807ed-0472-4f7b-b227-36f89cc86d5e" />

The elevator is on the stabiliser. It has the same pivot method as the aileron, though it is actuated by pushrods that lead to servos in the fuselage. I added slots for the servos in the fuselage.

<img width="463" height="359" alt="image" src="https://github.com/user-attachments/assets/6f41e03a-ffd4-4643-87d2-a2a622a04769" />

Next I started working on the nose landing gear. This would be a significant challenge. The nose gear must be able to retract, steer, and the bay doors must open and close. I followed one design philosophy with two pieces. The lower piece mounts the wheels (32mm diameter) and has two holes. The lower hole pivots on the top piece, and the upper hole mounts a spring, providing suspension.

<img width="511" height="748" alt="image" src="https://github.com/user-attachments/assets/1773f35d-6ec1-4a23-90ac-060e79e67168" />

This however was quite bulky, so I decided to try a different approach. I replicated similar to what actual planes have. The lower piece has a cylinder above it.

<img width="481" height="375" alt="image" src="https://github.com/user-attachments/assets/dc300519-3101-4919-807d-af4ed75c2d78" />

The upper piece is a hollow tube that slide over the lower piece, with a spring sitting inside the tube, pressing against the two pieces, providing suspension. To stop the lower piece falling out, there are rotating bars that extend to the lowest height of the gear. The lower bar pivots around the axle, attaches with an M2 screw to the upper bar, which mounts onto the main strut with an M2 screw.
<img width="430" height="565" alt="image" src="https://github.com/user-attachments/assets/f1991b00-a1bf-443b-8ddb-e2ed471d5237" />

The top piece has a toothed hole that matches the drive shaft of an SG90 servo. Through this, the servo rotates both the top and bottom pieces to move the nose wheel.

<img width="554" height="662" alt="image" src="https://github.com/user-attachments/assets/6f8256ac-cf74-4c85-8f31-85fa767a7a54" />

This is the main mechanism of the nose gear. The retraction part of the gear centers around a triangular strut. The triangle strut mounts the SG90 servo, and attaches to the middle of the top piece as 2 parts with M2 screws. The tri strut features a pin on either side to rotate around in the fuselage. the tri strut does not rotate, only the piece of the nose gear rotate.

<img width="542" height="702" alt="image" src="https://github.com/user-attachments/assets/9804017e-90b8-4902-a033-3c0d19636350" />
<img width="592" height="536" alt="image" src="https://github.com/user-attachments/assets/2dffbebe-5289-47dd-bd99-fc3981ed615a" />
<img width="577" height="454" alt="image" src="https://github.com/user-attachments/assets/536d176f-1a89-42c9-bf9a-207dbcbb79d6" />

To retract the gear, I used a mini linear actuator. It pulls a point on a bar in, folding two bars over themselves. The bottom of the bars mount to the screw hole on the tri strut, pulling the gear up, and extending when the actuator extends. Retracted position:

<img width="849" height="358" alt="image" src="https://github.com/user-attachments/assets/90a7a662-f840-4421-9d89-46ddae083901" />

I added a bar to mount the rectraction bars.
<img width="274" height="277" alt="image" src="https://github.com/user-attachments/assets/3e965bca-c604-4dce-8e27-f73a7100a546" />
<img width="687" height="501" alt="image" src="https://github.com/user-attachments/assets/dfc03843-a70a-4718-aca0-3495c00f21d2" />


I added holes in the fuselage for the strut pins to rotate in. I had to move the gear back in the fuselage a few times so that it can fit in the nose when retracted. My next challenge was the gear doors, I tried a few different things like different mounting and servo positions, though everything keeps causing collisions with the main fuselage. Originally I had the servos mounted vertically, either side of the nose gear, though I realised this made it very cramped for no reason. I have split the door body from the fuselage, but any mounting point within the fuselage means edges collide. The servo sits back and will rotate a bar, pushing/pulling the door up or down. I had to carve out a lot of space and chamfer a fair bit to make the gear fit.
<img width="670" height="560" alt="image" src="https://github.com/user-attachments/assets/1397ddd0-3bfe-4447-8382-abdf808efe5d" />

<img width="576" height="387" alt="image" src="https://github.com/user-attachments/assets/52ce4c2e-fdac-4cae-b0cc-a60c3750cb6d" />

My new plan is to have the doors pivot on the edge of the fuselage, though doing this will be a challenge, but I will approach this next session.
