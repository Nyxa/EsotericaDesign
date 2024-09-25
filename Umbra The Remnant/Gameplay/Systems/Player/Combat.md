<h1><center>Combat</center></h1>
***
This document details all of the combat systems available to the player. It does *not* take into account progression order, and instead details the *total* amount of combat systems that will be available throughout the game.

The systems in this document are *not* presented in any particular order.


### Glaive Throw
[[Umbra]] can throw [[Nox]] like a javelin, and it will fly in a straight line up to a maximum range, or until it hits an object or enemy. After it's attached, she may choose to **Reel** the glaive, detach it, or use it as a platform. 

**Reeling** has different effects based on the context:
- Light enemies and loose objects will be pulled towards **Umbra**, allowing her to deal some extra damage.
	- This is effectively a ranged [[Grab]] attack.
- Heavy enemies and objects, and terrain, will *not* be pulled towards **Umbra**, but she is pulled towards them instead.
	- This is effectively a gap-closing ability.

>[!info]
The glaive will *automatically* detach if **Umbra** goes out of range or attempts to use it to attack.
This means that attacking during Glaive Throw *cancels* the Glaive Throw animation.
>
>The glaive will *not* detach if **Umbra** dodges or jumps; however, **Reel** will be cancelled. 
**Reel** can be re-initiated as long as the glaive remains attached.


### Immortality
**Umbra** can *not* die; when her health is depleted, she reforms at the *nearest* [[Save]].

>[!info]
>Enemies that have previously fought **Umbra** *may* recognize her, and acknowledge that they've "killed" her before.


### Rewind
When **Umbra** is defeated by an enemy of [[Anomaly]] rank or higher, she cannot properly reform. To combat this, she's given a special [Injector](Injectors.md#Soulbrand) by [[Akira]], which allows her to rewind time to one of two specific points; either the latest phase of the current bossfight, or the *latest* **Save**.

>[!info]
> - Enemies that have previously fought **Umbra** will *not* recognize her after a **Rewind**, with some very rare exceptions.
> - Cutscenes *will* trigger again *only* if **Rewinding** to a previous **Save**, but *may* be skipped after first viewing.


### Amalgamate
Upon being defeated, **Umbra** *may* fuse with **Nox** in an all-or-nothing move, entering her "second phase" and regaining *half* of her maximum health, as well as enhancing all her *core* abilities. In return, for the remainder of the fight, she becomes *unable to heal*, and may *not* use any of her [Circuits](Injectors.md#Circuit).

Dying in this state *forcibly* **Rewinds** her to the *most recent* **Save**.

>[!info]
> - **Amalgamate** may only be activated in place of a **Rewind**; it is otherwise *not* available.
> - Any active [Stigmata](Injectors.md#Stigmata) will *remain* active for the duration of **Amalgamate**.

### Equinox
The **Equinox** is a type of Rapid Action Sequence {**RAS**} that is triggered by the following:
- Depletion of boss health bar
- Stealth kill
- Certain scripted sequences

During Equinox, **Umbra** will briefly perceive a slowdown in time. There will usually *not* be any input prompt on the screen during Equinox; however, input descriptors will appear via the [[Intuition]] system if the inputs in question have their meaning changed.

That is, if the "Attack" button becomes an option to, for example, push a rock, this *may* be indicated during an Equinox sequence.

Equinox *may* also depict Intuition helpers, such as indicating that an attack is coming from behind.

Equinox does *not* require a currently active cutscene to trigger. It may trigger during cutscenes *and* regular gameplay.

### Mercy
Certain enemies do not die upon being defeated. They simply go into an immobilized state and trigger **Equinox**. If the player chooses *not* to perform the finishing blow, this triggers **Mercy**. 

> [!info]
> After an enemy is granted **Mercy**, it will do *one* of the following:
 > - Start a questline, which *only* becomes available through **Mercy**. 
 > - Flee, regenerate a portion of their health, and attack you if encountered again.
 > - Immediately regenerate a portion of their health, and attack you again.
 > - Kill themselves.


The symbol/text for the finishing blow will include a "question mark" (or anything that evokes a similar response) to indicate that the player has a choice, in this scenario.


### Moxie
A special type of skill reserved for those whose soul extends into their weapon. Utilizing the weapon energizes it with **Qualia**, which slightly improves its damage, windup, and recovery.

The maximum potency is reached when the weapon is fully charged, further amplifying these stat increases.

Upon being fully charged, the player can perform a **Moxie Release**; a powerful special attack which uses *no* **Energy**, but completely depletes the energy stored in the weapon.

**Moxie** may *only* be gained by performing **Strikes** or **Perfect Parries**; **Normal Parry** and **Dodge** do *not* raise **Moxie**, and **Block** *depletes* it.


### The Hourglass
The **Hourglass** is a special kind of **Fetish** which gets absorbed by **Umbra**. 

It is *both* a **Fetish** and a **Soulbrand**.

It acts the **Health** and **Energy** management and display system, which allows **Umbra** to *swap* her **Health** and **Energy** at will.

> [!note]
**Umbra** can gather **Energy** through [Alliciency](Exploration.md#Alliciency),  by **Striking** or **Parrying** enemies.
Alternatively, she may expend **Health** with the **Hourglass** to gain more **Energy**.