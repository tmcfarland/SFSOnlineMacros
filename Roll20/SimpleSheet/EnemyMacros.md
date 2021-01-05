
## Roll for Initiative
Option to hide the roll:
```
%{selected|NPC-Initiative-Roll}
```
Roll without asking to hide
```

```
## Saves

```
&{template:pf_check}{{name=@{Selected|character_name} Saves}}{{check=[[1d20+@{Fort-npc}]] Fort [[1d20+@{Ref-npc}]] Ref [[1d20+@{Will-npc}]] Will }}
```

## Attack Rolls
Replace the $0 with the position of the weapon you want to use.  This is a zero based array (first item is $0, second is $1, etc)
```
%{selected|repeating_npc-weapon_$0_roll}
```
