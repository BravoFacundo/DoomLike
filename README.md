# DoomLike

[Work in progress] Shooting video game based on “Billboard” graphics or 2.5 D. Made in Unity, C#.

*Si lo prefieres, puedes leer esto en [español](README.es.md)*

# Technologies

Developed using:
- C# Language
- Unity 2021

*You can see the code [here](Assets/Scripts/).*

# Idea and development

This video game is designed to explore the development of a retro shooter as well as the implementation of billboard graphics in a precision shooting game.

Commonly billboarding is used only as an aesthetic appearance and is not related to the 3D environment, thus it does not hinder other systems (such as collisions).
The challenge proposed here is to use the sprite as a pixel-perfect collision detection system with high visual precision.

Making a retro shooter allows me to limit the size of the project and different aspects that make the use of billboard graphics more complex, such as: necessary animations, viewing angles, reactions to mechanics, etc.

# Implementation

To achieve the use of the sprite as a hitbox, a raycast system was implemented with impact coordinate detection on the sprite texture.
Later it is checked if the pixel in that coordinate belongs to the alpha of the image. *See the script [here](Assets/Scripts/Test.cs).*

If the RaycastHit on the texture belongs to the visible part of the image then it is considered an impact.
If it belongs to the invisible part of the image (its alpha) then it is not considered an impact and is discarded.

In the same way you can check the same impact coordinate on different stored textures (which can also be animated).
Allowing to determine areas that multiply the damage or trigger certain events.

# Links and credits

Animations were reused from a collaborative video game project.

Artists:
- Dose (Jose Bayugar): [Behance](https://www.behance.net/bayugarj79c4) - [Instagram](https://www.instagram.com/dose_jb/)
- Ikumi: [Instagram](https://www.instagram.com/ikumi_arte/)

