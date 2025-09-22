---
unique-page-id: 11379928
description: Modifier les détails dans Journal d’audit - Documents Marketo - Documentation du produit
title: Modifier des détails dans le journal d’audit
exl-id: 5583be62-46a6-42f9-b4b3-0df63a171b2d
feature: Audit Trail
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1902'
ht-degree: 15%

---

# Modifier des détails dans le journal d’audit {#change-details-in-audit-trail}

Le journal d&#39;audit offre beaucoup d&#39;insight pour savoir qui fait quoi dans votre abonnement Marketo. Voici les détails.

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
   <td>Type de canal « type de canal »<br>ou <br> cloné à partir de « nom du programme »</td>
  </tr>
  <tr>
   <td>Renommer</td>
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Cloné dans l’espace de travail « nom de l’espace de travail » <br>emplacement « dossier de campagne » ou « programme d’engagement » <br>nom du programme cloné « nouveau nom »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Modifier le canal</td>
   <td>Nouveau canal « nouveau nom du canal » Ancien canal « ancien nom du canal » </td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Ajoutez la valeur du jeton « nom du jeton » et la valeur du jeton « valeur du jeton ».</td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Modifier le jeton « nom du jeton » nouvelle valeur « nouvelle valeur » ancienne valeur « ancienne valeur »</td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Supprimer le jeton « nom du jeton »</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Ajout d’un « nom de comportement » de comportement Analytics</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td><p>Modifier le « nom du comportement » du comportement d’Analytics</p><p>Ancien comportement : « nom du comportement »</p></td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Supprimer le comportement d’analyse « nom du comportement »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Ajouter la valeur de coût de la période « # » au mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Modifier le coût de la période Nouvelle valeur de coût « # », Nouveau mois de programme « aaaa-mm », Ancienne valeur de coût « # », Ancien mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Supprimer le coût par période. Valeur « # » du mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td>Exporter</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td rowspan="19"><strong>E-mail</strong><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td>
   <td>Créer</td>
   <td>Créé à l’aide du modèle « nom du modèle » <br>ou <br>Cloné à partir du « nom de la ressource »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Mise à jour de « Nom de l’expéditeur » en « nouveau nom d’expéditeur »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Mise à jour de « De l’e-mail » vers « newemail@name.com »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Mise à jour de « Répondre à » en « newreplytoemail@name.com »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Mise à jour de « Subject » vers « new subject line »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Ajout de la segmentation « segmentation_name »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Segmentation supprimée</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Ajout du fragment de code « nom_fragment »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Extrait supprimé</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Modifie l’e-mail rompu du modèle « template_name » (REMARQUE : cela se produit aujourd’hui si vous modifiez directement le code).</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Nouvelle description « nouvelle description » Ancienne description « ancienne description »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Modifier le module <code>"&lt;module name&gt;" &lt;attribute&gt;</code> en « valeur »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Renommer</td>
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Cloné dans « Design Studio » dans le dossier « foldername » <br>Nom de la ressource clonée « name »<br>ou<br>Cloné dans « Activités marketing » dans le programme « nom du programme »<br>Nom de la ressource clonée « name »</td>
  </tr>
  <tr>
   <td>Déplacer</td>
   <td>Déplacé vers « Design Studio » dans le dossier « nom du dossier »<br>ou <br> Déplacé vers « Activités marketing » dans le programme « nom du programme »</td>
  </tr>
  <tr>
   <td>Approuver</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Annuler l'approbation</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Brouillon</td>
   <td>L’e-mail a été brouillé car le fragment de code « nom du fragment de code » a été approuvé<br>ou l<br>e-mail a été brouillé car le modèle « nom du modèle » a été approuvé</td>
  </tr>
   <td rowspan="17">Programme d’e-mail</td>
   <td>Créer</td>
   <td>Type de canal « type de canal »<br>ou <br> cloné à partir de « nom du programme »</td>
  </tr>
  <tr>
   <td colspan="1">Renommer</td>
   <td colspan="1">Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Cloné dans l’espace de travail « nom de l’espace de travail » <br>Emplacement « Dossier de campagne ou programme d’engagement » <br>Nom du programme cloné « nouveau nom »</td>
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
   <td>Nouveau canal « nouveau canal » Ancien canal « ancien canal »</td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Ajoutez la valeur du jeton « nom du jeton » et la valeur du jeton « valeur du jeton ».</td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Modifier le jeton « nom du jeton » Nouvelle valeur « nouvelle valeur » ancienne valeur « ancienne valeur »</td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Supprimer le jeton « nom du jeton »</td>
  </tr>
  <tr>
   <td>Modifier le planning du programme</td>
   <td>Définir la planification pour qu’elle commence à « date de début, heure de début » et se termine à « date de fin, heure de fin »</td>
  </tr>
  <tr>
   <td>Modifier le planning du programme</td>
   <td>Horaire modifié en « nouvelle date, nouvelle heure »</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Ajout d’un « nom de comportement » de comportement Analytics</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Modifier le comportement d’Analytics « nom du comportement »<br>Ancien comportement « nom du comportement »</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Supprimer le comportement d’analyse « nom du comportement »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Ajouter la valeur de coût de la période « # » au mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Modifier le coût de la période Nouvelle valeur de coût « # », Nouveau mois de programme « aaaa-mm », Ancienne valeur de coût « # », Ancien mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Supprimer le coût par période. Valeur « # » du mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td rowspan="8">Modèle d’e-mail</td>
   <td>Créer</td>
   <td>Vierge ou cloné à partir du « nom du modèle »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Nouvelle description « nouvelle description », description précédente « description précédente »</td>
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
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Cloné sur « nom du dossier » <br> « nom » de la ressource clonée</td>
  </tr>
  <tr>
   <td>Approuver</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Annuler l'approbation</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td rowspan="23">Programme d’engagement</td>
   <td>Créer</td>
   <td>Type de canal « type de canal »<br> ou <br> cloné à partir de « nom du programme »</td>
  </tr>
  <tr>
   <td>Renommer</td>
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Cloné dans l’espace de travail « nom de l’espace de travail » <br>Emplacement « Dossier de campagne ou programme d’engagement » <br>Nom du programme cloné « nouveau nom »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Modifier le canal</td>
   <td>Nouveau canal « nouveau canal » Ancien canal « ancien canal »</td>
  </tr>
  <tr>
   <td>Modifier le flux du programme</td>
   <td><p>Ajouter un flux</p><p>Nom « name » Emplacement « # »</p></td>
  </tr>
  <tr>
   <td>Modifier le flux du programme</td>
   <td><p>Modifier le flux</p><p>Nouveau nom du flux : « nouveau nom » Ancien nom du flux : « ancien nom »</p><p>Nouvel emplacement : « nouveau # » Ancien emplacement : « ancien # »</p></td>
  </tr>
  <tr>
   <td>Modifier le flux du programme</td>
   <td>Supprimer le nom du flux « name »</td>
  </tr>
  <tr>
   <td>Modifier le flux du programme</td>
   <td>Ajouter du contenu<br>Nom du flux « nom du flux »<br>Type « E-mail » ou « Programme »<br>Nom « nom de l’e-mail » ou « nom du programme »<br>Nom de la campagne intelligente « nom de la campagne intelligente »</td>
  </tr>
  <tr>
   <td>Modifier le flux du programme</td>
   <td>Activer le contenu<br>Nom du flux « nom du flux »<br>Nom du contenu « nom de l’e-mail » ou « nom du programme »</td>
  </tr>
  <tr>
   <td>Modifier le flux du programme</td>
   <td>Désactiver le contenu<br>Nom du flux « nom du flux »<br>Nom du contenu « nom de l’e-mail » ou « nom du programme »</td>
  </tr>
  <tr>
   <td>Modifier le flux du programme</td>
   <td>Supprimer le contenu<br>Nom du flux « nom du flux »<br>Nom du contenu « nom de l’e-mail » ou « nom du programme »</td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Ajoutez la valeur du jeton « nom du jeton » et la valeur du jeton « valeur du jeton ».</td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Modifier le jeton « nom du jeton » Nouvelle valeur « nouvelle valeur » ancienne valeur « ancienne valeur »</td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Supprimer le jeton « nom du jeton »</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Ajout d’un « nom de comportement » de comportement Analytics</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Modifier le comportement d’Analytics « nom du comportement »<br>Ancien comportement « nom du comportement »</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Supprimer le comportement d’analyse « nom du comportement »</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Modifier le statut du programme. Nouvelle valeur « on/off » Ancienne valeur « off/on »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Ajouter la valeur de coût de la période « # » au mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Modifier le coût de la période Nouvelle valeur de coût « # », Nouveau mois de programme « aaaa-mm », Ancienne valeur de coût « # », Ancien mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Supprimer le coût par période. Valeur « # » du mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td>Exporter</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td rowspan="18">Programme d’événement</td>
   <td>Créer</td>
   <td>Type de canal « type de canal »<br>ou <br> cloné à partir de « nom du programme »</td>
  </tr>
  <tr>
   <td>Renommer</td>
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Cloné dans l’espace de travail « nom de l’espace de travail » <br>emplacement « dossier de campagne » ou « programme d’engagement » <br>nom du programme cloné « nouveau nom »</td>
  </tr>
  <tr>
   <td>Modifier le canal</td>
   <td>Nouveau canal « nouveau canal » Ancien canal « ancien canal » </td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Ajoutez la valeur du jeton « nom du jeton » et la valeur du jeton « valeur du jeton ».</td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Modifier le jeton « nom du jeton » Nouvelle valeur « nouvelle valeur » ancienne valeur « ancienne valeur »</td>
  </tr>
  <tr>
   <td>Modifier le jeton de programme</td>
   <td>Supprimer le jeton « nom du jeton »</td>
  </tr>
  <tr>
   <td>Modifier le planning du programme</td>
   <td>Définir la planification pour qu’elle commence à « date de début, heure de début » et se termine à « date de fin, heure de fin »</td>
  </tr>
  <tr>
   <td>Modifier le planning du programme</td>
   <td>Horaire modifié en « nouvelle date, nouvelle heure »</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Ajout d’un « nom de comportement » de comportement Analytics</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Modifier le comportement d’Analytics « nom du comportement »<br>Ancien comportement « nom du comportement »</td>
  </tr>
  <tr>
   <td>Modifier la configuration du programme</td>
   <td>Supprimer le comportement d’analyse « nom du comportement »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Ajouter la valeur de coût de la période « # » au mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Modifier le coût de la période Nouvelle valeur de coût « # », Nouveau mois de programme « aaaa-mm », Ancienne valeur de coût « # », Ancien mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Supprimer le coût par période. Valeur « # » du mois de programme « aaaa-mm »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier la configuration du programme</td>
   <td colspan="1">Ajout de la mention « nom_partenaire » du partenaire d’événement</td>
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
   <td>Jeton ajouté « token_name », valeur « value »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Jeton modifié « token_name » nouvelle valeur « token_value » ancienne valeur « old_token_value »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Jeton « token_name » supprimé</td>
  </tr>
  <tr>
   <td rowspan="8">Formulaires</td>
   <td>Créer</td>
   <td>Bientôt disponible. En savoir plus ou cloné à partir du « nom du formulaire »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Renommer</td>
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Nouvelle description « nouvelle description » Ancienne description « ancienne description »</td>
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
   <td>Cloné dans « Design Studio » dans le dossier « foldername » <br>Nom de la ressource clonée « name »<br>ou<br>Cloné dans « Activités marketing » dans le programme « nom du programme »<br>Nom de la ressource clonée « name »</td>
  </tr>
  <tr>
   <td>Déplacer</td>
   <td>Déplacé vers « Design Studio » dans le dossier « nom du dossier »<br>ou <br> Déplacé vers « Activités marketing » dans le programme « nom du programme »</td>
  </tr>
  <tr>
   <td>Formulaires</td>
   <td>Approuver</td>
   <td>Utilisé par # ressources </td>
  </tr>
  <tr>
   <td rowspan="9">Page de destination</td>
   <td>Créer</td>
   <td>Créé à l’aide du modèle « nom du modèle » <br>ou <br>Cloné à partir du « nom de la ressource »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Renommer</td>
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Nouvelle description « nouvelle description » Précédente « description précédente »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Ajout De « Image », Suppression De « Image » Et Modification Du Composant Image</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Ajout De « Texte Enrichi », Suppression De « Texte Enrichi » Et Modification Du Composant De Texte Enrichi</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Cloné dans « Design Studio » dans le dossier « foldername »<br>Nom de la ressource clonée « name »<br>URL de la ressource clonée « www.url.com »<br>ou<br>Cloné dans « Activités marketing » du programme « nom du programme » <br>Nom de la ressource clonée « name »<br>URL de la ressource clonée « www.url.com »</td>
  </tr>
  <tr>
   <td>Déplacer</td>
   <td>Déplacé vers « Design Studio » dans le dossier « folder name »<br> ou <br> Déplacé vers « Activités marketing » dans le programme « program name »</td>
  </tr>
  <tr>
   <td>Approuver</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Brouillon</td>
   <td>La page de destination a été brouillée car le modèle « nom du modèle » a été approuvé.</td>
  </tr>
  <tr>
   <td>Annuler l'approbation</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td rowspan="8">Modèle de page de destination</td>
   <td>Créer</td>
   <td><p>Vide<br>ou <br> cloné à partir du « nom de la ressource »</p></td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Renommer</td>
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Nouvelle description « nouvelle description » description précédente « description précédente »</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Cloné sur « nom du dossier » <br>nom de la ressource clonée « nom »</td>
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
   <td>Annuler l'approbation</td>
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
   <td>Clonage de la « base de données des personnes » dans le dossier « nom du dossier » <br>Clonage du nom de la ressource « nom »<br>ou<br>Clonage de la base de données des personnes en « activités marketing » dans le programme « nom du programme »<br>Clonage du nom de la ressource « nom »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Renommer</td>
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
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
   <td>Déplacé vers « Programmes » dans le programme « nom du programme »<br>ou <br> Déplacé vers « Dossiers » dans le dossier « nom du dossier »</td>
  </tr>
  <tr>
   <td>Renommer</td>
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Nouvelle description « nouvelle description » Précédente « description précédente »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Cloné sur « Programmes » dans le programme « nom du programme » <br>Nom de la ressource clonée « nom »<br>ou <br> Cloné sur « Dossier » dans le dossier « nom du dossier »<br>Nom de la ressource clonée « nom »</td>
  </tr>
  <tr>
   <td>Modifier le paramétrage de la liste dynamique</td>
   <td>Affiche un instantané du statut actuel, y compris les noms et valeurs des filtres et des déclencheurs</td>
  </tr>
  <tr>
   <td>Modifier le planning de la campagne</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Action Modifier l’étape de flux</td>
   <td>Affiche un instantané de l’état actuel, y compris les noms et les valeurs de chaque étape de flux</td>
  </tr>
  <tr>
   <td rowspan="7">Liste intelligente</td>
   <td>Créer</td>
   <td>Cloné à partir du « nom de liste dynamique »</td>
  </tr>
  <tr>
   <td>Exporter</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Renommer</td>
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Nouvelle description « nouvelle description » Précédente « description précédente »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>S/O</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Clonage de la « base de données des personnes » dans le dossier « nom du dossier » <br>Clonage du nom de la ressource « nom »<br> ou <br> Clonage de la « base de données des personnes » dans le programme « nom du programme » <br>Clonage du nom de la ressource « nom »</td>
  </tr>
  <tr>
   <td>Modifier le paramétrage de la liste dynamique</td>
   <td>Affiche un instantané du statut actuel, y compris les noms et valeurs des filtres et des déclencheurs </td>
  </tr>
  <tr>
   <td rowspan="11">Extrait</td>
   <td>Créer</td>
   <td><p>Vide<br>ou <br> cloné à partir du « nom du fragment de code »</p></td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Ajout de la segmentation « segmentation_name »</td>
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
   <td>Nouveau nom « nouveau nom », nom précédent « nom précédent »</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Nouvelle description « nouvelle description » Précédente « description précédente »</td>
  </tr>
  <tr>
   <td>Cloner</td>
   <td>Cloné sur « nom du dossier » <br>nom du fragment de code cloné « nom »</td>
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
   <td>Annuler l'approbation</td>
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
   <td>Restrictions IP modifiées comme suit : « bloc » autorisé/bloqué, adresse IP « # », restrictions IP désactivées « »</td>
  </tr>
  <tr>
   <td rowspan="2">Division</td>
   <td>Créer</td>
   <td>Partition créée avec le nom « partition name »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>partition « nom de la partition » supprimée</td>
  </tr>
  <tr>
   <td>Niveau de sécurité du mot de passe</td>
   <td>Modifier</td>
   <td>Sécurité du mot de passe remplacée par le modèle : Sécurité standard, longueur minimale : #, valeur inférieure-supérieure : #, nombre : #, casse mixte : # , expiration : #, délai d’expiration de la session : #</td>
  </tr>
  <tr>
   <td rowspan="3">Rôle<br><br></td>
   <td>Créer</td>
   <td>Rôle créé avec « nom du rôle » (REMARQUE : si vous avez besoin de détails sur les autorisations ajoutées, veuillez contacter le support) - <br>affiche un instantané des autorisations attribuées au rôle</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>Le rôle « Nom du rôle » a été supprimé.</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>Rôle modifié de « nom précédent » en « nouveau nom » (REMARQUE : si vous avez besoin de détails sur les autorisations modifiées, veuillez contacter le support) - <br>affiche un instantané des autorisations attribuées au rôle<br></td>
  </tr>
  <tr>
   <td>Rapport des listes intelligentes</td>
   <td>Modifier</td>
   <td>SmartList modifié pour la connexion à télécharger : « true ou false »</td>
  </tr>
  <tr>
   <td rowspan="7">Utilisateur ou utilisatrice<br><br><br><br></td>
   <td>Créer (invitation)</td>
   <td>Utilisateur invité avec : adresse e-mail, nom, prénom et nom, l’accès expire « vide ou avec une date », utilisateur de l’API « true ou false » - <br> affiche un instantané des rôles et des espaces de travail affectés à l’utilisateur.</td>
  </tr>
  <tr>
   <td colspan="1">Supprimer</td>
   <td colspan="1">utilisateur « nom d’utilisateur » supprimé</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>L’utilisateur « ancien nom » a été renommé « nouveau nom » avec l’adresse e-mail : « e-mail », apiUser : l’accès « true ou false » expire : « vide ou avec une date ».</td>
  </tr>
  <tr>
   <td>Modifier</td>
   <td>L'utilisateur a été modifié pour l'e-mail : « email », apiUser : « true ou false », l'accès expire : « blank ou avec une date »</td>
  </tr>
  <tr>
   <td colspan="1">Modifier</td>
   <td colspan="1">Affiche un instantané du statut actuel, y compris les rôles et les espaces de travail affectés à l’utilisateur</td>
  </tr>
  <tr>
   <td>Problème</td>
   <td>Licence Calendrier délivrée à l’adresse e-mail : nom de l’utilisateur : nom de l’utilisateur</td>
  </tr>
  <tr>
   <td>Réinitialiser</td>
   <td>Réinitialisation du mot de passe pour le nom « name » et l’e-mail « email »</td>
  </tr>
  <tr>
   <td rowspan="2">Espace de travail</td>
   <td>Créer</td>
   <td>Workspace créé avec le nom « workspace name »</td>
  </tr>
  <tr>
   <td>Supprimer</td>
   <td>espace de travail « nom de l’espace de travail » supprimé</td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[Filtrage dans le journal d&#39;audit](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)
