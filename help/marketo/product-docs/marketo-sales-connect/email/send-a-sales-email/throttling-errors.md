---
unique-page-id: 14352581
description: Erreurs de limitation - Docs marketing - Documentation du produit
title: Erreurs de limitation
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# Erreurs de limitation {#throttling-errors}

## Limite de fichier atteinte {#file-limit-reached}

Si vous envoyez par l&#39;intermédiaire de votre propre serveur, le nombre de courriers électroniques que vous pouvez envoyer simultanément sera limité. Lors de l&#39;envoi via Sales Connect, vous avez la possibilité d&#39;envoyer de nombreux e-mails, mais nous essayons de les envoyer tous en même temps. Ainsi, si vous savez que votre serveur va vous couper 100 courriels par minute, vous n&#39;aurez qu&#39;à envoyer jusqu&#39;à 100 courriels par le biais de l&#39;[application Web](http://toutapp.com/login). Dans le cas contraire, les courriels peuvent arriver ici en raison du ralentissement des courriels sur votre serveur.

## Erreur d&#39;authentification {#authentication-error}

Cela signifie que nous n’avons pas pu authentifier la connexion à votre serveur SMTP. Il est probable que votre mot de passe a été modifié récemment et que vous devez simplement authentifier vos nouvelles informations d’identification.

Pour ce faire, accédez à vos [Paramètres SMTP](http://docs.marketo.com/display/docs/assets/external-link-1.jspa) `where you should see the same error message. Update your credentials and hit **Authenticate and Save** to see a confirmation message.`

Accédez à vos Diffusions en échec pour essayer de renvoyer ces courriers électroniques.
