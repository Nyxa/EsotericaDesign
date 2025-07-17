
<h1><center>Combat</center></h1>

---
This document details *all* of the combat systems within the game. It does *not* take into account progression order, and instead details the *total* amount of combat systems that will be available throughout the game.

The systems in this document are *not* presented in any particular order; however, some care was taken to place more fundamental systems before others.

### Attributes
All characters have 3 *primary* **Attributes**:
- **Health**
	- It's literally health
	- When this reaches zero, the current phase ends.
	- If there are no more phases, the encounter ends.
		- Typically, this means the enemy dies, or can be spared with **Mercy**.
	- [Umbra](Umbra.md) may *increase* this by *activating* a [[Dahlia]].
- **Resilience**
	- A resource that's lost instead of **Health** under certain circumstances.
	- When this reaches zero, the character is temporarily stunned by a **Stance Break**.
		- Afterwards, the *maximum* **Resilience** is reduced by a *percentage* of the *previous* maximum.
- **Energy**
	- A resource that is expended to perform special attacks, such as activating [Injectors](Injectors.md).

[Umbra](Umbra.md)'s [Hourglass](Combat.md#The%20Hourglass) heavily influences how she interacts with **Health** and **Energy**.

### Combat Actions
**Combat Actions** are the things characters can do to gain an edge in combat. All characters possess *four core* **Combat Actions** which are the primary drivers of combat interactions. 

##### Frame Windows
All **Actions** have **Frame Windows**, which are the three separate phases of an **Action**: 
- **Windup**
	- These are the frames *before* an action is happening; the frames leading into the **Action**.
- **Active**
	- These are the frames *during* an action; the frames wherein the **Action** has a certain effect.
- **Recovery**
	- These are the frames *after* an action; once these are completed, the **Action** is also considered completed.

**Frame Windows** can be **Committal**. This is a *period of vulnerability* during which *all* other **Combat Actions** are blocked.

Interrupting a non-**Committal** **Window** is known as a **Cancel**.

An **Action** may *not* perform a **Cancel** with itself; that is, a **Strike** can *not* be canceled by another successive **Strike**.

There are *at least* three different **Windows** of a **Combat Action**. Certain characters may have *unique* actions which have *additional* **Frame Windows**. They may also possess *unique traits* which allow them to *break conventions* of **Committal** actions. One such example is [Akira ~ The Demon of Hiraizumi](Akira%20~%20The%20Demon%20of%20Hiraizumi.md), whose actions are *all* **Cancelable**.

**Umbra** may obtain certain **Injectors** that affect the **Cancelability** of certain **Frame Windows**.

##### Core Actions
- **Strike**
	- A damaging attack which can be **Parried**.
	- **Committal** during:
		- **Windup** ❌
		- **Active** ✔️
		- **Recovery** ❌
- **Block**
	- A stance which prevents **Health** damage, and instead takes **Resilience** damage.
	- **Committal** during:
		- **Windup** ✔️
		- **Active** ❌
		- **Recovery** ❌
- **Dodge**
	- An evasive move with **Invulnerability** during its **Active** frames.
	- **Committal** during:
		- **Windup** ✔️
		- **Active** ✔️
		- **Recovery** ❌
- **Grab**
	- A move which temporarily **Immobilizes** another character, and has a secondary effect, such as **Damage**, **Crowd Control** or **Status**.
	- **Committal** during:
		- **Windup** ✔️
		- **Active** ✔️
		- **Recovery** ✔️

### Umbra's Attributes
**Umbra** has a few special additional **Attributes**. 

While these will be listed here, they are currently *not* very solidified, and are *highly subject to change* as we further iterate on the game. 

