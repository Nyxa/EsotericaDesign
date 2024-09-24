### General
- Things between `backquotes` are placeholders meant to be replaced with a proper item name.
- Things inside Curly Braces {**CB**} denote an abbreviation that will be used from here on out.
- Important qualifiers *will* be italicized.
- **Names** may be bolded in order to draw attention to them, or distinguish them from similar words.

### Gameplay
The **Gameplay** section includes information on gameplay systems & mechanics, boss fights, explorable areas, interactable entities, and useable items. Each of these categories is sorted into their own subdirectory, which each have their own subdirectories and slightly different workflow.

#### Regions
The **Regions** subsection is divided by subfolders for each explorable region within the game. It does *not* include regions which are part of the lore/history of [[Eiare]] but cannot be visited in-game.

Each **Region** folder has two relevant folders: **Points of Interest** and **Subregions**. They also all contain four different files: **Overview**, **NPC**, **Enemies**, and **Notable Miscellanea**. What each of these are for is outlined below.

##### Points of Interest
Each **PoI** is typically a location within a sub-region, such as an abandoned village, or an important statue of an unknown god. These files *must* contain a link to the **Subregion** they are located in. [Lumina](1.%20Overview.md) comes with an example layout already, as well as appropriate linking in its **PoI** section.

##### Subregions
Each **Subregion** is a visually distinct area within a **Region**, that follows its theme. One example is how [Lumina](1.%20Overview.md) comprises the [Caverns](Lumina%20Caverns.md) and [Forest](Lumina%20Forest.md)—both of which following Lumina's theme of bioluminescence—but also contains [Oscura](Oscura.md), which does the opposite of Lumina's theme and is shrouded in an impermeable darkness. Subregions *must* contain a description of their visual themes, as well as their purpose for existing in the world of Eiare, and may also include some detailing of their history.

The history of Eiare itself will *not* be localized to individual history files, as character and location backstories have too much overlap, and things would get very messy very quick if we tried to compartmentalize. Instead, relevant history will be added to relevant files, regardless of the categories of said files.

##### Overview
Each **Overview** file contains a thorough description of the region's *themes* and *purpose* in the story of U:TR, but does *not* contain specific information about navigation paths, enemy placements, or otherwise. This is reserved for map images, which *must* be added to a Region's **Overview** file when completed. 

Additional images (such as visual references, and completed environmental concept art) also *must* be added to a Region's **Overview** file when completed.

##### NPC
Each **NPC** file *must* contain a list of *all* NPCs that may be found within that **Region**. 

The file *must* be formatted as follows:
[NPC Name] → [Nearest Location]

Where [NPC Name] is a link to the NPC's **Character** file, and [Nearest Location] is a link to the highest fidelity location of the NPC in question. As an example, [Lady Lazuli](Lady%20Lazuli.md) can be found within the [Maylith Stronghold](Maylith%20Stronghold.md), so the Lumina **NPC** file would contain the following:

[Lady Lazuli](Lady%20Lazuli.md) → [Maylith Stronghold](Maylith%20Stronghold.md)

The **Lumina** folder contains an example [NPC](2.%20NPC.md) file.

##### Enemies
The **Enemies** file follows the same formatting and conventions as the **NPC** file, but it *must* link to the appropriate **Enemy** file rather than a **Character** file. Character files contain information about who a character is, what they look like, what they want, etc.; while Enemy files contain information about how a character fights, what their weaknesses are, and what rewards they may give.

While these are separate files for the time being, they *may* be unified at some point. In that case, **NPC** and **Enemy** files must link to the appropriate *subheading* within that file, instead.

##### Notable Miscellanea
The **Notable Miscellanea** file exists to contain all things which are worth listing in their own separate file. There is *no* standard convention for how to format these files, but you should use the aforementioned notes on the other files and sections as a guideline for how to keep these clean.