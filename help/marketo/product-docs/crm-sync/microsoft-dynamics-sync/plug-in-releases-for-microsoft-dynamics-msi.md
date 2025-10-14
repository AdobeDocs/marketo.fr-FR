---
unique-page-id: 10099102
description: Versions des plug-ins pour  [!DNL Microsoft Dynamics] MSI - Documents Marketo - Documentation du produit
title: Versions des plug-ins pour [!DNL Microsoft Dynamics] MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 1%

---

# Versions de plug-in pour [!DNL Microsoft Dynamics] MSI {#plug-in-releases-for-microsoft-dynamics-msi}

Lors de la première synchronisation avec [!DNL Microsoft Dynamics], vous téléchargez et installez la dernière version des plug-ins pour Marketo Sales Insight (MSI). Marketo met régulièrement à jour ces plug-ins afin que vous puissiez revenir au même endroit pour télécharger la nouvelle version.

Si vous utilisez la solution de synchronisation CRM native de Marketo pour [!DNL Dynamics], [téléchargez le dernier plug-in](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} correspondant à votre version [!DNL Dynamics]. Pour ceux qui disposent d’une synchronisation personnalisée et ont acheté Marketo Sales Insight, le package [&#x200B; est disponible ici](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>Ces versions fonctionnent pour les versions on-premise et en ligne d’[!DNL Dynamics].

## Mise à niveau de votre solution MSI {#upgrading-your-msi-solution}

1. Importez la dernière version de la solution _sur la version existante_ de votre CRM [!DNL Dynamics] en appuyant sur le bouton **[!UICONTROL Importer]** dans [!DNL Dynamics].

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Exemple : si votre CRM [!DNL Dynamics] dispose de la version 2.0.0.20 et que la dernière version est 2.0.0.21, vous devez importer la version __ over2.0.0.20.

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Sélectionnez **[!UICONTROL Phase de mise à niveau]** et **[!UICONTROL Maintenir les personnalisations]**, puis cliquez sur **[!UICONTROL Importer]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Après une importation réussie, vous verrez deux solutions MSI : MarketoSalesInsight et MarketoSalesInsight_Upgrade. Sélectionnez l’ancienne solution et cliquez sur Appliquer la mise à niveau de la solution.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

Et c&#39;est tout ! Après la mise à niveau, vous ne verrez qu&#39;une seule solution MSI.

## Mises à jour de version {#version-updates}

<table>
 <tbody>
  <tr>
   <th>Date de publication</th>
   <th>Version</th>
   <th>Notes</th>
  </tr>
  <tr>
   <td>02/14/24</td>
   <td>2.00.31</td>
   <td>Modifications apportées à la pagination sur l’activité web anonyme .
   <p>
   Chiffrez les informations de clé secrète à partir de la vue utilisateur. Le mot de passe doit être modifié après l’importation du nouveau package pour que le chiffrement s’effectue.</td>
  </tr>
  <tr>
   <td>10/18/23</td>
   <td>2.00.30</td>
   <td>La consolidation du journal des erreurs MSI et la suppression des notifications d’informations s’affichent sur l’entité d’erreur Marketo.</td>
  </tr>
  <tr>
   <td>05/19/23</td>
   <td>2.00.29</td>
   <td>Correction des problèmes de pagination des activités web et des moments significatifs dans le tableau de bord global.</td>
  </tr>
  <tr>
   <td>03/23/23</td>
   <td>2.00.28</td>
   <td>Création d’un <a href="https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip">nouveau package</a> pour MSI pour les connexions non natives au CRM.</td>
  </tr>
  <tr>
   <td>02/03/22</td>
   <td>2.0.0.27</td>
   <td>Mise en page du compte pour les informations : moments significatifs, modifications du score, activités web, activités e-mail.</td>
  </tr>
  <tr>
   <td>01/05/22</td>
   <td>2.0.0.26</td>
   <td>Score d’adoption du programme pour l’envoi d’e-mail.</td>
  </tr>
  <tr>
   <td>10/28/21</td>
   <td>2.0.0.25</td>
   <td>Mesures de score d’adoption du produit, nouveau tableau de bord global (activité web, e-mail, meilleurs résultats).</td>
  </tr>
  <tr>
   <td>02/10/21</td>
   <td>2.0.0.22</td>
   <td>Supprimez l'audit automatique activé et les modifications de la documentation sur la solution MSI.</td>
  </tr>
  <tr>
   <td>10/01/20</td>
   <td>2.0.0.21</td>
   <td>Correction de bug : attribution d’accès aux champs de configuration de l’API MSI pour les utilisateurs dotés du rôle Sales Insight.</td>
  </tr>
  <tr>
   <td>07/20/20</td>
   <td>2.0.0.20</td>
   <td>Correction de bug : ajout d’un message de validation pour les enregistrements non synchronisés.</td>
  </tr>
  <tr>
   <td>06/12/20</td>
   <td>2.0.0.19</td>
   <td>Correction de bug : pour masquer le mot de passe secret MSI sur la configuration de l’API MSD.</td>
  </tr>
  <tr>
   <td>05/26/20</td>
   <td>2.0.0.18</td>
   <td>Correction de bug : pour modifier la validation de l’ID de rôle MSI pour l’affichage des boutons MSI.</td>
  </tr>
  <tr>
   <td>05/21/20</td>
   <td>2.0.0.17</td>
   <td>Correction de bug : affichez le champ du propriétaire et rendez les champs non obligatoires.</td>
  </tr>
  <tr>
   <td>04/28/20</td>
   <td>2.0.0.16</td>
   <td>Correction de bug : suppression de la dépendance des liens du plan de site CRM MSD.</td>
  </tr>
 </tbody>
</table>
