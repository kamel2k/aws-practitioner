## Introduction du module 10 et objectifs

- Résumer les six piliers du cadre Well-Architected Framework.  
- Expliquer les six avantages du cloud computing.

---

## Le cadre AWS Well-Architected Framework

Six pilliers

![](images/wellarchitected.png)<!-- .element height="55%" width="55%" --> 

---

## Excellence opérationnelle

- L'Excellence opérationnelle est la capacité d'exécuter et de surveiller les systèmes pour assurer une valeur métier et pour améliorer en continu les processus et procédures de prise en charge.  
- Les principes de conception de l'excellence opérationnelle dans le cloud incluent l'exécution d'opérations sous forme de code, l'annotation de documentation, l'anticipation des échecs et l'application fréquente de petites modifications réversibles.

---

## Sécurité

- Le pilier Sécurité représente la capacité à protéger les informations, les systèmes et les ressources tout en fournissant une valeur métier par le biais de stratégies d'évaluation et de limitation des risques. 
- bonnes pratiques:
   - Automatisez les bonnes pratiques de sécurité lorsque cela est possible.
   - Appliquez la sécurité à toutes les couches.
   - Protégez les données en transit et au repos.

---

## Fiabilité

- Récupérer après les interruptions de service ou d'infrastructure
- Acquérir dynamiquement des ressources de calcul pour répondre à la demande
- Atténuer les perturbations telles que les erreurs de configuration ou les problèmes de réseau temporaires
- La fiabilité comprend le test des procédures de reprise, la mise à l'échelle horizontale pour renforcer la disponibilité globale du système, ainsi que la reprise automatique après une défaillance.

---

## Efficacité des performances

- L'efficacité des performances est la capacité d'utiliser efficacement les ressources de calcul pour répondre aux exigences du système et maintenir l'efficacité au fur et à mesure que la demande change et que les technologies évoluent. 
- Pour évaluer l'efficacité des performances de votre architecture, il faut expérimenter plus souvent, utiliser des architectures serverless et concevoir des systèmes pouvant toucher le monde entier en quelques minutes.

---

## Optimisation des coûts

- L'optimisation des coûts est la capacité à exécuter des systèmes de façon à assurer une valeur métier au niveau de prix le plus bas.
- L'optimisation des coûts inclut l'adoption d'un modèle de consommation, l'analyse et l'attribution des dépenses et l'utilisation de services gérés pour réduire le coût de possession.

---

## La durabilité 


- Capacité à continuellement améliorer les impacts sur la durabilité en réduisant la consommation d'énergie et en augmentant l'efficacité pour tous les composants d'une charge de travail en optimisant les avantages des ressources mises en service et en minimisant le nombre total de ressources requises.

  - Comprenez votre impact
  - Définissez des objectifs de durabilité
  - Optimisez l'utilisation
  - Anticipez et adoptez de nouvelles offres de matériels et de logiciels plus efficaces
  - Utilisez des services gérés
  - Réduisez l'impact en aval de vos charges de travail dans le cloud

---

<!-- .slide: data-auto-animate -->
<!-- .slide: data-auto-animate -->
#### Quiz: Quel pilier du cadre AWS Well-Architected Framework met l'accent sur la capacité d'une charge de travail à exécuter de manière cohérente et appropriée les fonctions prévues ? <!-- .element: style="color:#fd9731;" -->

- Excellence opérationnelle
- Efficacité des performances
- Sécurité
- Fiabilité

---

<!-- .slide: data-auto-animate -->
#### Quiz: Quel pilier du cadre AWS Well-Architected Framework met l'accent sur la capacité d'une charge de travail à exécuter de manière cohérente et appropriée les fonctions prévues ? <!-- .element: style="color:#fd9731;" -->

- Excellence opérationnelle
- Efficacité des performances
- Sécurité
- Fiabilité <!-- .element: style="color:#0de07d;" -->

---

<!-- .slide: data-auto-animate -->
#### Quiz: Quel pilier du cadre AWS Well-Architected Framework inclut la capacité à efficacement exécuter des charges de travail et à obtenir des informations sur leurs opérations ? <!-- .element: style="color:#fd9731;" -->

