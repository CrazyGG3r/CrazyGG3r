# If I could go back in time

### I would be stuck forever trying to fix everything i did
<br>
<br>

```python
def travel_back(year,current_mistakes):
  re_actions = {}
  for a in current_mistakes:
      new_Action = Correction_model.predict(a)
      if Consequences.predict(new_Action) == "Good to go":
          re_actions[current_mistakes] = new_Action
      else:
          date,new_mistakes = Consequences.build(new_Action)
          travel_back(date,new_mistakes)
  return re_actions

current_mistakes = ["writing this readme instead of progressing my fyp",]
date = "18-11-2024"
travel_back(date,current_mistakes)
```

<br>
<br>
so i will just drop my younger self from a height of 25 feet for being retarded asf
