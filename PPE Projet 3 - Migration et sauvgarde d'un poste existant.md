---
title: PPE Projet 3 - Migration et sauvgarde d'un poste existant

---

**Projet 3 - Migration et sauvegarde d'un poste existant**

***1. Faire l'inventaire des données à conserver (documents, favoris navigateur, paramètres réseau, logiciels installés***

'Faire l'inventaire' = 'Faire une liste de sauvegarde'

**1. Documents**

- Ouvrir 'Eplorateur de fichiers'

- Aller dans 'Bureau', 'Téléchargement', 'Documents', 'Images', 'Musique', 'Vidéos'

![2026-09-17_11h05_02](https://hackmd.io/_uploads/rJUcCQKtGe.png)

- Noter les fichier importants à conserver

- (Aucun fichier dans ma VM)

**2. Favoris du navigateur**

- Ouvrir 'Google chrome', ouvrir les favoris et vérifier quels fichiers sont importants

![2026-09-17_11h18_59](https://hackmd.io/_uploads/ry2vWNYKzl.png)

**3. Paramètres réseau**

- Cliquer dans le menu 'Démarrer' ---> 'Paramètres' ---> 'Réseaux et Internet'

- Noter ces différents points:

1. Adresse IPv4 = 192.168.29.2
2. Passerelle par défaut IPv4 = 192.168.29.2
3. Serveurs DNS IPv4 = 192.168.29.2
4. Nom de la machine = 'Windows 11 x64 v2'
5. Connexion utilisée (Wifi/Ethernet) = Réseau public

![2026-09-17_11h37_36](https://hackmd.io/_uploads/ryktSVKYMg.png)

![2026-09-17_11h38_50](https://hackmd.io/_uploads/BySFBNFFfe.png)

**4. Logiciels installés**

- Cliquer sur le menu 'Démarrer' ---> 'Paramètres' ---> 'Applications' ---> 'Applications installées'

![2026-09-17_11h41_29](https://hackmd.io/_uploads/ByJAIVFFGx.png)


- Noter les logiciels importants qu'il faudra réinstaller

1. Google chrome
2. Microsoft 365
3. Teams
4. Outlook

***2. Sauvegarder ces données sur un support externe ou un espace réseau (clé USB, disque externe, ou partage réseau)***

- Brancher la clé USB sur le PC réel

![2026-09-17_13h23_07](https://hackmd.io/_uploads/r1g3TBttfx.png)

- Redémarrer la VM Windows 11 en cliquant sur 'Power on this virtual machine' pour que la VM reconnaisse la clé USB

![2026-09-17_13h24_45](https://hackmd.io/_uploads/HJl70HKtfe.png)

- Une fois la VM redémarrer, en haut, cliquer sur 'VM' ---> 'Removable Device'

- Chercher la clé USB

- Cliquer sur '(Disconnect from Host)', la clé sera alors déconnectée du PC réel et connecter à la VM

- Dans la VM, ouvrir 'Explorateur de fichiers' ---> 'Ce PC', créer un dossier 'Sauvegarde' dans l'emplacement de la clé usb, et copier les documents, fichiers importants

![2026-09-17_13h47_42](https://hackmd.io/_uploads/ByU-48KtGg.png)

![2026-09-17_13h48_24](https://hackmd.io/_uploads/SkqbN8YFMl.png)

![2026-09-17_13h48_41](https://hackmd.io/_uploads/HJCbNUKYGx.png)

- Dans 'Explorateur de fichiers' regarder dans les fichiers ce qui est important, sélectionner, copier, coller dans le dossier sauvegarde

![2026-09-17_14h02_38](https://hackmd.io/_uploads/SylfPUKYGe.png)

![2026-09-17_14h03_04](https://hackmd.io/_uploads/SJLfwUYFfe.png)

- Dans 'Google chrome', appuyer sur 'trois points' ---> 'Favoris et listes' ---> 'Gestionnaire de favoris'

- Ensuite, 'trois points' ---> 'Exporter les favoris' et enregostrer dans le dossier 'Sauvegarde'

![2026-09-17_14h08_11](https://hackmd.io/_uploads/Bk8_j8YtMl.png)

![2026-09-17_14h10_23](https://hackmd.io/_uploads/Sy6_oLttfe.png)

![2026-09-17_14h11_39](https://hackmd.io/_uploads/ByJhs8KYfg.png)

- Sauvegarder les informations réseau dans le dossier 'Sauvegarde' 

- 'Clic droit' ---> 'Nouveau' ---> 'Document texte', renomer le document et écrire les informations du réseau

![2026-09-17_14h14_46](https://hackmd.io/_uploads/ByLm2UKtGl.png)

![2026-09-17_14h16_58](https://hackmd.io/_uploads/ryvj3UtFGg.png)

![2026-09-17_14h20_39](https://hackmd.io/_uploads/ry-anUKKzx.png)

- Créer un nouveau 'Document texte' pour noter tout les logiciels important à installer

![2026-09-17_14h31_55](https://hackmd.io/_uploads/BJhCT8YKfg.png)

- À la fin remettre la clé USB sur le PC Réel: 'VM' ---> 'Removable Devices' ---> 'Clé USB' ---> 'Disconnect (connect from Host)'

***3. Vérifier l'intégralité de la sauvegarde ( comparaison de tailles/nombres de fichiers )***

- Dans la VM, dans le dossier d'origine, faire 'Clic droit' ---> 'Propriétés' et comparer les valeurs entre le dossier d'origine et le dossier 'Sauvgarde' USB

![2026-09-17_14h38_50](https://hackmd.io/_uploads/r1fakvtYGe.png)

![2026-09-17_14h39_45](https://hackmd.io/_uploads/H1H6JvKKfx.png)

***4. Réinstaller proprement le système d'exploitation (formatage complet)***

- Cliquer sur 'Create a new Virtual machine' pour créer une nouvelle machine virtuel

![2026-09-17_14h57_52](https://hackmd.io/_uploads/HJW4EDFYGe.png)

- Sélectionner 'Typical' puis cliquer sur 'Next'

![2026-09-17_15h00_03](https://hackmd.io/_uploads/H1xDNPKYMl.png)

- Sélectionner 'Installer disc image file (iso)', cliquer sur 'Browser', double clic sur le fichier iso et cliquer sur 'Next'

![2026-09-17_15h01_56](https://hackmd.io/_uploads/SJPA4DtYfl.png)

- Sélectionner 'Microsoft Windows', la bonne version de Windows et cliquer sur 'Next'

![2026-09-17_15h03_05](https://hackmd.io/_uploads/ByvzrPKtzg.png)

- Nommer la machine virtuel, cliquer sur 'Browser' et créer un dossier pour pouvoir retrouver la VM dans 'Explorateur de fichiers'

![2026-09-17_15h07_43](https://hackmd.io/_uploads/Hk8w8wtYMg.png)

- Créer et confirmer un mot de passe et cliquer sur 'Next'

![2026-09-17_15h09_56](https://hackmd.io/_uploads/H1W3IDYFMx.png)

- Choisir la taille du 'Disk', sélectionner 'Split virtual disk into multiple files' et cliquer sur 'Next'

![2026-09-17_15h11_30](https://hackmd.io/_uploads/BJkMDvFKzx.png)

- Paramètrer la 'Mémoire', les 'Processeurs' et le 'Network Adapter' et cliquer sur 'Close' puis sur 'Finish'

![2026-09-17_15h15_16](https://hackmd.io/_uploads/ByfxdPtYzx.png)

![2026-09-17_15h13_19](https://hackmd.io/_uploads/HkEx_DtYzl.png)

![2026-09-17_15h13_28](https://hackmd.io/_uploads/Byvx_PFtGg.png)

![2026-09-17_15h16_25](https://hackmd.io/_uploads/HJ8EOPYYfx.png)

- Lancer la VM en cliquant sur 'Power on this virtual machine'

![2026-09-17_15h18_48](https://hackmd.io/_uploads/ByET_PFtGe.png)

- Choisir les bons paramètre de langue et cliquer sur suivant

![2026-09-17_15h20_51](https://hackmd.io/_uploads/ByAAYPKtze.png)

- Sélectionner les bon paramètres clavier et cliquer sur suivant

![2026-09-17_15h21_15](https://hackmd.io/_uploads/S1GfcDKFMl.png)

- Sélectionner 'Installer Windows 11' cliquer sur le petit carré et cliquer sur suivant

![2026-09-17_15h21_27](https://hackmd.io/_uploads/ByL_cDFKfx.png)

- Cliquer sur 'Je n'ai pas de clé de produit'

![2026-09-17_15h21_42](https://hackmd.io/_uploads/S1ocqvttGe.png)

- Sélectionner la bonne image et cliquer sur 'Suivant'

![2026-09-17_15h22_09](https://hackmd.io/_uploads/HJVzivFtfx.png)

- Accepter le contrat de licence

![2026-09-17_15h22_24](https://hackmd.io/_uploads/SJ07swYYzl.png)

- Sélectionner l'emplacement d'installation et cliquer sur 'Suivant'

![2026-09-17_15h22_57](https://hackmd.io/_uploads/Bkx8ivYKfe.png)

- Cliquer sur 'Installer'

![2026-09-17_15h23_12](https://hackmd.io/_uploads/rJP8oPtKfg.png)

- Choisir le bon pays

![2026-09-17_15h41_58](https://hackmd.io/_uploads/SJlr0vtKGe.png)

- Choisir la bonne disposition de clavier

![2026-09-17_15h42_57](https://hackmd.io/_uploads/HJZFCvtYMg.png)

- Nommer l'appareil

![2026-09-17_15h48_01](https://hackmd.io/_uploads/HJki1OYYGx.png)

- Sélectionner la configuration adéquate

![2026-09-17_15h51_15](https://hackmd.io/_uploads/HylOldKYMg.png)

- Créer un mot de passe et le confirmer

![2026-09-18_08h54_26](https://hackmd.io/_uploads/BySQWw9Fzg.png)

- Choisir 3 questions et répondre 3 fois la même chose

![2026-09-18_08h55_25](https://hackmd.io/_uploads/rJ1c-D9Yzx.png)

- Pour chaque choix, choisir le deuxième choix

![2026-09-18_08h57_11](https://hackmd.io/_uploads/HynxMwctMl.png)

![2026-09-18_08h57_30](https://hackmd.io/_uploads/SkJWGvqFMg.png)

![2026-09-18_08h57_41](https://hackmd.io/_uploads/rkEfMv5KMg.png)

![2026-09-18_08h57_53](https://hackmd.io/_uploads/BJvzfD5Kfg.png)

![2026-09-18_08h58_03](https://hackmd.io/_uploads/BycMMwqKGl.png)

![2026-09-18_08h58_14](https://hackmd.io/_uploads/S1BNGP9tMl.png)

- Après ça windows est installé

***5. Réinstaller les logiciels nécessaires identifiés lors de l'inventaire***

- En haut à gauche, sélectionner 'VM' ---> 'Removable Devices' ---> 'Clé USB' ---> 'Connect (Disconnect from Host)'

- Cliquer sur 'Explorateur de fichiers' ---> 'Clé USB' ---> 'Dossier Sauvegarde' ---> 'Installer chrome'

![2026-09-18_09h51_57](https://hackmd.io/_uploads/H12oTP9tfe.png)

![2026-09-18_09h52_35](https://hackmd.io/_uploads/HJBJCDqYMl.png)

![2026-09-18_09h55_40](https://hackmd.io/_uploads/rkr50DcKfe.png)

- Dans le document texte 'Installation logiciel', installer les applications écrites

![2026-09-18_10h16_29](https://hackmd.io/_uploads/BJ1MH_9Ffg.png)

Cliquer sur 'Rechercher' dans la barre des tâches, écrire une application à installer, dans le cas de la photo 'Microsoft 365' et cliquer en haut à gauche

![2026-09-18_10h16_55](https://hackmd.io/_uploads/B1bnSu9FGx.png)

- Sur cette page cliquer sur 'Télécharger' 

![2026-09-18_10h17_28](https://hackmd.io/_uploads/rJlEIO5Yfg.png)

- Cliquer sur le fichier en haut à droite et mettre à jour

![2026-09-18_10h17_49](https://hackmd.io/_uploads/BkfuL_qYfg.png)

- Il suffit de faire pareil pour les autres applications


***6. Restaurer les données sauvegardées et vérifier leur intégralité après restauration***

- 


***7. Reconfigurer les paramètres essentiels***

- Sur la clé USB, ouvrir le document texte 'Information réseau'

![2026-09-18_10h34_21](https://hackmd.io/_uploads/BJKcPucYMx.png)

- Cliquer sur 'Démarrer' ---> 'Paramètres' ---> 'Réseau et Internet' ---> 'Ethernet' ---> 'Attribution IP' ---> 'Modifier' ---> 'Manuel'

![2026-09-18_10h36_42](https://hackmd.io/_uploads/BkYQuuqKGg.png)

![2026-09-18_10h37_28](https://hackmd.io/_uploads/HkBIOuqKfe.png)









