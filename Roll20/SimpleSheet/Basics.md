
##Movement
When calculating movement with the range tool, if you hit the `q` key it will allow you to make a 'waypoint' and calculate movement correctly.

##Initiative
Ensure that your token is selected and this will roll your initiative and add it automatically to the initiative track
```
%{selected|Roll-for-initiative}
```

##Skill Checks

Token macro for drop down of skills
```
&{template:pf_check} {{name=@{selected|character_name}}} {{check=Skill Check}} {{foo= ?{Choose a Skill(† trained only)| Acrobatics, Acrobatics: [[ 1d20 + [[ @{selected|Acrobatics} ]] + ?{Modifier?&#124;0&#125; ]] | Athletics, Athletics: [[ 1d20 + [[ @{selected|Athletics} ]] + ?{Modifier?&#124;0&#125; ]] | Bluff, Bluff: [[ 1d20 + [[ @{selected|Bluff} ]] + ?{Modifier?&#124;0&#125; ]] | †Computers, Computers: [[ 1d20 + [[ @{selected|Computers} ]] + ?{Modifier?&#124;0&#125; ]] | †Culture, Culture: [[1d20 + [[@{selected|Culture} ]] + ?{Modifier?&#124;0&#125; ]] | Diplomacy, Diplomacy: [[ 1d20 + [[ @{selected|Diplomacy} ]] + ?{Modifier?&#124;0&#125; ]] | Disguise, Disguise: [[ 1d20 + [[ @{selected|Disguise} ]] + ?{Modifier?&#124;0&#125; ]] | †Engineering, Engineering: [[ 1d20 + [[ @{selected|Engineering} ]] + ?{Modifier?&#124;0&#125; ]] | Intimidate, Intimidate: [[ 1d20 + [[ @{selected|Intimidate} ]] + ?{Modifier?&#124;0&#125; ]] | †Life Science, Life Science: [[ 1d20+ [[ @{selected|Life-Science} ]] + ?{Modifier?&#124;0&#125; ]] | †Medicine, Medicine: [[ 1d20 + [[ @{selected|Medicine} ]] + ?{Modifier?&#124;0&#125; ]] | †Mysticism, Mysticism: [[ 1d20 + [[ @{selected|Mysticism} ]] + ?{Modifier?&#124;0&#125; ]] | Perception, Perception: [[ 1d20 + [[ @{selected|Perception} ]] + ?{Modifier?&#124;0&#125; ]] | †Physical Science, Physical Science: [[ 1d20+ [[ @{selected|Physical-Science} ]] + ?{Modifier?&#124;0&#125; ]] | Piloting, Piloting: [[1d20 + [[ @{selected|Piloting} ]] + ?{Modifier?&#124;0&#125; ]] | †Profession, Profession (@{selected|Profession-name}): [[ 1d20 + [[ @{selected|Profession} ]] + ?{Modifier?&#124;0&#125; ]] | †Profession 2, Profession (@{selected|Profession2-name}): [[ 1d20 + [[ @{selected|Profession2} ]] + ?{Modifier?&#124;0&#125; ]] | Sense Motive, Sense Motive: [[ 1d20 + [[ @{selected|Sense-Motive} ]] + ?{Modifier?&#124;0&#125; ]] | †Sleight of Hand, Sleight of Hand: [[ 1d20 + [[ @{selected|Sleight-of-Hand} ]] + ?{Modifier?&#124;0&#125; ]] | Stealth, Stealth = [[ 1d20 + [[ @{selected|Stealth} ]] + ?{Modifier?&#124;0&#125; ]] | Survival, Survival: [[ 1d20 + [[ @{selected|Survival} ]] + ?{Modifier?&#124;0&#125; ]]}}}
```

The following will be used to roll 
```
[[1d20 + [[@{select|SkillName}]] + ?{Modifier?&#124;0&#125;]]
```

##Saves
Token macro for rolling all saves:
```
&{template:pf_check}{{name=Saves}}{{check=[[1d20+@{Fort}]] Fort [[1d20+@{Ref}]] Ref [[1d20+@{Will}]] Will }} {{foo=@{save-notes}}}
```
