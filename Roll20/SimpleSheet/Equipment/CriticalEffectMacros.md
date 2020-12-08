
## DC Calculation 
The DC calculation is typically 10 + (1/2 * item level) + Ability modifier

```
Staggered DC [[10+0+@{key-ability}]]
```

This will equate to 10+(1/2*item level)+(key ability modifier).  For example:  A Level 4 Pistol would be 10+2+3 if your Dex modifier was a 3 that you used for the attack.  Other alternatives for this would be the follow attributes:

|Attribute    | Syntax      |
|-------------|-------------|
|STRENGTH:    | @{STR-mod}  |
|DEXTERITY:   | @{DEX-mod}  |
|CONSTITUTION:| @{CON-mod}  |
|INTELLIGENCE:| @{INT-mod}  |
|WISDOM:      | @{WIS-mod}  |
|CHARISMA:    | @{CHA-mod}  |
