# Foundry-VTT-Macros
Macros I made for myself that I found handy for Foundry VTT.  Based on content I found here on github.
Most maybe all of the basis is from // https://github.com/Sky-Captain-13/foundry.

The light toggle macros (in particular torch) I find myself using a lot.
You mass select tokens or just one, and hit the macro.  If the target has dim or bright light set to non zero - it turns light off
If they don't, then it will toggle to the light values I set for each of the macros.
These values are set in variables at the start of the code if you wish to tinker - this is just what I think looks good for lights.
Light opacity changed in 0.7.5 I believe - so an alpha setting of .3, for instance, results in a .55 on the "Color Intensity" within the token UI, which was previously known as light opacity it seems.

For the night vision macro:
You get a drop down.  When applied, it will set all selected tokens to have a dim vision of X amount of feet.
What I added on top of sky's code was that I put recommendations in the drop down of my concept of how much various amounts of moonlight might add.
Additionally, if you have a 5e character, it will parse their vision for darkvision - and ADD to the selected amount of vision in the following way:
They will gain BRIGHT vision in the amount of X.
They will have their dim vision set to X + darkvision.

In this way a character with no darkvision sees dim out to the ambient dim vision setting
A character with darkvision sees to bright in the amount of ambient light, and dim beyond that in the amount of their darkvision.

I found this much more realistic for simulating light conditions outside, I struggled with what to do with my many non darkvision PCs in foundry as setting them to no vision
doesn't make much sense except for the darkest of nights or a pitch black cave/room.  I tinkered with the setting a bit and found this to be a good way to simulate non pitch darkness
scenarios - and it still gives the darkvision characters a vast advantage.