- Optimisation des coûts
- Excellence opérationnelle
- Efficacité des performances
- Fiabilité

---

<!-- .slide: data-auto-animate -->
#### Quiz: Quel pilier du cadre AWS Well-Architected Framework inclut la capacité à efficacement exécuter des charges de travail et à obtenir des informations sur leurs opérations ? <!-- .element: style="color:#fd9731;" -->

- Optimisation des coûts
- Excellence opérationnelle <!-- .element: style="color:#0de07d;" -->
- Efficacité des performances
- Fiabilité

---

## Autres Services managés 1

- AWS Systems Manager: permet d'intégrer les ressources sur site à l'environnement cloud AWS pour une gestion centralisée. Grâce à l'agent SSM installé sur vos serveurs physiques ou machines virtuelles (VM) sur site, vous pouvez gérer ces systèmes en parallèle avec vos ressources AWS
- Amazon Connect: est un service de centre de contact cloud qui permet aux entreprises de configurer un centre d'appels virtuel facilement et rapidement. Il permet de gérer les interactions avec les clients par téléphone, chat, et autres canaux numériques. 
- AWS Global Accelerator: est un service réseau qui améliore la disponibilité et la performance des applications accessibles via Internet, en utilisant l'infrastructure mondiale d'AWS 
    - Optimisation du routage : Il dirige le trafic utilisateur vers l'endpoint AWS optimal (comme des instances EC2, des load balancers ou des clusters ECS) en fonction des performances réseau et de la géolocalisation de l'utilisateur, réduisant ainsi la latence
    - Tolérance aux pannes : Si un endpoint devient indisponible, Global Accelerator redirige automatiquement le trafic vers un autre endpoint assurant ainsi une haute disponibilité pour vos applications.

---

## Autres Services managés 2

- AWS Config : est un service de gestion de la conformité et des configurations qui permet de surveiller, auditer et évaluer les configurations de vos ressources AWS
    - Suivi des configurations : AWS Config capture l'état des ressources AWS (telles que les instances EC2, les buckets S3, les VPC, etc.) et suit les modifications apportées à leur configuration au fil du temps. Cela permet de visualiser l'historique des configurations et de comprendre comment elles ont évolué.
    - Évaluation de la conformité : Vous pouvez définir des règles de conformité basées sur les meilleures pratiques de sécurité, de performance ou d'autres exigences spécifiques à votre entreprise. AWS Config vérifie ensuite en continu si vos ressources respectent ces règles et signale les écarts.
    - Tableau de bord unifié : Il fournit une vue centralisée de toutes les ressources AWS gérées, montrant leur statut et leur conformité en temps réel, ce qui simplifie la gestion de la sécurité et des opérations.

---

## Autres Services managés 3 

- Amazon EMR (Elastic MapReduce) est un service cloud qui permet de traiter et analyser de grandes quantités de données à l'aide de frameworks tels que Apache Hadoop, Apache Spark, HBase, Presto, et Flink. 
- Amazon Cognito : est un service AWS qui permet d'ajouter des fonctionnalités d'authentification, d'autorisation et de gestion des utilisateurs à vos applications web et mobiles.
- AWS OpsWorks est un service qui permet d'automatiser la configuration, le déploiement et la gestion des applications sur des serveurs dans le cloud ou sur site, en utilisant des frameworks de gestion de configuration comme Chef et Puppet.
- AWS Storage Gateway : fournit une solution hybride qui permet à votre infrastructure locale de se connecter et de tirer parti du cloud AWS (S3 et Glacier), principalement pour des tâches comme :
    - Sauvegarde des fichiers ou volumes locaux vers le cloud.
    - Archivage à long terme dans des services de stockage cloud comme Amazon Glacier.

---

## Autres Services managés 4

