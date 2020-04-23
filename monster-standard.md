# For a monster sheet

## run actions such as attacks

```
%{selected|repeating_npcaction_$0_npc_action}
```

## Traits

```
/w gm &{template:npcaction} {{name=@{selected|npc_name}}} {{rname=@{selected|repeating_npctrait_$0_name}}} {{description=@{selected|repeating_npctrait_$0_desc}}}
/w gm &{template:npcaction} {{name=@{selected|npc_name}}} {{rname=Reaction: @{selected|repeating_npcreaction_$0_name}}} {{description=@{selected|repeating_npcreaction_$0_desc}}}
```

## Initiative

```
/w gm &{template:default} {{name=Initiative}}{{Initiative=[[1d20+@{dexterity_mod}]]}}
```

## Saves

```
/w gm &{template:default} {{name=Saving Throws}} {{Str Save= [[1d20+@{strength_save_bonus}]] | [[1d20+@{strength_save_bonus}]]}} {{Dex Save= [[1d20+@{dexterity_save_bonus}]] | [[1d20+@{dexterity_save_bonus}]]}} {{Con Save= [[1d20+@{constitution_save_bonus}]] | [[1d20+@{constitution_save_bonus}]]}} {{Int Save= [[1d20+@{intelligence_save_bonus}]] | [[1d20+@{intelligence_save_bonus}]]}} {{Wis Save= [[1d20+@{wisdom_save_bonus}]] | [[1d20+@{wisdom_save_bonus}]]}} {{Cha Save= [[1d20+@{charisma_save_bonus}]] | [[1d20+@{charisma_save_bonus}]]}}
```

## Perception

```
%{Selected|npc_perception}
@{selected|wtype}&{template:npc} {{normal=1}} {{name=@{selected|npc_name}}} {{rname=Passive Perception}} {{mod=}} {{r1=[[@{selected|npc_perception}+10]]}}
```

## Stats

```
/w gm &{template:default} {{name=Stats}} {{Armor Class= @{selected|npc_AC} @{selected|npc_actype}}} {{Hit Dice= @{selected|npc_hpformula} | [[@{selected|npc_hpformula}]]}} {{Speed= @{selected|npc_speed}}} {{Senses=@{selected|npc_senses}}}
```
