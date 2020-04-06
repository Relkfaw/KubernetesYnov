# KubernetesYnov
---
## Namespaces
### KubeDB
#### Ressources minimales:
  * 0.5 CPU
  * 1 Gi de mémoire

#### Ressources maximales:
  * 1 CPU
  * 2 Gi de mémoire

#### Pourquoi?
Ce namespace contenant la base de données KubeDB, il n'a pas besoin de beaucoup de ressources processeur, mais de mémoire pour stocker une grande quantité d'information.

### Wordpress
#### Ressources minimales:
  * 1 CPU
  * 500 Mi de mémoire

#### Ressources maximales:
  * 2 CPU
  * 1536 Mi de mémoire

#### Pourquoi?
Ce namespace contenant le pod Wordpress, il lui faut des ressources processeur en grande quantité afin de charger rapidement l'interface graphique du site.
Malgré tout, il doit pouvoir générer les pages riches en images ou vidéos, d'où la limite en mémoire élevée.