These **Attributes** are heavily related to [Combat Actions](Combat.md#Combat%20Actions). They may also affect specific abilities **Umbra** has.

Unless otherwise stated, these **Attributes** are *modified* via the [Circuit](Injectors.md#Circuits) system.

- **Power**
	- *Higher* values *increase* the *damage inflicted* by **Strikes**, **Grabs** and **Injectors**.
	- Higher values increase the *weight limit* of enemies which may be *pulled in* by a **Glaive Throw**.
	- It is increased by *activating* a [[Dahlia]].
- **Ghosting**
	- Higher values increase the **Active Window** of attacks which have **Invulnerability**.
- **Finesse**
	- Higher values increase the **Active Window** for the **Perfect Parry.**
	- Higher values *decrease* **Resilience** damage *taken* from **Blocked Strikes**.
- **Impact**
	- Higher values *increase* **Resilience** damage *inflicted* by a successful **Perfect Parry**.
	- Higher values increase **Resilience** damage *inflicted* when a **Strike** is **Blocked**.
- **Flow**
	- Higher values *decrease* the **Recovery Window** of **Dodge** and **Strike**.
	- Higher values *increase* the *damage inflicted* by a **Counter-Attack**.
- **Fortitude**
	- Higher values increase the **Max Resilience** that is *kept* after a **Stance Break**.
	- Higher values *decrease* **Resilience** damage *taken* from **Blocked Strikes**.
- **Resonance**
	- Higher values decrease **Energy** *costs* when using [Stigmata](Injectors.md#Stigmata).
	- Higher values *increase* **Energy** *gain* from all sources.


*Other characters* may also have unique **Attributes**.


### Glaive Throw
[[Umbra]] can throw [[Nox]] like a javelin, and it will fly in a straight line up to a maximum range, or until it hits an object or enemy. After it's attached, she may choose to **Reel** the glaive, detach it, or use it as a platform. 

**Reeling** has different effects based on the context:
- Light enemies and loose objects will be pulled towards **Umbra**, allowing her to deal some extra damage.
	- This is a long-range [[Grab]] attack.
- Heavy enemies and objects, and terrain, will *not* be pulled towards **Umbra**, but she is pulled towards them instead.
	- This is effectively a gap-closing ability.

>[!info]
The glaive will *automatically* detach if **Umbra** goes out of range or attempts to use it to attack.
This means that attacking during Glaive Throw **Cancels** the Glaive Throw **Action**.
>
>The glaive will *not* detach if **Umbra** dodges or jumps; however, **Reel** will be cancelled. 
**Reel** can be re-initiated as long as the glaive remains attached.


### Immortality
**Umbra** can *not* die; when her health is depleted, she **Reforms** at the *nearest* [[Dahlia]]. 

This is considered a **Reform Death**.

>[!info]
>Enemies that have previously fought **Umbra** *may* recognize her, and acknowledge that they've "killed" her before.


### Rewind
When **Umbra** is defeated by an enemy of [[Anomaly]] rank or higher, she cannot properly **Reform**. To combat this, she's given a [special Injector](Injectors.md#Soulbrand) by [[Akira]], which allows her to *rewind time* to one of two specific points; either the *latest phase* of the current encounter, or the *latest* **Save**.

This is considered a **Rewind Death**.

>[!info]
> - Enemies that have previously fought **Umbra** will *not* recognize her after a **Rewind**, with some very rare exceptions.
> - Cutscenes *will* trigger again *only* if **Rewinding** to a previous **Dahlia**, but *may* be skipped after first viewing.


### Amalgamate
Upon being defeated, **Umbra** *may* fuse with **Nox** in an all-or-nothing move, entering her "second phase" and regaining *half* of her maximum health, as well as enhancing all her *core* abilities. In return, for the remainder of the fight, she becomes *unable to heal*, and may *not* use any of her [Stigmata](Injectors.md#Stigmata).

Dying in this state *forcibly* **Rewinds** her to the *most recent* **Save**.

>[!info]
> - **Amalgamate** may only be activated in place of a **Rewind**; it is otherwise *not* available.
> - Any active [Circuits](Injectors.md#Circuits) will *remain* active for the duration of **Amalgamate**.

### Equinox
The **Equinox** is a type of event that is triggered by the following:
- Depletion of boss' *final* health bar
- Certain scripted sequences
- Special events

During **Equinox**, **Umbra** will briefly perceive a *diegetic* slowdown in time. At the bottom of the screen, a UI element indicating a depleting *timer* appears. An *input* action *may* be taken by the **Player** during this window.

Under normal circumstances, the following input actions are valid:
- Movement direction
- Attack
- Block
- Jump

Therefore, there will usually *not* be any input prompt on the screen during **Equinox**; however, input descriptors will appear via the [[Intuition]] system if the inputs in question have their meaning changed.

That is, if the "Attack" button becomes an option to, for example, push a rock, this *may* be indicated during an **Equinox** sequence.

This also counts for inputs which are typically *not* valid during **Equinox**, such as the input for activating the **Hourglass**.

>[!info]
> - Equinox *may* also depict *other* **Intuition** helpers, such as indicating that an attack is coming from behind.
> - Equinox does *not* require a currently active cutscene to trigger. It may trigger during cutscenes *and* regular gameplay.

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
A special type of skill reserved for those who have *deeply bonded with their weapon*. Utilizing the weapon energizes it with **Qualia**, which slightly improves its damage, windup, and recovery.

**Moxie Saturation**: The maximum potency is reached when the weapon is fully charged, further amplifying its stat increases, and granting access to **Moxie Release**. Sometimes a new passive effect is activated when **Moxie** is saturated.

**Moxie Release**: A powerful special attack which uses *no* **Energy**, but completely depletes the **Moxie** stored in the weapon. 

**Moxie** may *only* be gained by performing **Strikes** or **Perfect Parries**; **Normal Parry** and **Dodge** do *not* raise **Moxie**, and **Block** *depletes* it.


### The Hourglass
The **Hourglass** is a special kind of **Fetish** which gets absorbed by **Umbra**. 

It is *both* a **Fetish** and a **Soulbrand**.

It acts the **Health** and **Energy** management and display system, which allows **Umbra** to *swap* her **Health** and **Energy** at will.

> [!note]
**Umbra** can gather **Energy** through [Alliciency](Exploration.md#Alliciency),  by **Striking** or **Parrying** enemies.
Alternatively, she may expend **Health** with the **Hourglass** to gain more **Energy**.


### Parry
