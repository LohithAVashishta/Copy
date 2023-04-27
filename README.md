
=IFERROR(If(B5="Yes",A31,IF(AND($C$7<=1.2,$C$8>15),"As per Ref. TN X53RP1808817 Issue 2.0 page 73, Dents fulfilling form and nearness criteria up to 2.0mm deep have a negligible effect on static behavior (Stability and strength). Thus the dent is acceptable from a static perspective as the dent depth ("&$C$7&"mm) is less than 2.0mm as allowed per TN X53RP1808817 Issue 2.0 (Generic ADL: Dent #1 justification). Hence above mentioned ADL covers the reported dent without further calculations",IF(AND($C$7>1.2,$C$7<=2,$C$8>15),"As per Ref. TN X53RP1808817 Issue 2.0 page 73, Dents fulfilling form and nearness criteria up to 2.0mm deep have a negligible effect on static behavior (Stability and strength). Thus the dent is acceptable from a static perspective as the dent depth ("&$C$7&"mm) is less than 2.0mm as allowed per TN X53RP1808817 Issue 2.0 (Generic ADL: Dent #1 justification). Hence above mentioned ADL covers the reported dent without further calculations",IF(AND($C$7<=0.5,$C$8<=15),"As per Ref. TN X53RP1906976 Issue 1.0 page 47, “Dents below stiffening elements up to 0.5mm deep have a negligible effect on static behavior (Stability and strength)”. Thus the dent is acceptable from a static perspective as the dent depth ("&$C$7&"mm) is less than 0.5mm as allowed per TN X53RP1906976 Issue 1.0 (Generic ADL: Dent #2 justification). Hence above mentioned ADL covers the reported dent without further calculations.",If($B$6="Longitudinal","Conservatively, the dent is considered as a hole. The overstress coefficient calculation is performed in the longitudinal direction. Plate size is considered as the distance between frames, "&$B$16&" & "&$B$17&" = "&$C$17&"-"&$C$16&" = "&$C$18&"mm

Overstress coefficient = "&$C$18&" / ("&$C$18&"-"&MAX($C$9:$C$10)&") = "&Round($C$20,2)&"
(Max. dimension of the dent is considered for calculation)

Factored stress to be considered for skin is, σfactored = "&Round($C$15,2)&" X "&Round($C$20,2)&" = "&Round($C$21,2)&"MPa
RF = "&$C$19&" / "&Round($C$21,2)&" = " &IF($C$22>1,If($C$22="HIGH (>2)",$C$22,Round($C$22,2)),Round($C$22,2)&""),if($B$6="Circumferential/User Defined Plate width","Conservatively, the dent is considered as a hole. The overstress coefficient calculation is performed and plate size is considered as the distance = "&$C$11&"mm

Overstress coefficient = "&$C$11&" / ("&$C$11&"-"&MAX($C$9:$C$10)&") = "&Round($C$20,2)&"
(Max. dimension of the dent is considered for calculation)

Factored stress to be considered for skin is, σfactored = "&Round($C$15,2)&" X "&Round($C$20,2)&" = "&Round($C$21,2)&"MPa
RF = "&$C$19&" / "&Round($C$21,2)&" = " &IF($C$22>1,If($C$22="HIGH (>2)",$C$22,Round($C$22,2)),Round($C$22,2)&""))))))),"ERORR, PLEASE CHECK INPUT VALUES")
