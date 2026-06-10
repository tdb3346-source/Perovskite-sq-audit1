: What did you audit, against what, and why single-junction only?

A: I audited 8 single-junction perovskite solar cells from SCAPS-1D simulation papers against the Shockley-Queisser (SQ) radiative ceiling computed by my calculator, focusing strictly on single-junction cells so they all share the same baseline thermodynamic ceiling.

: For each paper, what two numbers did you extract and how did you decide PASS vs FLAG?

A: I extracted the claimed efficiency and the absorber bandgap, triggering a FLAG if the claimed efficiency exceeded the SQ ceiling at that specific gap. I used a strict absorber-identification rule to focus on the primary light-absorbing layer, keeping me from pulling the wrong bandgap from the charge transport layers.

: How many FLAGed, which ones, and what does a FLAG physically mean?

A: 2 out of the 8 papers FLAGed: MASnI3 (claiming 33.46% at 1.3 eV) and KSnI3 (claiming 30.21% at 1.84 eV). A FLAG means the claimed efficiency exceeds the absolute thermodynamic limit by assuming zero non-radiative loss, which is physically impossible; the contrast shows that responsible, multi-material studies (like PMC12409573) strictly respect wide-gap ceilings, while hype-optimization papers blow right past them.

: What happened with MASnI₃ — how did you first call it, what did the tool say, and why does that gap matter?

A: I originally eyeballed the ceiling at ~33.5% and called it a PASS by a tiny 0.05% margin. However, because a 1.3 eV bandgap sits just to the left of the peak SQ efficiency (1.34 eV), the tool computed the actual ceiling at 33.1%, flipping the result to a FLAG. The tool caught a thermodynamic violation the human eye completely missed.

 What can this audit NOT conclude?

A: It cannot conclude that a PASS is actually achievable in a lab, only that it is "not impossible." It also takes each paper's bandgap as absolute truth (meaning it cannot verify if a claimed gap like a hydrogenated 1.61 eV is real), and it does not model real-world non-radiative losses.