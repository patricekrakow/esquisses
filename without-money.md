# Without Money

## Basics

_Agent-A_ sells a good-U to _agent-B_ for u EUR;

_Agent-B_ pays _agent-A_ by owing u EUR (due to _agent-A_);

_Agent-B_ has a **debt of u EUR** due to _agent-A_.

Then

_Agent-C_ sells a good-V to _agent-A_ for v EUR;

**If v = u**

_Agent-A_ pays _agent-C_ by transferring the _agent-B_ **debt of u EUR**;

_Agent-B_ has a **debt of u EUR** due to _agent-C_;

_Agent-A_ does not have any debt due to _agent-C_.

**If v > u**

_Agent-A_ partly pays _agent-C_ by transferring the _agent-B_ **debt of u EUR**, and by owing v-u EUR (due to _agent-C_);

_Agent-B_ has a **debt of u EUR** due to _agent-C_;

_Agent-A_ has a **debt of v-u EUR** due to _agent-C_.

**If v < u**

_Agent-A_ splits the _agent-B_ debt of u EUR into 2 debts: one **debt of v EUR** and another **debt of u-v EUR**;

_Agent-A_ pays _agent-C_ by transferring the agent-B **debt of v EUR**;

_Agent-B_ has a **debt of v** EUR due to _agent-C_;

_Agent-B_ has a **debt of u-v** EUR due to _agent-A_;

_Agent-A_ does not have any debt due to _agent-C_.

## The Automatic Clearing of Debt Loops

_Alice_ sells a good/service to _Barry_ for 100 EUR;

_Barry_ pays _Alice_ by owing 100 EUR (due to _Alice_);

_Barry_ has a **debt of 100 EUR** due to _Alice_.

Then

_Calum_ sells a good/service to _Alice_ for 100 EUR;

_Alice_ pays _Calum_ by owing 100 EUR (due to _Calum_);

_Alice_ has a **debt of 100 EUR** due to _Calum_.

Then

_Barry_ sells a good/service to _Calum_ for 100 EUR;

_Calum_ pays _Barry_ by owing 100 EUR (due to _Barry_);

_Calum_ has a **debt of 100 EUR** due to _Barry_.

Then

the system finds out that there is a _loop_:
- _Barry_ has a **debt of 100 EUR** due to _Alice_;
- _Alice_ has a **debt of 100 EUR** due to _Calum_;
- _Calum_ has a **debt of 100 EUR** due to _Barry_;

and therefore **the system can simply clear the three debts**. You can see it as if the system would borrow 100 EUR to _Barry_, so _Barry_ can give these 100 EUR to Alice to pay his debt, then _Alice_ can give these 100 EUR to Calum to pay her bebt, then _Calum_ can give these 100 EUR to _Barry_ to pay his debt, and finally _Barry_ can give the 100 EUR back to the system!
