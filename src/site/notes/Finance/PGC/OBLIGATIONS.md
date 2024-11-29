---
{"dg-publish":true,"permalink":"/finance/pgc/obligations/"}
---

### Essentiel  :https://www.buyupside.com/calculators/bondconvexity.htm

### Calcul du prix d'une obligation avec calculette financière (Present value):

![Pasted image 20240816203401.png](/img/user/Data/Pasted%20image%2020240816203401.png)

Ce calcul ce fait avec le Yield to Maturity , comment le trouver et le calculer ? 

### Yield to Maturity : 

Le **yield to maturity (YTM)** diffère souvent du taux de coupon de l'obligation, appelé aussi le **taux nominal** ou **taux d'intérêt annuel** (parfois noté **i/y**), parce que le prix auquel l'obligation est achetée sur le marché peut être différent de sa valeur nominale. On la paye avec un **premium** ou un **discount**

Le **yield to maturity (YTM)** prend en compte non seulement les paiements de coupons, mais aussi la différence entre le prix d'achat de l'obligation et sa valeur nominale à l'échéance.


**Calcul avec une calculatrice financière** : On entre le prix d'achat de l'obligation, les paiements de coupons, la valeur nominale, et l'échéance. La calculatrice trouve ensuite le YTM en résolvant l'équation qui équilibre le prix de l'obligation avec la somme des flux actualisés par ce taux unique.

**Present value inconnu** : A ce moment on utilise les **spot rates**


### Calcul de la Present value avec spot rates pour trouver le YTM 

On va avoir besoin des **spot rates**  on calcul la present value en remplacement le YTM par les **spots rates** ensuite on viens calculer le YTM avec cette **present value** et la **calculatrice financière**

### Dirty price vs Clean price

Supposons que tu as une obligation qui paie un **coupon annuel** de 100 €, chaque 1er janvier.

1. **Le 1er janvier** : Tu reçois 100 € de coupon. Juste après, tu ne possèdes plus d'intérêts courus, car tu viens de recevoir ton paiement.
    
2. **Le 1er juillet** : Tu veux vendre ton obligation. Il s'est écoulé 6 mois depuis le dernier coupon, donc 6 mois d'intérêts se sont accumulés. Comme le coupon annuel est de 100 €, tu as accumulé 50 € d'intérêts courus (la moitié du coupon annuel).

- **Clean Price** : C'est le prix de l'obligation sans tenir compte des intérêts courus (par exemple, 1 000 €).
    
- **Intérêts Courus** : 50 € que tu as accumulés en détenant l'obligation depuis le dernier paiement de coupon.
    
- **Dirty Price** : Si quelqu'un achète ton obligation le 1er juillet, il devra te payer le **clean price** (1 000 €) **plus** les 50 € d'intérêts courus. Le total est donc 1 050 €.


#### Méthode de calcul : 

![Pasted image 20240817194001.png](/img/user/Data/Pasted%20image%2020240817194001.png)



### Passer du Dirty Price au Clean Price avec le Accrued interest : 

![Pasted image 20240817194355.png](/img/user/Data/Pasted%20image%2020240817194355.png)

![Pasted image 20240817194413.png](/img/user/Data/Pasted%20image%2020240817194413.png)


### Passer du spot rates au forward rates : 

Définissons les notions de **spot rates** et de **forward rates** : 

Le taux spot est le taux d'intérêt applicable aujourd'hui pour un investissement qui commence immédiatement et qui se termine à une date précise dans le futur.

Le taux forward est le taux d'intérêt prévu pour un investissement qui commencera à une date future et se terminera à une autre date future.

![Pasted image 20240819174315.png](/img/user/Data/Pasted%20image%2020240819174315.png)

==Le spot rate permets de calculer le taux forward avec la formule suivante : 

![Pasted image 20240819174417.png](/img/user/Data/Pasted%20image%2020240819174417.png)
*Une version plus lisible est la suivante : 

![Pasted image 20240819174707.png](/img/user/Data/Pasted%20image%2020240819174707.png)

![Pasted image 20240819174919.png](/img/user/Data/Pasted%20image%2020240819174919.png)

===Retenons que le F1 est obtenu avec le S1 et le S2, le F2 serais obtenu avec le S2 et le S3.


### Les Forward Rate Agreements (FRAs)

Un **FRA (Forward Rate Agreement)** est un contrat financier entre deux parties qui fixe un taux d'intérêt pour un futur prêt ou emprunt, pour une période spécifique à venir. L'idée principale est de se protéger contre la fluctuation des taux d'intérêt ou de profiter des variations prévues.

