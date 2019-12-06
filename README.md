Rogue-like game developed in rust following guide at https://tomassedovic.github.io/roguelike-tutorial/

All credits to the author.

Found mistakes in tutorial:
part 9 - spells - confusion spell part:
function 'target_monster' doesn't exist, expect it should be 'closest_monster'

Targeting fireball:
add `&mut Map` to  `cast_fireball` but it's not used anywhere
Switching from i32 to f32 is a bit confusing as some methods from before expect / return i32 but new one expect / return f32