---
unique-page-id: 11387674
description: Mises à jour de la terminologie de Marketo - Documents marketing - Documentation du produit
title: Mises à jour de la terminologie du marketing
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---


# Mises à jour de la terminologie du marketing {#updates-to-marketo-terminology}

Nous apportons des changements à notre plateforme, ce qui va affecter ce que certains éléments appellent. Si vous disposez d’une nouvelle instance de Marketo à compter de mars 2016 ou si votre société a été renouvelée après juillet 2016, il se peut que la nouvelle terminologie s’affiche maintenant.

Bien que la terminologie de la documentation de Marketo puisse être différente, soyez assuré que chaque article sera bientôt mis à jour pour refléter ces modifications. Toutes les instructions sont les mêmes.

Alors, qu&#39;est-ce qui a changé ?

## Le prospect est maintenant une personne {#lead-is-now-person}

Le changement le plus important est le changement de nom de piste/pistes vers personne/personnes.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Vieux</strong></td> 
   <td><strong>Nouveau</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img width="295" src="assets/leads.png" data-linked-resource-id="11387678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img width="295" src="assets/people.png" data-linked-resource-id="11387679" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Dans certains cas, le mot &quot;plomb&quot; est simplement supprimé.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Vieux</strong></td> 
   <td><strong>Nouveau</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-database.png" data-linked-resource-id="11387676" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <p><img src="assets/database.png" data-linked-resource-id="11387677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"></p> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Le plomb et la personne **sont la même chose**.

## Jetons {#tokens}

Les jetons contenant le mot &quot;plomb&quot; ne **changent** pas. Nous nous excusons pour toute confusion ; toutefois, modifier tous les jetons pour qu&#39;ils correspondent à la nouvelle terminologie briserait un grand nombre de jetons actuellement utilisés. Vous verrez donc toujours des jetons tels que &quot;`{{lead.First Name}}`&quot;. Il n&#39;existe pas de jetons spécifiques à une personne.

>[!NOTE]
>
>Il *existe* un jeton appelé &quot;Notes personnelles&quot;, mais ce jeton était toujours présent. Il est généralement utilisé pour un champ de description dans votre gestion de la relation client, le cas échéant.

## Gestion de terrain {#field-management}

Les champs qui contenaient le terme Piste ont été remplacés par Personne ou le mot Piste a été supprimé. Le champ &quot;Propriétaire de la piste&quot; constitue toutefois une exception notable. Il est désormais connu sous le nom de &quot;Propriétaire de la vente&quot;.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Vieux</strong></td> 
   <td><strong>Nouveau</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-owner.png" data-linked-resource-id="11387757" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/sales-owner.png" data-linked-resource-id="11387758" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Pour une liste complète des noms de champs concernés, veuillez visiter cet article [](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens)d&#39;assistance.

## La personnalisation en temps réel (RTP) est désormais la personnalisation Web {#real-time-personalization-rtp-is-now-web-personalization}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Vieux</strong></td> 
   <td><strong>Nouveau</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/rtp.png" data-linked-resource-id="11387692" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/web.png" data-linked-resource-id="11387693" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Outre le changement de nom, il comprend désormais quatre applications distinctes :

| ** Personnalisation [](http://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP)Web** | Dispose de sa propre mosaïque sur l’écran d’accueil |
|---|---|
| ** Marketing [Web basé sur](http://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing)le compte** | Accessible via la mosaïque Personnalisation Web |
| ** [Ciblage](http://docs.marketo.com/display/DOCS/Website+Retargeting)personnalisé** | Accessible via la mosaïque Personnalisation Web |
| ** Contenu [](http://docs.marketo.com/display/DOCS/Predictive+Content)prédictif** | Dispose de sa propre mosaïque sur l’écran d’accueil |

>[!NOTE]
>
>Les mosaïques visibles sur votre écran d’accueil reflètent les modules achetés.

Merci pour votre patience durant cette mise à jour.
