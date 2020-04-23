# Perception for a token

rolls perception and also show passive perception

```
/w gm &{template:atk} {{rname=Perception}} {{mod=@{target|pc|perception_bonus}}} {{r1=[[1d20 + @{target|pc|perception_bonus}]]}} {{always=1}} {{r2=[[1d20 + @{target|pc|perception_bonus}]]}} {{charname=@{target|pc|character_name}}} {{range=}} {{desc=Passive perception [[10 + @{target|pc|perception_bonus}]]}} {{spelllevel=}} ammo=
```

