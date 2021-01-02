![VSH2 Logo by Nergal/Assyrianic](https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/efc8ece3-f4a3-4477-8ebb-cb9595fb9e58/ddiv9m4-cbc4d719-c2fd-4890-b62a-17be7f01210f.png?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7InBhdGgiOiJcL2ZcL2VmYzhlY2UzLWY0YTMtNDQ3Ny04ZWJiLWNiOTU5NWZiOWU1OFwvZGRpdjltNC1jYmM0ZDcxOS1jMmZkLTQ4OTAtYjYyYS0xN2JlN2YwMTIxMGYucG5nIn1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmZpbGUuZG93bmxvYWQiXX0.JjuSnfGa4fwWanCRmVmvkaI5GV9u5PYReeJ9ll1AIBQ)

#### Current STABLE Version: *2.0.5*
[![Master Build Status](https://travis-ci.org/VSH2-Devs/Vs-Saxton-Hale-2.svg?branch=master)](https://travis-ci.org/VSH2-Devs/Vs-Saxton-Hale-2)
#### Current DEVELOPMENT Version: *2.9.27*
[![Develop Build Status](https://travis-ci.org/VSH2-Devs/Vs-Saxton-Hale-2.svg?branch=develop)](https://travis-ci.org/VSH2-Devs/Vs-Saxton-Hale-2)

**[VSH2 Addons Repository](https://github.com/VSH2-Devs/VSH2-Addons)**


VSH2 is rewrite of VSH1. VSH1 and FF2 both had a very bad code framework using shoddy, hacky coding. I could even go as far to say they probably had no framework at all and even no real structure to its code.

VSH2 actually has a structured, event-based framework and combines the best features of both FF2 and VSH1 by not only having multiplayer boss support but also to make it easier to add new bosses **and** give them truly unique abilities and mechanics through giving the developer full, uninhibited control by code rather than config files.

FF2's purpose is to be very easy to add bosses in a generic, cookie-cutter manner. Of course there's a trade off: FF2 is alot more difficult, if not impossible, to truly customize boss mechanics and abilities without having to recode parts of FF2 itself. VSH2, since it requires experience with SourcePawn, is somewhat more difficult for a newbie than FF2 to create new bosses but it rewards taking the harder route by allowing you to control damn near every individual boss behavior and logic.

If you do require help in setting up the bosses or at least need some info on the API for boss building in VSH2, [have a look at the VSH2 wiki](https://github.com/VSH2-Devs/Vs-Saxton-Hale-2/wiki)

**NB:** While VSH2 will work perfectly fine as-is out of the box as a VSH1 replacement, it was designed with capable SourcePawn **_developers_** in mind to make the most out of the coded-from-scratch framework! So don't expect to be able to easily modify/add bosses if you have no prior SourcePawn experience like you would with FF2.

### Why VSH2?

* VSH2 was created to facilitate easier boss additions to a VSH-esque gamemode while having extensive customisation capabilities, even more so than FF2.
* VSH2 operates through a series of Event Handling functions across different Boss, non-Boss actions, and clear cut API which allows developers to control boss code at will and with ease.
* VSH2's game state is controlled through a singleton instance of the VSHGameMode methodmap which allows for easier management of the entire gamemode's state.
* VSH2 gives you the option to either hard code your new bosses directly into the plugin or use VSH2's vast API to build bosses as subplugins/modules!

### How do I get set up?

* Compile with spcomp
* VSH2 uses the same map configurations as FF2 and VSH1 and this is for compatibility reasons.
* Dependencies: TF2Items, MoreColors, ConfigMap.
* Optional Dependencies: TF2Attributes (https://github.com/FlaminSarge/tf2attributes), SteamTools (https://forums.alliedmods.net/showthread.php?t=170630)
* Compile plugin into .smx and put in addons/sourcemod/plugins folder
* Take a look at the [Wiki](https://github.com/VSH2-Devs/Vs-Saxton-Hale-2/wiki) to get started making your own boss!

### Who do I talk to?

* **Lead Developer:** *Nergal the Ashurian/Assyrian* - https://forums.alliedmods.net/member.php?u=176545
* **Repository Manager & Contributor:** *Starblaster 64* - https://forums.alliedmods.net/member.php?u=261662
* **Contributors:** *Scags/RageNewb* , *BatFoxKid* , *01Pollux/WhiteFalcon* .

### Contribution Rules
#### Code Format:
* Use New sourcepawn syntax (sourcemod 1.7+).
* Single line comments that convey a message must have 3 slashes: `///`.
* Multi-line comments that convey a message should have an extra beginning star: `/**`.
* Properties, functions, & methods smaller than 30 lines of code should have the beginning `{` brace in K&R C style, for example: `ret func() {`.
* Local variable names should be in snake_case.
* Property names must have a single-letter prefix of their type.
* Functions, methods, methodmaps, enums, enum values, must be named in PascalCase. Pascal_Case is also acceptable.
* Enum values used as flags may be upper-case.