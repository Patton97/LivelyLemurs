This is the keycard. Assets include:

* Static Mesh for the keycard "keycard_mesh"
* Material for use by a blue keycard "keycard_blue"
* Material for use by a red keycard "keycard_red"
* Material for use by a green keycard "keycard_green"
* Blueprint for the keycard, which allows for changing of colour by a simple variable. (0 = blue, 1 = red, 2 = green)

I am convinced this keycard can be streamlined to dynamically create & apply materials, rather than storing & calling upon 3 different predefined materials. This could improve performance but since we're not too worried about performance right now this can be looked into at a later date.
