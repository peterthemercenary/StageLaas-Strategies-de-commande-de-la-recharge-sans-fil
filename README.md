# StageLaas – Stratégies de commande de la recharge sans fil ⚡🔋

## Description
Ce projet explore différentes stratégies de commande pour la recharge sans fil à l’aide de microcontrôleurs STM32.

## Implémentations de la commande 

- **Microcontrôleur STM32L476RG** (TIMER normal)  
  → Fichier : `CommandeDuPontComplet` pour la commande du pont complet ( un timer de base , un timer en retard par rapport au timer de base et l'autre en avance )<br>
  → Fichier : `PWMFREQL476RG` pour moduler la fréquence des signaux PWM à déphaser afin de contrôler le courant ( à moitié fonctionnel à cause d'un petit
               problème d'implémentation : le déphasage ne se met pas à jour périodiquement)

- **Microcontrôleur STM32G474RE** (High Resolution TIMER)  
  → Fichier : `TestHRTIM1` (avec test du DAC) pour la commande du pont complet avec des HRTIMs ( des PWM déphasés et/ou inversés)


✍️ Auteur :       
&nbsp;&nbsp;Pierre Diamane SENGHOR<br> 
&nbsp;&nbsp;Hassan SARIH <br>
📅 Projet réalisé dans le cadre d’un stage au **LAAS-CNRS**
