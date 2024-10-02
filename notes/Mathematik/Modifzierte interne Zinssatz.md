Test Ist der Zinssatz einer Investition, zu dem das investierte Kapital \( K_0 \) denselben Endwert erbringt, wie die wieder verzinsten Rückflüsse. 
$$ 
i_{\text{mod}} = \sqrt[n]{\frac{E_R}{K_0}} - 1 
$$ $$ 
E_R = \bar{Z}_1 \cdot q^{n-1} + \bar{Z}_2 \cdot q^{n-2} + \ldots + \bar{Z}_{n-1} \cdot q + \bar{Z}_n 
$$ 
Die Investition ist sinnvoll, wenn 
$$
i_{\text{mod}} > i
$$
___
**Beispiel:** Eine Firma plant die Anschaffung eines neuen EDV-Systems. Die angenommene Nutzungsdauer beträgt 6 Jahre und es werden in dieser Zeit die in der Tabelle angeführten Ausgaben und erzielten Einnahmen durch dieses System vermutet. Alle Einnahmen und Ausgaben werden am Jahresende verbucht. Die Anschaffungskosten entstehen am Ende des Jahres 0.

- Berechne den internen Zinssatz dieser Investition.
- Ermittle den modifizierten internen Zinssatz dieser Investition, wenn die erwirtschafteten Rückflüsse nur zu einem Zinssatz von 3,5 % p.a. angelegt werden können.
- Überlege, wie sich der modifizierte interne Zinssatz ändert, wenn der Kalkulationszinssatz 4 % p.a. beträgt.

| Jahr | Einnahmen | Ausgaben |
| :--: | :-------: | :------: |
|  0   |     —     | 96.000 € |
|  1   | 40.000 €  | 1.000 €  |
|  2   | 45.000 €  | 1.000 €  |
|  3   | 50.000 €  | 2.000 €  |
|  4   | 40.000 €  | 4.000 €  |
|  5   | 30.000 €  | 4.000 €  |
|  6   | 20.000 €  | 4.000 €  |

Berechne den internen Zinssatz dieser Investition.
$$
-96.000 + \frac{39.000}{q} + \frac{44.000}{q^2} + \frac{48.000}{q^3} + \frac{36.000}{q^4} + \frac{26.000}{q^5} + \frac{16.000}{q^6} = 0
$$
$$ q = 1,326 \Rightarrow i = 32,6\% $$
Ermittle den modifizierten i**nternen Zinssatz dieser Investition**, wenn die erwirtschafteten Rückflüsse nur zu einem Zinssatz von **3,5 % p.a.** angelegt werden können.

$$ i_{\text{mod}} = \sqrt[n]{\frac{E_R}{K_0}} - 1 $$
$$
i = 3,5\% \Rightarrow q = 1,035
$$
$$
E_R = 39.000 \cdot q^5 + 44.000 \cdot q^4 + 48.000 \cdot q^3 + 36.000 \cdot q^2 + 26.000 \cdot q + 16.000
$$
$$
= 231503,33595
$$
$$ i_{\text{mod}} = \sqrt[6]{\frac{231503,33}{96000}} - 1 $$ $$ = 0,15802 $$ $$ \Rightarrow 15,8\% $$
**Die Investition ist sinnvoll, da 15,8% > 3,5%.**

