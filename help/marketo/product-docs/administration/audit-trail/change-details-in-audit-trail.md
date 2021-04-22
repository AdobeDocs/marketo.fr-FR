---
unique-page-id: 11379928
description: Détails des modifications dans la piste d’audit - Documentation Marketo - Documentation du produit
title: Modifier les détails dans la piste d’audit
exl-id: 5583be62-46a6-42f9-b4b3-0df63a171b2d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1913'
ht-degree: 14%

---

# Détails des modifications dans la piste d&#39;audit {#change-details-in-audit-trail}

Les offres de la piste d&#39;audit fournissent beaucoup d&#39;informations sur qui fait quoi dans votre abonnement Marketo. Voici les détails.

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
   <td>Type de canal "canal type"<br>ou<br>Cloné à partir de "programme name"</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur l’espace de travail "nom de l’espace de travail" <br>Emplacement "dossier Campaign" ou "programme d’engagement" <br>Nom du programme cloné "nouveau nom"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Modifier canal</td> 
   <td>Nouveau canal "nouveau nom du canal" Ancien canal "ancien nom du canal" </td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Jeton Ajouté "nom du jeton" valeur "valeur du jeton"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Modifier le jeton "nom du jeton" nouvelle valeur "nouvelle valeur" ancienne valeur "ancienne valeur"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Supprimer le jeton "nom du jeton"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Ajouter le comportement d'analyse "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td><p>Modifier le comportement d'analyse "nom du comportement"</p><p>Ancien comportement "nom du comportement"</p></td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Supprimer le comportement d'analyse "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Valeur de coût de la période de Ajoute "#" mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Coût de la période de modification Nouvelle valeur de coût "#", Nouveau mois de programme "aaaa-mm", Ancienne valeur de coût "#", Ancien mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Supprimer le coût par période. Valeur "#" programme mois "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td>Exporter</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td rowspan="19"><strong>E-mails</strong><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>Créer</td> 
   <td>Créé à l’aide du modèle "nom du modèle" <br>ou <br>cloné à partir de "nom du fichier"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Mise à jour de "From Name" en "new from name"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Mise à jour de "From Email" en "newemail@name.com"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Mise à jour de "Répondre à" en "newreplytoemail@name.com"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Mise à jour de "Objet" sur "nouvelle ligne d’objet"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Segmentation Ajoutée "segmentation_name"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Segmentation supprimée</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>extrait de code Ajouté "snippet_name"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Extrait supprimé</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Les modifications ont rompu le courrier électronique du modèle "template_name" (REMARQUE : ceci se produit aujourd’hui si vous modifiez directement le code)</td> 
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
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "Design Studio" dans le dossier "nom du dossier" <br>Nom du fichier cloné "nom"<br>ou<br>Cloné sur "Activités marketing" dans le programme "nom du programme"<br>Nom du fichier cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Déplacer</td> 
   <td>Déplacé vers "Design Studio" dans le dossier "folder name"<br>ou<br>Déplacé vers "Marketing activités" dans le programme "programme name"</td> 
  </tr> 
  <tr> 
   <td>Approuver</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Désapprouver</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Brouillon</td> 
   <td>Le courrier électronique a été rédigé car le fragment de code "nom du fragment de code" a été approuvé<br>ou<br>Le courrier électronique a été rédigé car le modèle "nom du modèle" a été approuvé.</td> 
  </tr> 
   <td rowspan="17">Programme de courriel</td> 
   <td>Créer</td> 
   <td>Type de canal "canal type"<br>ou<br>Cloné à partir de "programme name"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Renommer</td> 
   <td colspan="1">Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur l’espace de travail "nom de l’espace de travail" <br>Emplacement "dossier Campaign ou programme d’engagement" <br>Nom du programme cloné "nouveau nom"</td> 
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
   <td>Modifier canal</td> 
   <td>Nouveau canal "nouveau canal" Ancien canal "ancien canal"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Jeton Ajouté "nom du jeton" valeur "valeur du jeton"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Modifier le jeton "nom du jeton" Nouvelle valeur "nouvelle valeur" ancienne valeur "ancienne valeur"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Supprimer le jeton "nom du jeton"</td> 
  </tr> 
  <tr> 
   <td>Modifier le Planning du programme</td> 
   <td>Définissez la planification sur début le "début date, début time" et se termine par "end date, end time".</td> 
  </tr> 
  <tr> 
   <td>Modifier le Planning du programme</td> 
   <td>Modification de la planification en "nouvelle date, nouvelle heure"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Ajouter le comportement d'analyse "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Modifier le comportement d'analyse "nom du comportement"<br>Ancien comportement "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Supprimer le comportement d'analyse "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Valeur de coût de la période de Ajoute "#" mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Coût de la période de modification Nouvelle valeur de coût "#", Nouveau mois de programme "aaaa-mm", Ancienne valeur de coût "#", Ancien mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Supprimer le coût par période. Valeur "#" programme mois "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Modèle d’e-mail</td> 
   <td>Créer</td> 
   <td>Vierge ou clonée à partir du "nom du modèle"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description", description précédente "description précédente"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Modification HTML</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "nom du dossier" <br> Nom de fichier cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Approuver</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Désapprouver</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td rowspan="23">Programmes d'engagement</td> 
   <td>Créer</td> 
   <td>Type de canal "canal type"<br> ou <br> Cloné à partir de "programme name"</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur l’espace de travail "nom de l’espace de travail" <br>Emplacement "dossier Campaign ou programme d’engagement" <br>Nom du programme cloné "nouveau nom"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Modifier canal</td> 
   <td>Nouveau canal "nouveau canal" Ancien canal "ancien canal"</td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td><p>Ajouter un stream</p><p>Nom "name" Placement "#"</p></td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td><p>Modifier le stream</p><p>Nouveau nom du flux : "nouveau nom" Ancien nom du flux : "ancien nom"</p><p>Nouvel emplacement : "new #" Ancien emplacement : "old #"</p></td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td>Supprimer le nom de flux "name"</td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td>Contenu Ajouté<br>Nom de flux<br>Type "Adresse électronique" ou "Programme"<br>Nom "nom de courriel" ou "nom de programme"<br>Smart Campaign "nom de campagne intelligent"</td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td>Activez le contenu <br>Nom du flux "nom du flux"<br>Nom du contenu "nom de courriel" ou "nom du programme".</td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td>Désactiver le contenu <br>Nom du flux "nom du flux"<br>Nom du contenu "nom de courriel" ou "nom du programme"</td> 
  </tr> 
  <tr> 
   <td>Modification du flux de programme</td> 
   <td>Supprimer le contenu <br>nom du flux "nom du flux"<br>nom du contenu "nom de l’adresse électronique" ou "nom du programme"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Jeton Ajouté "nom du jeton" valeur "valeur du jeton"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Modifier le jeton "nom du jeton" Nouvelle valeur "nouvelle valeur" ancienne valeur "ancienne valeur"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Supprimer le jeton "nom du jeton"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Ajouter le comportement d'analyse "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Modifier le comportement d'analyse "nom du comportement"<br>Ancien comportement "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Supprimer le comportement d'analyse "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Modifier le statut du programme. Nouvelle valeur "on/off" Ancienne valeur "off/on"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Valeur de coût de la période de Ajoute "#" mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Coût de la période de modification Nouvelle valeur de coût "#", Nouveau mois de programme "aaaa-mm", Ancienne valeur de coût "#", Ancien mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Supprimer le coût par période. Valeur "#" programme mois "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td>Exporter</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td rowspan="18">Programme événement</td> 
   <td>Créer</td> 
   <td>Type de canal "canal type"<br>ou<br>Cloné à partir de "programme name"</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
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
   <td>Modifier canal</td> 
   <td>Nouveau canal "nouveau canal" Ancien canal "ancien canal" </td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Jeton Ajouté "nom du jeton" valeur "valeur du jeton"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Modifier le jeton "nom du jeton" Nouvelle valeur "nouvelle valeur" ancienne valeur "ancienne valeur"</td> 
  </tr> 
  <tr> 
   <td>Modifier le jeton de programme</td> 
   <td>Supprimer le jeton "nom du jeton"</td> 
  </tr> 
  <tr> 
   <td>Modifier le Planning du programme</td> 
   <td>Définissez la planification sur début le "début date, début time" et se termine par "end date, end time".</td> 
  </tr> 
  <tr> 
   <td>Modifier le Planning du programme</td> 
   <td>Modification de la planification en "nouvelle date, nouvelle heure"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Ajouter le comportement d'analyse "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Modifier le comportement d'analyse "nom du comportement"<br>Ancien comportement "nom du comportement"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des programmes</td> 
   <td>Supprimer "nom du comportement" du comportement d'analyse</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Valeur de coût de la période de Ajoute "#" mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Coût de la période de modification Nouvelle valeur de coût "#", Nouveau mois de programme "aaaa-mm", Ancienne valeur de coût "#", Ancien mois de programme "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Supprimer le coût par période. Valeur "#" programme mois "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modification de la configuration des programmes</td> 
   <td colspan="1">Partenaire de événement Ajouté "partner_name"</td> 
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
   <td>Jeton Ajouté "token_name", valeur "value"</td> 
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
   <td>Bientôt disponible. En savoir plus ou Cloné à partir du "nom du formulaire"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
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
   <td>Cloné sur "Design Studio" dans le dossier "nom du dossier" <br>Nom du fichier cloné "nom"<br>ou<br>Cloné sur "Activités marketing" dans le programme "nom du programme"<br>Nom du fichier cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Déplacer</td> 
   <td>Déplacé vers "Design Studio" dans le dossier "folder name"<br>ou<br>Déplacé vers "Marketing activités" dans le programme "programme name"</td> 
  </tr> 
  <tr> 
   <td>Formulaires</td> 
   <td>Approuver</td> 
   <td>Utilisé par # les ressources </td> 
  </tr> 
  <tr> 
   <td rowspan="9">Landing page</td> 
   <td>Créer</td> 
   <td>Créé à l’aide du modèle "nom du modèle" <br>ou <br>cloné à partir de "nom du fichier"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" Précédente "précédente description"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>"Image" Ajoutée, "Image" supprimée, composant Image modifié</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>"Texte enrichi" Ajouté, "Texte enrichi" supprimé, Composant Texte enrichi modifié</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "Design Studio" dans le dossier "nom du dossier"<br>Nom de la ressource clonée "nom"<br>URL de la ressource clonée "www.url.com"<br>ou<br>Cloné sur "Activités marketing" dans le programme "nom du programme" <br>Nom de la ressource clonée "nom"<br>URL de la ressource clonée "www.url.com"</td> 
  </tr> 
  <tr> 
   <td>Déplacer</td> 
   <td>Déplacé vers "Design Studio" dans le dossier "folder name"<br> ou <br> Déplacé vers "Marketing activités" dans le programme "programme name"</td> 
  </tr> 
  <tr> 
   <td>Approuver</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Brouillon</td> 
   <td>Le landing page a été rédigé car le modèle "nom du modèle" a été approuvé</td> 
  </tr> 
  <tr> 
   <td>Désapprouver</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Modèle de page de destination</td> 
   <td>Créer</td> 
   <td><p>Vierge<br>ou<br>cloné à partir de "nom de fichier"</p></td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" description précédente "description précédente"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "nom du dossier" <br>Nom de fichier cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Exporter</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Approuver</td> 
   <td>Utilisé par # les ressources </td> 
  </tr> 
  <tr> 
   <td>Désapprouver</td> 
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
   <td>Cloné sur "Base de données des personnes" dans le dossier "nom du dossier" <br>Nom du fichier cloné "nom"<br>ou<br>Cloné sur "Activités marketing" dans le programme "nom du programme"<br>Nom du fichier cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
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
   <td>Déplacé vers "Programmes" dans le programme "programme name"<br>ou<br>Déplacé vers "Folders" dans le dossier "folder name"</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" Précédente "précédente description"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné en "Programmes" dans le programme "nom du programme" <br>Nom de la ressource clonée "nom"<br>ou<br>Cloné en "dossier" dans le dossier "nom du dossier"<br>Nom de la ressource clonée "nom"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des smartlist</td> 
   <td>Affiche un instantané de l’état actuel, y compris les noms et valeurs des filtres et déclencheurs.</td> 
  </tr> 
  <tr> 
   <td>Modifier le calendrier de campagne</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Modifier l’action de l’étape de flux</td> 
   <td>Affiche un instantané de l’état actuel, y compris les noms et les valeurs de chaque étape de flux.</td> 
  </tr> 
  <tr> 
   <td rowspan="7">Liste intelligente</td> 
   <td>Créer</td> 
   <td>Cloné à partir du "nom de la liste intelligente"</td> 
  </tr> 
  <tr> 
   <td>Exporter</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Renommer</td> 
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" Précédente "précédente description"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "Base de données des personnes" dans le dossier "nom du dossier" <br>Nom du fichier cloné "nom"<br>ou<br>Cloné sur "Activités marketing" dans le programme "nom du programme" <br>Nom du fichier cloné "nom"</td> 
  </tr> 
  <tr> 
   <td>Modification de la configuration des smartlist</td> 
   <td>Affiche un instantané de l’état actuel, y compris les noms et valeurs des filtres et déclencheurs. </td> 
  </tr> 
  <tr> 
   <td rowspan="11">Extrait</td> 
   <td>Créer</td> 
   <td><p>Vierge<br>ou<br>cloné à partir du "nom de fragment de code"</p></td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Segmentation Ajoutée "segmentation_name"</td> 
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
   <td>Nouveau nom "nouveau nom", prénom "nom précédent"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Nouvelle description "nouvelle description" Précédente "précédente description"</td> 
  </tr> 
  <tr> 
   <td>Cloner</td> 
   <td>Cloné sur "nom du dossier" <br>Nom du fragment de code "nom"</td> 
  </tr> 
  <tr> 
   <td>Approuver</td> 
   <td>Utilisé par # les ressources</td> 
  </tr> 
  <tr> 
   <td>Approuver sans brouillon</td> 
   <td>S/O</td> 
  </tr> 
  <tr> 
   <td>Désapprouver</td> 
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
   <td>Modification des restrictions d’adresse IP aux suivantes : "Bloc" autorisé/bloqué, adresse IP "#", Restrictions IP désactivées ""</td> 
  </tr> 
  <tr> 
   <td rowspan="2">Division</td> 
   <td>Créer</td> 
   <td>Partition créée avec le nom "partition name"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>partition "nom de la partition" supprimée</td> 
  </tr> 
  <tr> 
   <td>Niveau de sécurité du mot de passe</td> 
   <td>Modifier</td> 
   <td>La sécurité du mot de passe a été remplacée par le modèle : Sécurité standard, longueur minimale : #, inférieur supérieur : #, number : #, casse mixte : #, expiration : #, expiration de session : #</td> 
  </tr> 
  <tr> 
   <td rowspan="3">Rôle<br><br></td> 
   <td>Créer</td> 
   <td>Rôle créé avec "nom du rôle" (REMARQUE : si vous avez besoin de détails sur les autorisations ajoutées, contactez l'assistance) - <br>affiche un instantané des autorisations attribuées au rôle</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>Le rôle "Nom du rôle" a été supprimé.</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>Rôle Modifié de "nom précédent" en "nouveau nom" (REMARQUE : si vous avez besoin de détails sur les autorisations modifiées, contactez l'assistance) - <br>affiche un instantané des autorisations attribuées au rôle<br></td> 
  </tr> 
  <tr> 
   <td>Rapport des listes intelligentes</td> 
   <td>Modifier</td> 
   <td>SmarList modifié pour la connexion à télécharger : "true" ou "false"</td> 
  </tr> 
  <tr> 
   <td rowspan="7">Utilisateur<br><br><br><br></td> 
   <td>Créer (inviter)</td> 
   <td>Invité par l'utilisateur avec : Adresse électronique, Nom "prénom et nom", Access expire "vide ou avec une date", Utilisateur de l'API "vrai ou faux" - <br>affiche un instantané des rôles et espaces de travail attribués à l'utilisateur</td> 
  </tr> 
  <tr> 
   <td colspan="1">Supprimer</td> 
   <td colspan="1">"nom d'utilisateur" utilisateur supprimé</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>L’utilisateur a été renommé "ancien nom" en "nouveau nom" par courrier électronique : "email", apiUser: L’accès "vrai ou faux" expire : "vide ou avec une date"</td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>L’utilisateur a été modifié pour le courrier électronique : "email", apiUser: "true ou false", l’accès expire : "vide ou avec une date"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifier</td> 
   <td colspan="1">Affiche un instantané de l’état actuel, y compris les rôles et espaces de travail attribués à l’utilisateur.</td> 
  </tr> 
  <tr> 
   <td>Problème</td> 
   <td>Licence de calendrier délivrée à l'adresse électronique : nom du "courrier électronique de l’utilisateur" : "nom d’utilisateur"</td> 
  </tr> 
  <tr> 
   <td>Réinitialiser</td> 
   <td>Réinitialisation du mot de passe pour le nom "name" et l’adresse électronique "email"</td> 
  </tr> 
  <tr> 
   <td rowspan="2">Espace de travail</td> 
   <td>Créer</td> 
   <td>Espace de travail créé avec le nom "nom de l’espace de travail"</td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>Espace de travail supprimé</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Filtrage dans la piste d’audit](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)
