---
unique-page-id: 11379928
description: Modification des détails dans le journal d’audit - Documents Marketo - Documentation du produit
title: Modification des détails dans le journal d’audit
exl-id: 5583be62-46a6-42f9-b4b3-0df63a171b2d
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1902'
ht-degree: 14%

---

# Modification des détails dans le journal d’audit {#change-details-in-audit-trail}

Le journal d’audit offre de nombreuses informations sur les personnes qui effectuent les opérations dans votre abonnement Marketo. Voici les détails.

## Journal d’audit de la ressource {#asset-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">Ressource/Type</th> 
   <th colspan="1">Action</th> 
   <th colspan="1">Modifier les détails</th> 
  </tr> 
  <tr> 
   <td rowspan="15"><strong>Programme par défaut</strong><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>Créer</td> 
   <td>Type de canal "type de canal"<br>ou<br>cloné à partir de "nom de programme"</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur l'espace de travail "nom de l'espace de travail" <br>Emplacement "Dossier de campagne" ou "Programme d'engagement" <br>Nom du programme cloné "nouveau nom"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Modifier le canal</td> 
   <td>Nouveau canal "nouveau nom du canal" Ancien canal "ancien nom du canal" </td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Ajouter la valeur "token name" du jeton "token value"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Modifier le jeton "token name" nouvelle valeur "new value" ancienne valeur "old value"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Supprimer le jeton "token name"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Ajouter "nom du comportement" du comportement d’analyse</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td><p>Modifier le "nom du comportement" du comportement d’analyse</p><p>Ancien "nom du comportement"</p></td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Suppression du comportement d’analyse "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Ajoutez la valeur de coût de période "#" du mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Coût de la période d'édition Nouvelle valeur de coût "#", Nouveau mois de programme "aaaa-mm", Ancien valeur de coût "#", Ancien mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Supprimer le coût par période. Valeur "#" du mois du programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td>Exporter</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td rowspan="19"><strong>E-mail</strong><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>Créer</td> 
   <td>Créé à l'aide du modèle "nom du modèle" <br> ou <br>cloné à partir de "nom de ressource"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Mise à jour de "Du nom" à "Nouveau du nom"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Mise à jour de "From Email" vers "newemail@name.com"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Mise à jour de "Répondre à" à "newreplytoemail@name.com"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Mise à jour de "Objet" en "nouvelle ligne d’objet"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Ajout de la segmentation "segmentation_name"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Segmentation supprimée</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Ajout du fragment de code "fragment de code_name"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Extrait supprimé</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Les modifications ont interrompu le courrier électronique à partir du modèle "template_name" (REMARQUE : cela se produit aujourd’hui si vous modifiez directement le code).</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" Ancienne description "ancienne description"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Modifier le module <module name><attribute> à "value"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "Design Studio" dans le dossier "nom de dossier" <br>Nom de ressource cloné "nom"<br>ou<br>cloné à "Activités marketing" dans le programme "nom de programme"<br>Nom de ressource cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Déplacer</td> 
   <td>Déplacé vers "Design Studio" dans le dossier "nom du dossier"<br>ou<br>Déplacé vers "Activités marketing" dans "nom du programme"</td> 
  </tr> 
  <tr> 
   <td>Approuver</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Dévalider</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Brouillon</td> 
   <td>L'email a été rédigé car le fragment de code "nom du fragment de code" a été approuvé<br>ou<br>L'email a été rédigé car le modèle "nom du modèle" a été approuvé.</td> 
  </tr> 
   <td rowspan="17">Programme d’e-mail</td> 
   <td>Créer</td> 
   <td>Type de canal "type de canal"<br>ou<br>cloné à partir de "nom de programme"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Renommer</td> 
   <td colspan="1">Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur l'espace de travail "nom de l'espace de travail" <br>Emplacement "Dossier de campagne ou programme d'engagement" <br>Nom du programme cloné "nouveau nom"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Abandonner</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Modifier le canal</td> 
   <td>Nouveau canal "nouveau canal" Ancien canal "ancien canal"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Ajouter la valeur "token name" du jeton "token value"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Modifier le jeton "token name" Nouvelle valeur "new value" ancienne valeur "old value"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Supprimer le jeton "token name"</td> 
  </tr> 
  <tr> 
   <td>Modifier le planning du programme</td> 
   <td>Définir le planning pour qu’il commence à la "date de début, heure de début" et se termine par "date de fin, heure de fin"</td> 
  </tr> 
  <tr> 
   <td>Modifier le planning du programme</td> 
   <td>Modification du planning en "nouvelle date, nouvelle heure"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Ajouter "nom du comportement" du comportement d’analyse</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Modifier le comportement d’analyse "nom du comportement"<br>Ancien comportement "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Suppression du comportement d’analyse "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Ajoutez la valeur de coût de période "#" du mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Coût de la période d'édition Nouvelle valeur de coût "#", Nouveau mois de programme "aaaa-mm", Ancien valeur de coût "#", Ancien mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Supprimer le coût par période. Valeur "#" du mois du programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Modèle d'e-mail</td> 
   <td>Créer</td> 
   <td>Vide ou cloné à partir de "nom du modèle"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description", description précédente "description précédente"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>HTML modifié</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "nom du dossier" <br> Nom de ressource cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Approuver</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Dévalider</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td rowspan="23">Programme d’engagement</td> 
   <td>Créer</td> 
   <td>Type de canal "type de canal"<br> ou<br> cloné à partir de "nom du programme"</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur l'espace de travail "nom de l'espace de travail" <br>Emplacement "Dossier de campagne ou programme d'engagement" <br>Nom du programme cloné "nouveau nom"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Modifier le canal</td> 
   <td>Nouveau canal "nouveau canal" Ancien canal "ancien canal"</td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td><p>Ajouter un flux</p><p>Nom "name" Placement "#"</p></td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td><p>Modification du flux</p><p>Nouveau nom du flux : "nouveau nom" Ancien nom du flux : "ancien nom"</p><p>Nouvel emplacement : "nouveau #" Ancien emplacement : "ancien #"</p></td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td>Suppression du nom de flux "name"</td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td>Ajoutez du contenu <br>Nom de flux"<br>Type "Email" ou "Program"<br>Nom de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de production"{3<br>Type "Nom de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de flux de</td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td>Activer le contenu<br>Nom de la diffusion "nom de la diffusion"<br>Nom du contenu "nom de l’email" ou "nom du programme"</td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td>Désactivez le contenu<br>Nom de la diffusion "nom de la diffusion"<br>Nom du contenu "nom de l’email" ou "nom du programme"</td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td>Supprimez le contenu<br>Nom du flux "nom du flux"<br>Nom du contenu "nom de l’email" ou "nom du programme"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Ajouter la valeur "token name" du jeton "token value"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Modifier le jeton "token name" Nouvelle valeur "new value" ancienne valeur "old value"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Supprimer le jeton "token name"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Ajouter "nom du comportement" du comportement d’analyse</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Modifier le comportement d’analyse "nom du comportement"<br>Ancien comportement "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Suppression du comportement d’analyse "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Modifier le statut du programme. Nouvelle valeur "on/off" Ancienne valeur "off/on"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Ajoutez la valeur de coût de période "#" du mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Coût de la période d'édition Nouvelle valeur de coût "#", Nouveau mois de programme "aaaa-mm", Ancien valeur de coût "#", Ancien mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Supprimer le coût par période. Valeur "#" du mois du programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td>Exporter</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td rowspan="18">Programme d’événement</td> 
   <td>Créer</td> 
   <td>Type de canal "type de canal"<br>ou<br>cloné à partir de "nom de programme"</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur l'espace de travail "nom de l'espace de travail" <br>Emplacement "dossier de campagne" ou "programme d'engagement" <br>Nom du programme cloné "nouveau nom"</td> 
  </tr> 
  <tr> 
   <td>Modifier le canal</td> 
   <td>Nouveau canal "nouveau canal" Ancien canal "ancien canal" </td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Ajouter la valeur "token name" du jeton "token value"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Modifier le jeton "token name" Nouvelle valeur "new value" ancienne valeur "old value"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Supprimer le jeton "token name"</td> 
  </tr> 
  <tr> 
   <td>Modifier le planning du programme</td> 
   <td>Définir le planning pour qu’il commence à la "date de début, heure de début" et se termine par "date de fin, heure de fin"</td> 
  </tr> 
  <tr> 
   <td>Modifier le planning du programme</td> 
   <td>Modification du planning en "nouvelle date, nouvelle heure"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Ajouter "nom du comportement" du comportement d’analyse</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Modifier le comportement d’analyse "nom du comportement"<br>Ancien comportement "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration du programme</td> 
   <td>Suppression du "nom du comportement" du comportement d’analyse</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Ajoutez la valeur de coût de période "#" du mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Coût de la période d'édition Nouvelle valeur de coût "#", Nouveau mois de programme "aaaa-mm", Ancien valeur de coût "#", Ancien mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Supprimer le coût par période. Valeur "#" du mois du programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration du programme</td> 
   <td colspan="1">Ajout du partenaire d’événement "partner_name"</td> 
  </tr> 
  <tr> 
   <td>Exporter</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td rowspan="5">Dossiers</td> 
   <td>Créer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Ajout du jeton "token_name", valeur "value"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Jeton modifié "token_name" nouvelle valeur "token_value" ancienne valeur "old_token_value"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Jeton supprimé "token_name"</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Formulaires</td> 
   <td>Créer</td> 
   <td>Bientôt disponible. En savoir plus ou cloné à partir de "nom du formulaire"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" Ancienne description "ancienne description"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Paramètres du formulaire modifiés </td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Informations sur le champ modifié</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "Design Studio" dans le dossier "nom de dossier" <br>Nom de ressource cloné "nom"<br>ou<br>cloné à "Activités marketing" dans le programme "nom de programme"<br>Nom de ressource cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Déplacer</td> 
   <td>Déplacé vers "Design Studio" dans le dossier "nom du dossier"<br>ou<br>Déplacé vers "Activités marketing" dans "nom du programme"</td> 
  </tr> 
  <tr> 
   <td>Formulaires</td> 
   <td>Approuver</td> 
   <td>Utilisé par # ressources </td> 
  </tr> 
  <tr> 
   <td rowspan="9">Page de destination</td> 
   <td>Créer</td> 
   <td>Créé à l'aide du modèle "nom du modèle" <br> ou <br>cloné à partir de "nom de ressource"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" Précédent "description précédente"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Ajout de "Image", suppression de "Image", composant Image modifié</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Ajout de "Texte enrichi", suppression de "Texte enrichi", composant Texte enrichi modifié</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "Design Studio" dans le dossier "foldername"<br>Nom de ressource cloné "name"<br>URL de ressource clonée "www.url.com"<br>ou<br>cloné à "Activités marketing" dans le programme "nom du programme" <br>Nom de ressource cloné "name"<br>URL de ressource clonée "www.url.com"</td> 
  </tr> 
  <tr> 
   <td>Déplacer</td> 
   <td>Déplacé vers "Design Studio" dans le dossier "nom du dossier"<br> ou<br> Déplacé vers "Activités marketing" vers "nom du programme"</td> 
  </tr> 
  <tr> 
   <td>Approuver</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Brouillon</td> 
   <td>La landing page a été ébauchée car le modèle "nom du modèle" a été approuvé.</td> 
  </tr> 
  <tr> 
   <td>Dévalider</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Modèle de page de destination</td> 
   <td>Créer</td> 
   <td><p>Vierge<br>ou<br>cloné à partir de "nom de ressource"</p></td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" description précédente "description précédente"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "nom du dossier" <br>Nom de la ressource clonée "nom"</td> 
  </tr> 
  <tr> 
   <td>Exporter</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Approuver</td> 
   <td>Utilisé par # ressources </td> 
  </tr> 
  <tr> 
   <td>Dévalider</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td rowspan="5">Liste (statique)</td> 
   <td>Créer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Exporter</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "Base de données de personne" dans le dossier "nom de dossier" <br>Nom de ressource cloné "nom"<br>ou<br>Cloné sur "Activités marketing" dans le programme "nom de programme"<br>Nom de ressource cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td rowspan="12">Campagne intelligente</td> 
   <td>Créer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Activer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Désactiver</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Abandonner</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Déplacer</td> 
   <td>Déplacement vers "Programmes" en "nom du programme"<br>ou<br>Déplacé vers "Dossiers" dans le dossier "nom du dossier"</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" Précédent "description précédente"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "Programmes" dans le programme "nom du programme" <br>Nom de ressource cloné "nom"<br>ou<br>Cloné sur "Dossier" dans le dossier "nom du dossier"<br>Nom de ressource cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration de la liste intelligente</td> 
   <td>Affiche un instantané de l’état actuel, y compris les noms et les valeurs des filtres et des déclencheurs.</td> 
  </tr> 
  <tr> 
   <td>Modification du planning de campagne</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Modification de l’action d’étape de flux</td> 
   <td>Affiche un instantané de l’état actuel, y compris les noms et les valeurs de chaque étape de flux.</td> 
  </tr> 
  <tr> 
   <td rowspan="7">Liste intelligente</td> 
   <td>Créer</td> 
   <td>Cloné à partir du "nom de liste dynamique"</td> 
  </tr> 
  <tr> 
   <td>Exporter</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" Précédent "description précédente"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "Base de données de personne" dans le dossier "nom de dossier" <br>Nom de ressource cloné "nom"<br>ou<br>cloné à "Activités marketing" dans le programme "nom de programme" <br>Nom de ressource cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration de la liste intelligente</td> 
   <td>Affiche un instantané de l’état actuel, y compris les noms et les valeurs des filtres et des déclencheurs. </td> 
  </tr> 
  <tr> 
   <td rowspan="11">Extrait</td> 
   <td>Créer</td> 
   <td><p>Blank<br>or<br>Cloner à partir de "nom de fragment de code"</p></td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Ajout de la segmentation "segmentation_name"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Segmentation supprimée</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Modifié</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", nom précédent "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" Précédent "description précédente"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "nom du dossier" <br>Nom du fragment de code cloné"</td> 
  </tr> 
  <tr> 
   <td>Approuver</td> 
   <td>Utilisé par # ressources</td> 
  </tr> 
  <tr> 
   <td>Approuver sans brouillon</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Dévalider</td> 
   <td><p>S/O</p></td> 
  </tr> 
 </tbody> 
</table>

## Journal d’audit de l’administrateur {#admin-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Zone d’administration</th> 
   <th>Action</th> 
   <th>Modifier les détails</th> 
  </tr> 
  <tr> 
   <td>Restrictions IP</td> 
   <td>Modifier</td> 
   <td>Modification des restrictions d’adresse IP aux suivantes : "block" autorisé/bloqué, "address"#", "disabled IP Restrictions"</td> 
  </tr> 
  <tr> 
   <td rowspan="2">Division</td> 
   <td>Créer</td> 
   <td>Partition créée avec le nom "partition name"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>"nom de la partition" partition supprimée</td> 
  </tr> 
  <tr> 
   <td>Niveau de sécurité du mot de passe</td> 
   <td>Modifier</td> 
   <td>La sécurité du mot de passe a été remplacée par le modèle : Sécurité standard, longueur min. : #, inférieur-supérieur : #, nombre : #, casse mixte : #, expiration : #, délai d’expiration de la session : #</td> 
  </tr> 
  <tr> 
   <td rowspan="3">Rôle<br><br></td> 
   <td>Créer</td> 
   <td>Rôle créé avec "nom du rôle" (REMARQUE : si vous avez besoin de détails sur les autorisations ajoutées, veuillez contacter l’assistance) - <br>affiche un instantané des autorisations affectées au rôle</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>Suppression du rôle "Nom du rôle"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Rôle Modifié de "nom précédent" en "nouveau nom" (REMARQUE : si vous avez besoin de détails sur les autorisations modifiées, veuillez contacter l’assistance) - <br>affiche un instantané des autorisations affectées au rôle<br></td> 
  </tr> 
  <tr> 
   <td>Rapport des listes intelligentes</td> 
   <td>Modifier</td> 
   <td>SmarList édité pour connexion à télécharger : "true ou false"</td> 
  </tr> 
  <tr> 
   <td rowspan="7">Utilisateur<br><br><br><br></td> 
   <td>Créer (invitation)</td> 
   <td>L’utilisateur est invité avec : Email "email address", Name "first and last name", Access Expires "blank or with a date", API User "true or false" - <br> affiche un instantané des rôles et des espaces de travail attribués à l’utilisateur</td> 
  </tr> 
  <tr> 
   <td colspan="1">Supprimer</td> 
   <td colspan="1">"nom d’utilisateur" utilisateur supprimé</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>L’utilisateur a été renommé "ancien nom" en "nouveau nom" par email : "email", apiUser: "vrai ou faux" l’accès expire : "vide ou avec une date"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>L’utilisateur a été modifié pour le courrier électronique : "email", apiUser: "true ou false", l’accès expire : "vide ou avec une date"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifier</td> 
   <td colspan="1">Affiche un instantané de l’état actuel, y compris les rôles et les espaces de travail affectés à l’utilisateur.</td> 
  </tr> 
  <tr> 
   <td>Problème</td> 
   <td>Licence de calendrier émise à l’adresse électronique : nom "adresse électronique de l’utilisateur" : "nom de l’utilisateur"</td> 
  </tr> 
  <tr> 
   <td>Réinitialiser</td> 
   <td>Réinitialisation du mot de passe pour le nom "name" et l’email "email"</td> 
  </tr> 
  <tr> 
   <td rowspan="2">Espace de travail</td> 
   <td>Créer</td> 
   <td>Workspace créé avec le nom "nom de l’espace de travail"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>"nom de l’espace de travail" espace de travail supprimé</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Filtrage dans le journal d’audit](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)
