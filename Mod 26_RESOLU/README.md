# Mod 26

## 0x1 Description

>Cryptography can be easy, do you know what ROT13 is? cvpbPGS{arkg_gvzr_V'yy_gel_2_ebhaqf_bs_ebg13_MAZyqFQj}

## 0x2 Résolution

Tout est dans la description, c'est une simple substitution de CAESAR, avec le paquet bsdgames et l'outil ROT13, la solution est automatique

```bash
echo "cvpbPGS{arkg_gvzr_V'yy_gel_2_ebhaqf_bs_ebg13_MAZyqFQj}" | rot13
```

>picoCTF{next_time_I'll_try_2_rounds_of_rot13_ZNMldSDw}

## 0x3 Bonus

Pour les utilisateurs de VIM, la solution peut être trouvée avec la commande suivante:

Pour la ligne complète:

>g??

Pour une selection visuelle:

>[selection visuel]g?
