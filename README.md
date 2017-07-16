# 3DS RNG Tool [![Build status](https://ci.appveyor.com/api/projects/status/p58tu8nai3cqexuq/branch/master?svg=true)](https://ci.appveyor.com/project/wwwwwwzx/3dsrngtool/branch/master)

This is an RNG Tool for main 3DS Pokemon games. Some parts should work with [PokeCalcNTR](https://gbatemp.net/threads/pokecalcntr-for-gen-6-the-rng-tool-suite-for-the-3ds.473221/) using NTR-CFW.

This tool is a complete rewrite based off my SMEncounterRNGTool with largely improved performance and the following features:
- Gen6 RNG. including stationary Pokemon(95%), Mystery Gift Pokemon(100%), wild Pokemon(60%), Eggs(100%) and ID(90%).
- Gen7 stationary, Mystery Gift and wild Pokemon RNG from my SMEncounterRNGTool.
- Gen7 egg RNG and ID RNG based on Quandra's [PokemonSunMoonRNGTool](https://github.com/Quandra/PokemonSunMoonRNGTool) 
- Nidoran line/Volbeat/Illumise gender prediction and shortest accept/reject path solution for Gen7 Egg RNG.

## User Guide and Useful References

- [Final Screen](#final-screen) you should wait at and make the final key pressing.
- [Reddit Gen 6 RNG Megathread](https://www.reddit.com/r/pokemonrng/comments/6fhnb8/gen_6_rng_megathread/)
- [Gen VI Events Thread](https://projectpokemon.org/forums/forums/topic/39398-gen-vi-event-contribution-thread-2017/)
- [Gen VII Events Thread](https://projectpokemon.org/forums/forums/topic/39400-gen-vii-events-contribution-thread/)

## Credit

- Zaksabeast, Zep715, Real96, Admiral Fish and Shiny_Sylveon for great teamworks on gen6 development  
  Zaksabeast and Admiral Fish for building up the plugin  
  Real96 for testing and lots of good advice  
  Zep715 for figuring out tons of infomation from the assembly  
  Shiny_Sylveon for contributions to Gen6 Egg RNG
  
- Kaphotics for PkHeX and Pk3DS. I borrowed some code from the PKHeX Core Library and extracted ROM info using Pk3DS.
- 44670 for NTRClient.

## Final Screen

Usually it's the last screen before the battle starts, or the special dialogue box.

#### Generation 6

- __Pokemon Link__: _Would you like to retrieve data using Pokemon Link? Yes/No_
- __Fossils__: _This is xxx! Please take good care of it._
- __Kalos/Hoenn Starters__: _Choose this Pokemon? Yes/No_
- __Horde__: Sweet Scent / Honey Selected. USE/GIVE/DISCARD
- __Rock Smash__: _Would you like to use Rock Smash? Yes/No_
- __Mystery Gift__: _xxx received xxx!_
- __Eggs__ from Day Care: 
Accepting: _You do want it. don't you? / You'll be wanting it won't you?_  
Rejecting: _Well then, I'll hang on to it. Thank you! / Well then, I'll hang on to it. Thank you!_
- __ID__ : _xxx... Tres bien! What a fantastic name! / So you're xxx? Yes/No_

##### XY
- __Mewtwo__: _Mew!_
- __Xerneas/Yveltal__: _Xshaa!/Ygaaa!_
- __Zygarde__: _Zzzz-dddd-aaaaaa!_
- __Kanto Legendary Birds__: No dialogue.\* Press arrow key to run to it.
- __Pidgey__: No dialogue.\* Wait at the first line of the grass. The encounter will happen at the 2nd row of grass. Press arrow key to run to it.
- __Kanto Starters__: _You picked xxx. then! I see. That's simply wonderful!_
- __Snorlax__: _Snorlax opened its eyes wide!_
- __Lucario__: _Lucario is staring intently at xxx. Will you take Lucario with you? Yes/No_
- __Lapras__: _Would you mind taking Lapras with you on your journey? Sure!/I coundn't_
- __Berry Tree__: _A Pokemon appeared!_
- __Shaking Trash Can__: No dialogue.\*

##### Omega Ruby and Alpha Sapphire
- __Portal(Hoopa Ring)__: _Would you like to put your hand deep in the hole? / Would you like to examine it? Yes/No_
- __Soaring Legends__: _Despite that, do you want to fly into the clouds? / Do you want to fly into the gap? Yes/No_
- __Storyline Latios/Latias__: _xxx joined your team!_
- __Eon Ticket Latios/Latias__: _Hyahhn!_
- __Primal Kyogre/Groudon__: No dialogue.\*  (The delay varies from console and save, and should be an odd number)
- __Rayquaza__: _Kiiiryarrrarrrarrrraaaashiiiii!!!_ (Tip: Wait until it finishes its movement)
- __Deoxys__: _The stone tablet before you--!!!_
- __Regirock, Regice and Registeel__: No dialogue.\*
- __Regigigas__: _Zut zutt!_
- __Starters(Gen 2/4/5)__: _Yes, that one from the xxx region._
- __Wrumple__: No dialogue.\* Wait after the second step in grass. The encounter will happen at the 3rd steps in grass. Press arrow key to run to it.
- __Cosplay Pikachu__: _You'll really, really, really stand out if you two go on stage with matching costumes!_
- __Castform/Sharpedo/Carmerupt/Gift eggs(Wynaut/Togepi)__: _xxx recieved xxx._
- __Beldum__: _xxx obtained a Beldum_
- __Spiritomb__: _Shahhh!_
- __Kecleon__: _The startled Pokemon attacked!_
- __Voltorb, Electrode__: No dialogue.\*

##### Tip: 
 \* For consistent delay, use D-pad (arrow keys) to move along grid.  

#### Generation 7
##### Sun and Moon
- __Tapus__: _Tapu ko-ko-ko-kooo!!! / Ta-pu-leeeh! / Ta-pu-loooo! / Ta-pu-fiiieee!_
- __Solgaleo/Lunala__: No dialogue.
- __Zygarde__: _Zygarde has gone into a Poke Ball!_
- __UBs, Island Scan & wild Pokemon__: Press A and thus enter the bag from X menu.
- __Type:Null/Cosmog/Porygon/Aerodactyl/Magearna/Fossils/Gift Eevee egg and Mystery Gift__: _You received xxx!_
- __Crabrawler__: _There was a Pokemon feeding on the Berries and it leaped out at you!_
- __Pikipek__: No dialogue. Before the fourth step in grass.
- __Exeggutor__: _Ahhh! What is that, xxx?!_
- __Main RNG egg__: _But you want the Egg your Pokemon was holding. right?_
- __Starters__: _Having accepted on another, you'll surely be friends for life._
- __Poke Pelago__: Press A and thus go to Poke Pelago from X menu.
