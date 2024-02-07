---
aliases:
  - capacitors
---
> [!info] Capacitors store charge. They are usually built using two plates that aren't touching. The [[capacitance]] of a capacitor tells you how good it is at storing charge.

When you hook up a capacitor to a battery, the negative terminal of the battery repels electrons onto one plate, while the positive terminal attracts electrons, leaving one plate negatively charged and one plate positively charged with equal charge. At some point, the electrons will be pulled by the positive side of the capacitor as much as the positive terminal of the battery, and the capacitor will be fully charged, with the same [[voltage]] as the battery.

The type of [[energy]] stored in [[capacitor|capacitors]] is electrical [[potential energy]]. This is equal to half the charge of the plates times voltage.
$$
E=\frac{1}{2}QV
$$
$$
E=\frac{1}{2}CV^2
$$
(derived from formula for [[capacitance]])
> [!warning] The reason why energy is not just charge times voltage is because as discharge occurs, voltage drops.

Inserting a non-conducting [[material]] between plates will always increase capacitance. This non-conducting [[material]] is known as a [[dielectric]]. The negatives in the [[dielectric]] will shift towards the positive plate of the capacitor, the the positives in the dielectric will shift towards the negative plate. If no battery is connected this decreases [[voltage]] because the charges in the [[dielectric]] will cancel out some of the charge of the plates. Lower [[voltage]] at the same charge means more [[capacitance]]. Or, if a battery is connected and trying to maintain constant voltage, you end up with more charges necessary to keep that same voltage, and $C$ increases.
### Series
Capacitors in series all have the same charge because the charges a capacitor gains or loses are from the capacitor in front of behind. 
The sum of [[voltage]] across capacitors in series is basically equal to the total [[voltage]] of the circuit for a circuit. We know from the formula for [[capacitance]] that $V=\frac{Q}{C}$ Thus, $V_{total}=\frac{Q}{C_{1}}+\frac{Q}{C_{2}}\dots$ Factor out the Q, divide both sides by q, and you get
$$
\frac{1}{C_{eq}}=\frac{1}{C_1}+\frac{1}{C_{2}}+\frac{1}{C_{3}}+\dots
$$
### Parallel
In parallel, each capacitor is essentially hooked up directly to the battery. Thus the [[voltage]] of each capacitor is equal to the voltage of the battery. Because you are essentially building one big capacitor with smaller capacitors,
$$
C_{eq}=C_{1}+C_{2}+C_{3}+\dots
$$
