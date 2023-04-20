"# Knowledge-based-Systems" 

Monkey And Banana

Goal State {
Happy(monkey),
isOn(Chair, Desk),
isOn(Desk, floor),
Eat(Monkey, Banana),
isOn(Monkey, Chair)}

Production Rules

If isOn(C, F) & isOn(D, F)
Then isOn(C, F) -> isOn(C,D)
If isOn(M,F) & isOn(C,F)
Then isOn(M,F) -> isOn(M,C)
If isOn(M,F) & isOn(D,F)
Then isOn(M,F) -> isOn(M,D)
If isOn(M,D) & isOn(C,D)
Then isOn(M,D) -> isOn(M,C)
If isOn(M,C) & isOn(C,D)
Then isOn(B,€) -> Eat(M,B)
If Eat(M,B)
Then Hungry(M) -> Happy(M)