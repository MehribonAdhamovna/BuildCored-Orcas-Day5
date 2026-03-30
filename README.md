# BuildCored-Orcas-Day5
FaceEQ — BUILDCORED ORCAS Day 05

What it does. I built a controller that uses a webcam to track your head movements and manipulate music in real-time. Turning your head left or right scrubs through the track, while tilting up or down adjusts the playback speed.

Hardware concept. The project treats your head as a physical rotary encoder, where rotational displacement is translated into digital control signals. Specifically, yaw and pitch act as two independent axes that feed position data directly into the audio engine.

What I would do differently. I’d definitely look into using a more robust audio library like sounddevice or pydub because pygame gets a bit glitchy when you rapidly change playback speeds. I also think adding a smoothing algorithm for the scrubbing would make the seeking feel a lot more fluid and less jumpy.

Run it. python day05_starter.py