Imaginons qu'une entreprise prévoit d'emprunter 1 million d'euros dans 3 mois, pour une durée de 6 mois. L'entreprise craint que les taux d'intérêt augmentent d'ici là, ce qui rendrait l'emprunt plus coûteux.

- **FRA conclu aujourd'hui** : L'entreprise signe un FRA avec une banque, fixant un taux d'intérêt de 4 % pour cet emprunt de 6 mois, commençant dans 3 mois.
    
- **Après 3 mois** : Si le taux d'intérêt du marché est supérieur à 4 %, disons 5 %, l'entreprise devra payer 5 % d'intérêts sur son emprunt, mais recevra une compensation de la banque pour la différence de 1 % (par rapport au 4 % fixé dans le FRA).
    
- **Si le taux est inférieur à 4 %** : L'entreprise paiera toujours 4 % (comme convenu dans le FRA), même si le taux d'intérêt du marché est par exemple de 3 %. Dans ce cas, l'entreprise paie plus que le taux du marché, mais elle avait la sécurité de savoir à l'avance combien elle paierait


--- 

Comment le calculer ? : 

Un FRA couvre une période future spécifique. Par exemple, si vous voulez couvrir les taux d'intérêt pour une **période de 6 mois qui commence dans 1 an**, vous avez deux moments clés :

- Le début du FRA : 1 an (au bout de 12 mois).
- La fin du FRA : 1,5 an (au bout de 18 mois).

![Pasted image 20240821193014.png](/img/user/Data/Pasted%20image%2020240821193014.png)

La puissance 1/0.5 dans l'exemple correspond au fait que nous calculons un taux forward pour une période de 6 mois (ou 0,5 an)

- Si la période future était de 1 an, l'exposant serait 1/1
- Si la période future est de 6 mois (0,5 an), l'exposant est 10/5


## La duration 

On viens distinguer deux duration, **duration de Macaulay** et **duration modifie** 

===Retenons que la duration est plus élevés quand les obligations sont sur une plus grosse durée car on manque des opportunités sur les marches pendant une plus grosse période.

===Un coupon élevé au contraire va permettre d'avoir une duration moins élevés, car on aura un retour sur investissement plus rapide donc on pourra aller chercher d'autres opportunités. 

==Pour finir une obligation zéro coupon est bien plus sensible car pas de coupons donc une duration plus longue.==


### Duration de Macaulay

C'est un resultat qui s'exprime en annees, le nombres d'annees necessaire avant le remboursement de son investissement , pour mieux le comprendre on doit partir du principe que l'obligation rembourse en continue.

Le calcul est assez simple :

Multiplier les flux de l'annes par l'annes, pour venir chercher une division par la present value de l'obligation.

![Pasted image 20240829075145.png](/img/user/Data/Pasted%20image%2020240829075145.png)



\

### Duration modifie ou classique 

C'est un calcul qui exprime la sensibilite d'une obligation aux taux d'interets. Elle ce base sur le calcul de la duration de Macaulay

![Pasted image 20240829075350.png](/img/user/Data/Pasted%20image%2020240829075350.png)



### La convexité et la duration (linéaire vs non linéaire)

#### **La Duration Modifiée : Une Approximative Linéaire**

- **Ce qu'elle mesure** : La duration modifiée mesure la sensibilité du prix d'une obligation à une petite variation des taux d'intérêt, en supposant que la relation entre le prix de l'obligation et le taux d'intérêt est linéaire.
    
- **Limite** : Cette linéarité implique que la duration modifiée est précise pour des petites variations de taux d'intérêt, mais devient de moins en moins précise pour des variations plus importantes. Cela s'explique parce que la relation réelle entre le prix d'une obligation et le taux d'intérêt est courbe (non linéaire), pas une ligne droite.
    

#### 2. **La Convexité : Une Correction Non Linéaire**

- **Ce qu'elle mesure** : La convexité capture la courbure (ou la forme non linéaire) de la relation entre le prix d'une obligation et les taux d'intérêt. Elle mesure donc non seulement la sensibilité initiale (comme la duration), mais aussi comment cette sensibilité change à mesure que les taux d'intérêt changent.
    
- **Avantage** : Parce qu'elle prend en compte cette courbure, la convexité offre une correction pour les approximations faites par la duration modifiée. Elle est particulièrement utile lorsque les taux d'intérêt subissent des variations importantes. En incluant la convexité dans le calcul, on obtient une estimation plus précise du changement de prix de l'obligation.


==Ce que l'on retiens c'est que changer 1 pourcent sur un taux a 1 % c'est changer 100 % sur un taux a 2 % c'est 50 % alors forcement cela ne peut être linéaire. 

![Pasted image 20240902184147.png](/img/user/Data/Pasted%20image%2020240902184147.png)



