---
{"dg-publish":true,"permalink":"/secteur-d-activites/intelligence-artificielle/"}
---

### Fonctionnement

Un modèle traditionnel, qui se concentre sur la détection de « patterns », qui classe et prédise des donnés.

Un modèle génératif, qui permets de créer de nouvelles données à partir de donnés exemples.

Les modèles génératifs ce basent sur le DEEP LEARNING (machine Learning).   

Dans le contexte de l’IA et du ML, un modèle est un algorithme mathématique qui est entraîné pour arriver au même résultat ou à la même prévision qu’un expert humain lorsqu’on lui fournit les mêmes informations. Dans le cas du deep learning, les algorithmes sont inspirés de la structure du cerveau humain, et connus sous le nom de réseaux neuraux.  Il existe différents modèles de deep learning que l’on peut envisager comme différente structures neuronales.

Si on prend l’exemples d’agents conversationnels comme chatgpt alors on est sur un réseau neuronal de type Large Language Models qui est l’aboutissement d’un autre modele neuronal (transformers).

 

**Les différentes configurations neuronales possible pour l’IA :**

![image001 (1).png](/img/user/Data/image001%20(1).png)


**Zoom sur CHATGPT :****

Si on prend l’exemples d’agents conversationnels comme chatgpt alors on est sur un réseau neuronal de type Large Language Models qui est l’aboutissement d’un autre modele neuronal (transformers).

 

**Le fonctionnement d’un LLM :****
![image004.png](/img/user/Data/image004.png)

![image002.png](/img/user/Data/image002.png)
 
Chaque mot est tokenisé, l’intelligence artificielle va observer les suites de tokens les plus reprises sur la data qu’elle possède pour pouvoir par la suite prédire le prochain mot d’une phrase.

Le fonctionnement du next token prédiction : https://alonsosilva-tokenizer.hf.space/

 

Si on reprend l’exemple de Chatgpt , il va ce nourrir de data, pour assimiler les suites logiques de tokens.

![image005.png](/img/user/Data/image005.png)

 

Le next token prediction n’est pas suffisant il ne permets pas à l’IA de discuter , elle va donc être entrainé en 3 phases pour devenir un agent conversationnel
![image006.png](/img/user/Data/image006.png)

 Pour résumé : On créer un réseau de neurone profonds qui s’améliore par le biais du Next token prédiction, on lui envoie énormément de data pour alimenter ses neurones, on couple ça a un entrainement pour le rendre conversationnel.


![image001 (2).png](/img/user/Data/image001%20(2).png)