- AWS Certificate Manager (ACM) est un service qui facilite la gestion des certificats SSL/TLS pour sécuriser les applications web et d'autres ressources hébergées sur AWS
- Amazon ECR (Elastic Container Registry) est un service entièrement géré par AWS qui permet de stocker, gérer et déployer des images de conteneurs Docker de manière sécurisée.
- Amazon Kinesis Video Streams est un service entièrement géré qui facilite le streaming en temps réel de vidéos depuis des appareils connectés, des caméras ou d'autres sources vers AWS pour le stockage, le traitement et l'analyse
- Amazon SES (Simple Email Service) est un service de messagerie électronique cloud d'AWS qui permet d'envoyer et de recevoir des e-mails de manière évolutive, fiable et économique.
- AWS Health Dashboard est un outil qui fournit des informations en temps réel et personnalisées sur l'état des services AWS et l'impact potentiel sur vos ressources. Il vous aide à surveiller la santé de vos services et à identifier rapidement les problèmes qui peuvent affecter votre infrastructure.

---

## Autres Services managés 5

- AWS Secrets Manager est un service qui permet de gérer, protéger et récupérer des informations sensibles, comme des identifiants, des clés d'API, des mots de passe ou d'autres secrets, de manière sécurisée. 
- Amazon MQ est un service de messagerie géré qui facilite l'intégration et la communication entre les différentes applications et services en utilisant des protocoles de messagerie standard comme Apache ActiveMQ et RabbitMQ.
- AMI (Amazon Machine Image) est une image préconfigurée qui contient les informations nécessaires pour lancer une instance dans Amazon EC2. Elle sert de modèle pour démarrer des serveurs virtuels en spécifiant le système d'exploitation, les logiciels, les bibliothèques, et les configurations spécifiques. 
- Amazon Comprehend est un service AWS de traitement du langage naturel (NLP) qui utilise l'intelligence artificielle et le machine learning pour extraire des informations significatives à partir de textes non structurés. 
- AWS X-Ray est un service qui permet de faire du traçage distribué

---

## Autres Services managés 6

- AWS Cloud9 est un environnement de développement intégré (IDE) en cloud 
- AWS Data Pipeline est un service web qui permet de déplacer et de transformer des données de manière fiable entre différents services AWS ou entre des sources de données sur site et des services AWS. Il permet d'automatiser le déplacement, la transformation, et le traitement de grandes quantités de données dans des intervalles de temps définis, facilitant la création de flux de travail de traitement de données.
- AWS Glue est un service entièrement géré d'intégration de données qui permet de préparer, nettoyer, et transformer les données pour les analyses et le reporting. Il facilite l'extraction, la transformation et le chargement des données (ETL) à partir de différentes sources vers des entrepôts de données comme Amazon Redshift, des lacs de données sur Amazon S3, ou des bases de données relationnelles comme Amazon RDS

AWS Glue est un service ETL sans serveur automatisé conçu pour la préparation et la transformation de données pour l'analyse, tandis que AWS Data Pipeline est un service d'orchestration flexible permettant de déplacer et traiter les données entre différents services AWS ou environnements sur site avec plus de contrôle manuel.

---

## Autres Services managés 7

- Amazon Polly est un service de synthèse vocale qui convertit du texte en discours réaliste
- AWS CodeCommit est un service de gestion de code source entièrement géré qui facilite le stockage et la gestion de votre code dans des dépôts Git.
- AWS CodeArtifact est un service de gestion de référentiels qui vous permet de stocker, partager et déployer des artefacts de logiciels.
- AWS CodeBuild est un service entièrement géré qui compile le code source, exécute des tests et produit des artefacts prêts à être déployés.
- AWS Cloud Map est un service de découverte de services qui permet de localiser les ressources cloud et de les associer à des noms de services
- AWS OpsCenter est un service qui facilite la gestion et la résolution des problèmes liés aux ressources AWS.

---

## Autres Services managés 8

- Amazon Macie est un service de sécurité et de protection des données qui utilise l'apprentissage automatique pour aider à découvrir, classer et protéger les données sensibles dans Amazon S3.
- AWS Migration Hub est un service qui facilite la planification et la gestion des migrations vers AWS. Il fournit une vue centralisée de vos projets de migration, vous aidant à suivre le progrès et à coordonner les efforts de migration.





