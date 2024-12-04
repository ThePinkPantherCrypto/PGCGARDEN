---
{"dg-publish":true,"permalink":"/orderbook/"}
---

![Pasted image 20241204075211.png](/img/user/Pasted%20image%2020241204075211.png)

## DIFFERENTS TYPES D'ORDRES : 

### **Market Order (Ordre au marché)**

- **Description** : Exécute immédiatement l'ordre au meilleur prix disponible dans le carnet d'ordres.
- **Avantage** : Rapidité d'exécution.
- **Inconvénient** : Le prix d'exécution est incertain, surtout sur des marchés peu liquides.
- **Exemple** : "Acheter 1 BTC au prix du marché."



---
### **Limit Order (Ordre limite)**

- **Description** : Exécute l'ordre uniquement si le prix atteint ou dépasse un seuil fixé par le trader.
- **Avantage** : Contrôle du prix maximum (pour un achat) ou minimum (pour une vente).
- **Inconvénient** : L'ordre peut ne pas être exécuté si le prix limite n'est pas atteint.
- **Exemple** : "Acheter 1 BTC si le prix tombe à 20 000 $ ou moins."
---
### **Stop Order (Ordre stop)**

- **Description** : L'ordre devient un ordre au marché lorsque le prix atteint un seuil prédéfini (prix stop).
- **Avantage** : Automatisation pour entrer ou sortir d'une position une fois un niveau atteint.
- **Inconvénient** : Le prix final peut varier en cas de forte volatilité.
---
### **Stop-Limit Order (Ordre stop-limite)**

- **Description** : Combinaison d'un ordre stop et d'un ordre limite. L'ordre est déclenché à un prix stop, mais ne sera exécuté que si un prix limite est respecté.
- **Avantage** : Plus de contrôle sur le prix d'exécution qu'avec un simple stop.
- **Inconvénient** : L'ordre peut ne pas s'exécuter si le prix limite n'est pas atteint.
- **Exemple** : "Vendre 1 BTC si le prix tombe à 18 000 $, mais pas en dessous de 17 500 $."

**Explication :** Cela te permets de placer un ordre à un certains montant quand l'actif passe un certains montant, typiquement tu fais de l'analyse technique tu déscele une  résistance a 58k si elle est cassé la prochaine est a 55k alors tu mets un ordre stop-limit qui ce déclenche à 58k et qui va acheter a 55k, en gros quand on atteind 58k tu fill un ordre sur l'orderbook pour 55k. 



- ---

### **Trailing Stop Order (Ordre stop suiveur)**

- **Description** : Un ordre stop ajusté dynamiquement en fonction de l'évolution du prix.
- **Avantage** : Protège les gains en laissant une marge pour suivre les tendances du marché.
- **Inconvénient** : Peut être déclenché par des fluctuations à court terme.
- **Exemple** : "Vendre 1 BTC si le prix descend de 5 % par rapport à son sommet récent."
