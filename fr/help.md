---
title: FAQ
lang: fr
render_toc: true
header: Foire aux questions
---


## Qu'est-ce que Delta Chat ?

Delta Chat est une application de clavardage qui utilise le courrier électronique pour délivrer ses messages et les chiffre avec Autocrypt lorsque c'est possible.
**Vous n'avez pas besoin de vous créer un nouveau compte, vous pouvez simplement utiliser votre compte courriel existant avec Delta Chat.**

<img style="float:right; width:50%; max-width:360%; margin:1em;" src="../assets/home/delta-what-optim.png" />


### Comment puis-je trouver des gens avec qui discuter ?

Avec Delta Chat, vous pouvez écrire à toutes les adresses courriels existantes, même si le destinataire n'utilise pas l'application. Votre correspondant pourra simplement répondre au courriel qu'il aura reçu. Contrairement aux autres messageries instantanées, il n'est pas nécessaire que vos amis installent le même client pour discuter avec vous.


### Quels sont les avantages de Delta Chat par rapport aux autres messageries ?

- _Independent_ of any company or services. _You_ own your data.
- Your data is not saved on a central server unless all users are using
  the same e-mail servers
- You do not distribute your address book to anyone.
- _Fast_ by the use of Push-IMAP.
- _Largest userbase_ - recipients _not_ using Delta Chat can be reached as well.
- _No Spam_ - only messages of known users are shown by default.
- _End-to-end encryption_ via Autocrypt.
- _Copyleft_ and _Standards_ based libre software.
- _Flexible identity_ with built-in support for [multiple accounts](#multiple-accounts)


### Quels sont les messages qui apparaissent dans Delta Chat ?

Par défaut, Delta Chat affiche tous les courriels.

Vous pouvez changer cette préférence en vous rendant dans vos "Paramètres -> Discussions & fichiers multimédia -> Voir les courriels classiques". Trois options sont disponibles :

- "Non, seulement les discussions": vous verrez seulement les messages envoyés par d'autres utilisateurs de Delta Chat et les réponses à vos messages Delta Chat. Cette option est recommandée si vous utilisez le même compte pour recevoir aussi des courriels normaux.
- "Tout": vous verrez dans Delta Chat tous les courriels envoyés à votre adresse. Cette option est recommandée si vous souhaitez utiliser Delta Chat pour tous vos courriels, afin de ne rater aucun message.
- "Pour les contacts acceptés": vous verrez dans Delta Chat tous les courriels envoyés par les personnes avec qui vous avez déjà ouvert une discussion, mais les notifications de nouvelles conversations ne s'afficheront que pour des messages envoyés via Delta Chat. Cette option vous permet de décider au cas par cas si vous souhaitez échanger via Delta Chat ou via une application de courriel "classique".


### Et si j'attends un message de quelqu'un avec qui je n'ai encore jamais échangé ?

- Si vous recevez un message de la part d'un contact inconnu, vous recevez une **invitation** que vous
  devez d'abord accepter pour pouvoir répondre au message.
- Vous pouvez également choisir de "supprimer" l'invitation si vous ne souhaitez pas discuter avec cet inconnu maintenant. Cela
  ne supprime *pas* le message sur le serveur, seulement sur votre appareil. Vous pouvez donc
  toujours traiter le message depuis une application de courriel différente.
- Si vous supprimez une invitation, les futurs messages de ce contact apparaîtront
  de nouveau comme des invitations, de sorte que vous pouvez changer d'avis par la suite. Si vous ne voulez vraiment pas
  recevoir de messages de cette personne, nous vous conseillons de la *bloquer*.


### Delta Chat prend-il en charge les images, vidéos et autres pièces jointes ?

Oui. En plus du texte brut, toutes les pièces jointes aux courriels sont affichées sous forme de messages séparés. Les messages sortants expédient automatiquement les pièces jointes que vous ajoutez.

- Pour améliorer les performances, les images sont redimensionnées et envoyées en taille réduite par défaut ; mais vous pouvez les envoyer en tant que "fichier" pour en conserver la taille originale.

<h3 id="multiple-accounts">Comment naviguer entre plusieurs comptes et comment en ajouter ?</h3>

Vous pouvez facilement gérer des comptes supplémentaires sur les clients Delta Chat mobile ou de bureau en cliquant :
- soit sur le bouton du menu, puis sur "Changer de compte" (Android et PC) ;
- soit sur l'icône de profil, puis sur "Ajouter un compte" (iOS).

Peut-être voudrez-vous aussi savoir [comment ajouter un compte sur plusieurs appareils](#multiclient).

### Qui peut voir ma photo de profil ?

Dans les paramètres vous pouvez ajouter une photo de profil. Si vous écrivez à vos contacts ou que vous les ajoutez via le QR code, ils la verront automatiquement comme votre photo de profil.

- Les contacts qui n'utilisent pas Delta Chat ne voient pas la photo de profil.
(Toutefois, ils peuvent bien sûr installer Delta Chat :)

- Pour des raisons de confidentialité, personne ne peut voir votre photo de profil sans que vous ayez d'abord entamé une discussion.

- Votre photo de profil n'est pas envoyée avec chaque message, mais assez régulièrement pour que vos contacts aient une photo à jour même s'ils ajoutent un nouvel appareil.


### Est-ce que Delta Chat gère les courriels en HTML ?

Yes, incoming HTML messages come with a "Show full message" button. 
Outgoing messages always use plain text.


### Pourquoi dois-je entrer le mot de passe de mon compte de courriel dans Delta Chat ? Est-ce sécurisé ?

Comme pour les autres clients de courriel, Thunderbird, FairEmail, K9-Mail, Outlook, etc, celui-ci a besoin des identifiants / mots de passe pour recevoir et envoyer des courriels. 
Bien sûr le mot de passe est uniquement stocké sur votre appareil. Et il est utilisé uniquement pour vous authentifier auprès de votre fournisseur de courriel, qui a, rappelons-le, accès à vos courriels non chiffrés.

Si vous utilisez un fournisseur de courriel qui prend en charge OAuth2, comme gmail.com ou yandex.ru,
il n'est pas nécessaire de stocker votre mot de passe sur votre appareil. Dans ce cas, seul un jeton d'accès est utilisé.

Comme Delta Chat est un logiciel libre, vous pouvez étudier le [code source](https://github.com/deltachat/deltachat-core-rust/blob/master/src/login_param.rs) pour vérifier que vos identifiants / mots de passe sont utilisés de façon sécurisée. Nous sommes très heureux d'avoir des retours pour renforcer la sécurité de l'application.


### De quelles autorisations Delta Chat a-t-il besoin?

Selon le système d'exploitation utilisé,
il vous sera peut-être demandé d'accorder des autorisations à l'application.
Voici ce que fait Delta Chat avec ces autorisations:

- Appareil photo * (peut être refusé) *
  - prendre des photos et des vidéos : pour envoyer des photos
- Contacts * (peut être refusé) *
  - lire vos contacts : pour trouver des contacts avec lesquels discuter
- Localisation * (peut être refusé) *
  - accéder à la localisation approximative (sources de localisation réseau) : pour la fonction de streaming de localisation
  - accéder à la localisation précise (GPS et sources de localisation réseau) : pour la fonction de localisation en continu
- Microphone * (peut être refusé) *
  - enregistrement audio : pour les messages audio
- Stockage * (peut être refusé) *
  - modifier ou supprimer le contenu de votre carte SD : pour télécharger les pièces jointes des messages
  - lire le contenu de votre carte SD : pour partager des fichiers avec vos contacts
- Autres capacités de l'application
  - modifier vos paramètres audio : pour choisir les sonneries et le volume des notifications et des messages audio
  - s'exécuter au démarrage : pour ne pas avoir besoin de démarrer Delta Chat manuellement
  - contrôler les vibrations : pour les notifications
  - afficher les connexions réseau : pour se connecter au fournisseur de messagerie
  - empêcher la veille du téléphone : pour copier plus facilement le code de sécurité pendant le message de configuration Autocrypt
  - avoir un accès complet au réseau : pour se connecter au fournisseur de messagerie
  - afficher les connexions Wi-Fi : pour se connecter au fournisseur de messagerie
  - demander d'ignorer les optimisations de batterie : pour les utilisateurs qui souhaitent recevoir des messages tout le temps

### Que signifient "épingler", "sourdine" et "archiver" ?

Ces options vous permettent d'organiser et trier vos discussions :

- Les **discussions épinglées** restent en haut de votre liste de discussions. Vous pouvez ainsi retrouver plus rapidement vos discussions favorites ou éviter d'oublier des messages importants.

- Utilisez la **sourdine** pour les discussions dont vous ne voulez pas recevoir les notifications. Les discussions en sourdine figurent toujours dans votre liste et peuvent aussi être les épinglées.

- **Archivez les discussions** si vous ne voulez plus les voir apparaître dans votre liste de discussions.
  Les discussions archivées restent accessibles au-dessus de la liste de discussions ou via la recherche. 

- Lorsqu'un nouveau message est envoyé sur une discussion que vous avez archivée, et que vous n'avez pas mise en sourdine, la discussion **sort des archives** et reprend sa place dans votre liste de discussions.
  **Les discussions en sourdine restent archivées** tant que vous ne les désarchivez pas manuellement.

Pour archiver ou épingler une discussion, faites un appui long sur la discussion concernée (Android), ouvrez le menu de la conversation (Android/application de bureau), ou balayez vers la gauche (iOS) ;
pour mettre une discussion en sourdine, ouvrez le menu de la conversation (Android/application de bureau) ou le profil de la discussion (iOS).


### Que signifie le point vert ?

- Depuis la version 1.34 de Delta Chat, vous voyez parfois un "point vert" à côté de la photo de profil d'un contact. Cela signifie qu'il a été "vu récemment".
- Plus précisément, cela signifie que Delta Chat a détecté l'activité de ce contact au cours des 10 dernières minutes :
  - soit parce qu'il vous a écrit personnellement ;
  - soit parce qu'il a écrit dans un groupe dont vous êtres tous les deux membres ;
  - soit parce qu'il a renvoyé l'accusé de lecture d'un message que vous lui avez écrit ;
  - ou bien parce qu'il a envoyé des données à votre appli Delta Chat via une [appli Webxdc](#webxdc).
- Le "point vert" n'est donc pas un statut en temps réel. Aussi, si quelqu'un ne vous répond pas immédiatement alors qu'il semble être en ligne, ne vous inquiétez pas et donnez-lui du temps ;-)
- D'un autre côté, vos contacts ne vous voient pas forcément "en ligne". Si vous avez désactivé les accusés de lecture, ils ne verront pas de point vert tant que vous ne leur écrivez pas directement ou n'écrivez pas dans un groupe dont ils font aussi partie.


### How do disappearing messages work? {#ephemeralmsgs}

You can turn on "disappearing messages"
in the settings of a chat,
at the top right of the chat window,
by selecting a time span
between 1 minute and 5 weeks.

Until the setting is turned off again,
each chat member's Delta Chat app takes care
of deleting the messages
after the selected time span.
The time span begins
when the receiver first sees the message in Delta Chat.
The messages are deleted
both in each email account on the server,
and in the app itself.

Note that you can rely on disappearing messages
only as long as you trust your chat partners;
malicious chat partners can take photos,
or otherwise save, copy or forward messages before deletion.

Apart from that,
if one chat partner uninstalls Delta Chat,
the messages will not get deleted from their email account.
They will most likely also not be decryptable anymore
(as long as they were encrypted in the first place).


### Comment supprimer mon compte ?

Étant donné que vous utilisez Delta Chat à travers un compte courriel, la façon dont vous pouvez supprimer votre compte dépend de votre fournisseur de courriel.
Comme nous n'exerçons aucun contrôle sur votre compte courriel, nous ne sommes pas en mesure de vous aider à le supprimer.

Si vous souhaitez conserver votre compte mais désinstaller Delta Chat, nous vous recommandons de quitter toutes les discussions de groupe avant de procéder à la désinstallation.


## Groupes

### Création d'un groupe

- Sélectionnez **Nouvelle discussion** puis **Nouveau groupe** dans le menu à trois points situé en haut à droite de la fenêtre ou son équivalent sous Android et iOS.
- Sur l'écran suivant, sélectionnez **Ajouter des participants** et choisissez un **Nom du groupe**. Vous pouvez aussi choisir une **image de groupe**.
- Lorsque vous enverrez le **premier message** dans le groupe, tous les membres en seront informés et pourront répondre. Le groupe est invisible aux autres membres si vous n'écrivez pas de premier message.


### Ajouter une personne à un groupe

- Chaque membre du groupe a les **mêmes droits** que les autres. Pour cette raison, chacun peut supprimer tous les membres ou en ajouter de nouveaux.
- Pour ajouter ou supprimer des membres, cliquez sur le nom du groupe dans le chat.


### J'ai quitté un groupe par accident.

- Comme vous n'êtes plus membre du groupe, vous ne pouvez pas vous y ajouter vous-même. 
Contactez n'importe quel autre membre de ce groupe dans une discussion directe pour lui demander de vous y ré-inviter.


### Je ne souhaite plus recevoir les messages d'un groupe.

- Supprimez-vous de la liste des membres ou supprimez la discussion entière. 
Si souhaitez rejoindre le groupe plus tard, demandez à un autre membre du groupe de vous ré-inviter.

- Vous pouvez également mettre un groupe en "Sourdine" : vous recevrez tous les messages et pourrez toujours écrire, mais n'aurez plus les notifications des nouveaux messages.


### Que signifient les coches affichées à côté des messages sortants ?

- **Une coche** signifie que le message a été envoyé avec succès à votre fournisseur.
- **Deux coches** signifient qu'au moins un appareil du destinataire
a signalé avoir reçu le message.
- Il se peut que les destinataires aient désactivé les accusés de réception,
donc même si vous ne voyez qu'une seule coche, le message peut avoir été lu.
- À l'envers, deux coches ne signifient pas automatiquement
qu'un humain a lu ou compris le message ;)


### Que se passe-t-il si j'active l'option "Supprimer les anciens messages sur le serveur" ?

- Par défaut, Delta Chat stocke tous les messages sur votre appareil. Vous pouvez donc configurer Delta Chat pour qu'il supprime automatiquement les anciens messages reçus, si vous souhaitez libérer de l'espace de stockage chez votre fournisseur de courriel. Ces messages seront conservés localement jusqu'à ce que vous les supprimiez aussi de votre appareil.

- Pour activer cette option, accédez à vos paramètres de "Discussions et fichiers multimédia", puis à **Supprimer les anciens messages → Supprimer les messages du serveur**.
  Vous pouvez régler un délai allant de "Immédiatement" à "Après 1 année".
  Tous les courriels reçus sur Delta Chat seront supprimés du serveur une fois le délai écoulé.

- Attention : si vous utilisez Delta Chat sur plusieurs appareils, vous devez laisser vos messages sur le serveur suffisamment longtemps pour permettre à votre/vos autre(s) appareil(s) de les télécharger aussi.


### Que se passe-t-il si j'active l'option "Supprimer les anciens messages de l'appareil" ? {#delold}

- Vous pouvez choisir de supprimer automatiquement les anciens messages pour libérer de l'espace de stockage sur votre appareil. 
- Pour activer cette option, ouvrez les paramètres des "Discussions et fichiers multimédias" et cliquez sur "Supprimer les anciens messages de l'appareil". Vous pouvez définir le délai après lequel *tous* les messages seront supprimés de votre appareil, parmi plusieurs choix allant de "Immédiatement" à "Après 1 année".


## Encryption and Security 

### Which standards are used for end-to-end encryption? 

[Autocrypt](https://autocrypt.org) is used for automatically
establishing end-to-end encryption with contacts and group chats.
Autocrypt uses a limited and [secure subset of the OpenPGP standard](#openpgp-secure).
End-to-End encrypted messages are marked with a padlock 
<img style="vertical-align:middle; width:1.2em; margin:1px" src="../assets/help/lock-icon.png" alt="padlock"/>.

[Secure-Join protocols](https://securejoin.delta.chat/en/latest/new.html)
are used for establishing chats with guaranteed end-to-end encryption 
which protects against network attacks and compromised servers.
Chats marked with a green checkmark 
<img style="vertical-align:middle; width:1.5em; margin:1px" src="../assets/help/green-checkmark.png" alt="green checkmark"/>
guarantee end-to-end encrypted messages. 

### How can i know if messages are end-to-end encrypted? {#whene2e}

All end-to-end encrypted messages carry a padlock:

<img style="width:160px; margin:1px" src="../assets/help/lock-screenshot.png" alt="padlock in bubble"/>

End-to-end encryption is guaranteed if there is a green checkmark next to the chat title:

<img style="width:211px; margin:1px" src="../assets/help/green-checkmark-screenshot.png" alt="green checkmark in title"/>


### How can I get guaranteed end-to-end encryption and green checkmarks? {#howtoe2ee}

Meet your chat partner outside Delta Chat, preferably in person
but a second channel like a video chat
or a different messenger is fine as well.
Perform the following QR show/scan procedure with your chat partner.
One of you is the "Inviter", the other is the "Joiner". 

**Inviter side**:

- Group invitation: 
  Tap the chat group title to see its member list, and select "QR Invite code". 
  Share the QR image with the other side either in person or through a second channel.

- Direct 1:1 chat invitation: 
  Tap the QR Code icon <img style="vertical-align:middle; width:1.8em; margin:1px" src="../assets/help/qr-icon.png" />
  on the Delta Chat app main screen -- 
  on Desktop the QR Icon is in the left-side sandwich menu.
  Share the QR image with the other side either in person or through a second channel.

**Joiner side**:

- Tap the QR Code icon <img style="vertical-align:middle; width:1.8em; margin:1px" src="../assets/help/qr-icon.png" />
  on the Delta Chat app main screen -- 
  on Desktop the QR Icon is in the left-side sandwich menu.

- Choose "SCAN QR CODE" and scan the QR Code 
  that you see from your chat partner in a second channel.

- Tap "OK"


**Both Inviter and Joiner**:

Wait while [Secure-Join network messages are exchanged](https://securejoin.delta.chat/en/latest/new.html#setup-contact-protocol) between both devices.

- If both devices are online,
  both sides will eventually see a (group or direct) chat with a green checkmark
  <img style="vertical-align:middle; width:1.5em; margin:1px" src="../assets/help/green-checkmark.png" alt="green checkmark"/>
  next to the title.

- If one of the devices is offline, the green checkmarks will only
  appear later when the device is internet-connected again
  and the Secure-Join network protocol completed. 

Congratulations! 
You now will automatically use guaranteed end-to-end encryption
with this contact and both of you can add each other to green-checkmarked groups
<img style="vertical-align:middle; width:1.5em; margin:1px" src="../assets/help/green-checkmark.png" alt="green checkmark"/>,
thereby automatically spreading guaranteed end-to-end encryption among its members. 


### What does the green checkmark and "guaranteed end-to-end encryption" mean? {#e2eeguarantee}

Chat titles with green checkmarks
<img style="vertical-align:middle; width:1.5em; margin:1px" src="../assets/help/green-checkmark.png" alt="green checkmark" />
mean that all messages in the chat will be end-to-end encrypted
and can not be read or altered by compromised e-mail servers or Internet providers. 
Joining green-checkmarked group chats
safely spreads everybody's encryption information (and green checkmarks)
in a manner that guarantees end-to-end encryption in the group and among members. 

Contact profiles with green checkmarks 
<img style="vertical-align:middle; width:1.5em; margin:1px" src="../assets/help/green-checkmark.png" alt="green checkmark" />
mean that messaging a contact is currently guaranteed to be end-to-end encrypted.
Every green-checkmarked contact either did a direct [QR-scan](#howtoe2ee) with you
or was introduced by a another green-checkmarked contact.
Introductions happen automatically when adding members to groups. 
Whoever adds a contact to a green-checkmarked group becomes an introducer 
to those members who didn't yet know about the added contact.
In a contact profile you can tap on the "Introduced by ..." text repeatedly
until you get to the one with whom you directly did a [QR-scan](#howtoe2ee).

Note that in a contact profile you may see and tap introducers 
but there is no green checkmark in the profile title. 
This usually means that the contact ["sent a message from another device"](#nocryptanymore). 

For more in-depth discussion of "guaranteed end-to-end encryption"
please see [Secure-Join protocols](https://securejoin.delta.chat/en/latest/new.html)
and specifically read about "Verified Groups", the technical term
of what is called here "green-checkmarked" or "guaranteed end-to-end encrypted" chats.


### A contact "sent a message from another device", what can i do? {#nocryptanymore}

Your chat with a contact lost guaranteed end-to-end encryption. 
The green checkmark was removed for this chat and contact when you see this warning. 
**If you find the sudden drop of guaranteed end-to-end encryption 
surprising for this contact then don't accept the warning!**
Instead check with your contact through a second channel 
like a video call, other messenger or a phone call,
to find out what happened. 

If your contact actually caused the drop of guaranteed end-to-end encryption
please see the next paragraphs for common reasons and their mitigations. 
Regardless, all other green-checkmarked chats remain guaranteed end-to-end encrypted
even if the contact is a member there. 

**Your contact is using Delta Chat on a second device (phone or laptop)**

If they have another device with a Delta Chat app running,
they should remove the account from the new device
and add it [as a second device as described here](#multiclient).
As soon as they message you afterwards, the warning will be gone
and guaranteed encryption is established with both devices of your contact. 

**Your contact reinstalled Delta Chat using their old account login**
 
If they have [a backup file](#backup), 
they should remove the account from the new device 
and rather import the backup file to re-create their account. 
As soon as they message you afterwards, the warning will be gone
and guaranteed encryption is re-established for this contact.

If they don't have a backup file, it's best to perform a [QR scan](#howtoe2ee) 
with your chat partner to re-establish guaranteed end-to-end encryption.

**Your contact sent a mail through a webmail interface or another e-mail app
and will get back to using Delta Chat soon again.**

If you are sure that the contact sometimes uses webmail,
or another mail app lacking end-to-end encryption,
then you may accept the warning.
As soon as your contact uses Delta Chat again, 
guaranteed end-to-end encryption will be automatically re-established. 

**Your contact stopped using Delta Chat entirely**

Sometimes remaining in contact is more important than end-to-end encryption.
["Transport Layer Encryption" (TLS)](#tls) may still meaningfully protect
the confidentiality of your messages between your device and the e-mail server. 
But without end-to-end encryption you and your contact are trusting your e-mail server
to not read or manipulate your messages, and to not hand them to third parties. 

In any case, you can not do much else than accept the warning.
Please also remove the contact from any active green-checkmarked group 
which you can find in "Shared chats" in the Contact profile. 
This spares your contact from getting "unreadable" messages. 

If the contact removed Delta Chat because of buggy or undesirable behaviour, 
please consider posting to our [support forum](https://support.delta.chat) 
to help us identify and address common problems. Thanks!


### Are attachments (pictures, files, audio etc.) end-to-end encrypted?

Oui.

When we talk about an "end-to-end encrypted message"
we always mean a whole message is encrypted,
including all the attachments
and attachment metadata such as filenames.


### Is OpenPGP secure? {#openpgp-secure}

Yes, Delta Chat uses a secure subset of OpenPGP
and only displays a padlock security indicator on a message
if the whole message is properly encrypted and signed.
For example, "Detached signatures" are not treated as secure.

OpenPGP is not insecure by itself.
Most publically discussed OpenPGP security problems
actually stem from bad usability or bad implementations of tools or apps (or both).
It is particularly important to distinguish between OpenPGP, the IETF encryption standard, 
and GnuPG (GPG), a command line tool implementing OpenPGP. 
Many public critiques of OpenPGP actually discuss GnuPG which Delta Chat has never used. 
Delta Chat rather uses the OpenPGP Rust implementation [rPGP](https://github.com/rpgp/rpgp),
available as [an independent "pgp" package](https://crates.io/crates/pgp),
and [security-audited in 2019](https://delta.chat/assets/blog/2019-first-security-review.pdf). 

We aim, along with other OpenPGP implementors, 
to further improve security characteristics by implementing the
[new IETF OpenPGP Crypto-Refresh](https://datatracker.ietf.org/doc/draft-ietf-openpgp-crypto-refresh/) 
which was thankfully adopted in summer 2023. 


### Did you consider using alternatives to OpenPGP for end-to-end -encryption? {#openpgp-alternatives}

Yes, we are following efforts like [MLS](https://en.wikipedia.org/wiki/Messaging_Layer_Security)
or [Saltpack](https://saltpack.org/) 
but adopting them would mean breaking end-to-end encryption interoperability 
with all other e-mail apps that typically support OpenPGP encryption. 
So it would not be a light decision to take 
and there must be tangible improvements for users. 

Delta Chat takes a holistic "usable security" approach 
and works with a wide range of activist groupings as well as 
renowned researchers such as [TeamUSEC](https://teamusec.de) 
to improve actual user outcomes against security threats. 
The wire protocol and standard for establishing end-to-end encryption is
only one part of "user outcomes",
see also our answers to [device-seizure](#device-seizure)
and [message-metadata](#message-metadata) questions. 


### Is Delta Chat vulnerable to EFAIL?

No, [Delta Chat never was vulnerable to EFAIL](https://delta.chat/en/2018-05-15-delta-chat-not-vulnerable-to-efail)
because its OpenPGP implementation [rPGP](https://github.com/rpgp/rpgp) 
uses Modification Detection Code when encrypting messages
and returns [an error](https://docs.rs/pgp/latest/pgp/errors/enum.Error.html#variant.MdcError)
if the Modification Detection Code is incorrect.

Delta Chat also never was vulnerable to the "Direct Exfiltration" EFAIL attack
because it only decrypts `multipart/encrypted` messages
which contain exactly one encrypted and signed part,
as defined by the Autocrypt Level 1 specification. 


### Is a message exposed in cleartext if end-to-end encryption is not available? {#tls}

Even if your messages are not guaranteed to be end-to-end encrypted, 
they are still protected from Internet providers like cell or cable companies. 
However, your and your recipient's e-mail providers 
may read, analyze or even modify your messages, 
including any attachments,
if they are not end-to-end encrypted. 

Delta Chat by default uses strict 
[TLS encryption](https://en.wikipedia.org/wiki/Transport_Layer_Security) 
which secures connections between your device and your e-mail provider. 
All of Delta Chat's TLS-handling has been independently [security audited](#security-audits).
Moreover, the connection between your and the recipient's e-mail provider
will typically be transport-encrypted as well.
If the involved e-mail servers support [MTA-STS](https://datatracker.ietf.org/doc/html/rfc8461)
then transport encryption will be enforced between e-mail providers 
in which case Delta Chat communications will never be exposed in cleartext to the Internet
even if the message was not end-to-end encrypted.

Note that [maintaining guaranteed end-to-end encryption](#howtoe2ee) on top of TLS encryption 
provides pervasive safety between your and the recipient's devices.
Not even your e-mail or Internet provider will be able to read or modify your messages. 


### How does Delta Chat protect metadata in messages? {#message-metadata}

Delta Chat protects most message metadata by putting the following information
into the end-to-end encrypted part of messages:

- Subject line 
- Group avatar and name 
- MDN (read receipt) requests (`Chat-Disposition-Notification-To`)
- Disappearing message timer (`Ephemeral-Timer`) 
- `Chat-Group-Member-Removed`, `Chat-Group-Member-Added` 
- `Secure-Join` header containing secure join commands
- Notification about enabling location streaming
- WebRTC room URL

E-Mail servers do not get access to this protected metadata 
but they do see the message date as well as the message size,
and, more importantly, the sender and receiver addresses. 
E-mail servers need receiver addresses to route and 
deliver messages to recipient's devices. 


### How to protect metadata and contacts when a device is seized? {#device-seizure}

Both for protecting against metadata-collecting e-mail servers 
as well as against the threat of device seizure
we recommend to use a Delta Chat optimized [e-mail server instance](https://delta.chat/serverguide)
to create pseudonymous temporary accounts through QR-code scans.
Note that Delta Chat apps on all platforms support multiple accounts 
so you can easily use action-specific "1-week" or "1-month" accounts next to your "main" account
with the knowledge that all temporary account data, along with all metadata, will be deleted.
Moreover, if a device is seized then contacts using temporary e-mail accounts
can not be identified easily, as compared to messengers which reveal
phone numbers in chat groups which in turn are often associated with legal identities.


### How can i check encryption information?

You may check the end-to-end encryption status manually in the "Encryption" dialog
(user profile on Android/iOS or right-click a user's chat-list item on desktop).
Delta Chat shows two fingerprints there.
If the same fingerprints appear on your own and your contact's device,
the connection is safe.


### How can I check the encryption status of messages?

A little **padlock** in a message bubble denotes
that the message was properly end-to-end encrypted from the given sender.
If there is **no padlock**, the message was not properly end-to-end encrypted
most likely because the sender uses an app or webmail interface
without support for end-to-end--encryption.


### Why do I see unencrypted messages? 

If a contact uses a non-Autocrypt e-mail app,
all messages involving this contact (in a group or 1:1 chat)
will not be end-to-end encrypted, and thus not show a "padlock" with messages.
Note that even if your contacts use Delta Chat on their account,
they might also use a non-Autocrypt e-mail app on that account
which then may cause intermittently unencrypted messages.
Replying unencrypted to unencrypted messages is mandated by Autocrypt
to prevent unreadable messages on the side of your contacts
and their non-Autocrypt e-mail app.

### How can i get an end-to-end encrypted chat with a Delta Chat contact who sometimes uses webmail or another non-Autocrypt e-mail app? 

If you need a safely end-to-end encrypted chat with a contact 
who is using their account both with Delta Chat and non-Autocrypt apps (e.g. webmail),
it's best to setup [guaranteed end-to-end encryption with them](#howtoe2ee)
and then create a guaranteed end-to-end encrypted group chat with you two as members. 
In this group chat all messages will be end-to-end encrypted 
even if the direct chat between you two has a
["… sent a message from another device"](#nocryptanymore) warning. 


### How can I ensure message end-to-end encryption and deletion?

The best way to ensure every message is end-to-end encrypted,
and metadata deleted as quickly as possible
is [using chats with guaranteed end-to-end encryption](#howtoe2ee)
and turning on [disappearing messages](#ephemeralmsgs).

Guaranteed end-to-end encrypted chats protect against [MITM attacks](https://en.wikipedia.org/wiki/Man-in-the-middle_attack)
and turning on disappearing messages deletes the messages
on the server after a user-configured time.

If you don't need a longer-lived copy of your messages on the server, 
you can also turn on ["delete messages from server automatically"](#delold).


### Does Delta Chat support Perfect Forward Secrecy? {#pfs}

No, Delta Chat doesn't support Perfect Forward Secrecy (PFS).
This means that if your Delta Chat private decryption key is leaked,
and someone has collected your prior in-transit messages,
they will be able to decrypt and read them using the leaked decryption key.

Note, however, that if anyone obtains to your decryption keys, 
they will typically also be able to obtain your messages, 
irrespective if Perfect Forward Secrecy is in place or not. 
The typical real-world situation for leaked decryption keys is device seizure
which we discuss in our answer [on metadata and device seizure](#device-seizure). 

It is possible that Delta Chat evolves to support Perfect Forward Secrecy,
because OpenPGP is just a container for encrypted messages 
but encryption key management (and thus key rotation or key "ratcheting") 
could be organized in flexible ways. 
See [Seqouia's PFS prototype](https://gitlab.com/sequoia-pgp/openpgp-dr)
for existing experiments in the OpenPGP implementor community.


### Is end-to-end encryption of Delta Chat as safe as Signal? 

It depends on what is important to you. 
Delta Chat [does not support PFS](#pfs) like Signal does
but it provides [guaranteed end-to-end encrypted chats](#e2eeguarantee)
that are safe against compromised servers or corrupted networks. 
Signal and most other PFS-supporting messengers do not provide 
a practical scheme for protecting chat groups from network attacks
which are arguably more worrysome 
than a potential attacker who seizes your phone and private encryption setup
but somehow not your messages, yet has a full record of all 
past encrypted messages. 

In any case, Delta Chat's end-to-end encryption uses a [secure subset of OpenPGP](#openpgp-secure)
which has been [independently security-audited](../assets/blog/2019-first-security-review.pdf).

### Puis-je ré-utiliser ma clé privée existante ?

Oui.
The best way is to send an Autocrypt Setup Message from the other e-mail client.
Look for something like **Start Autocrypt Setup Transfer** in the settings of the other client and follow the instructions shown there.

Alternatively, you can import the key manually in "Settings -> Advanced settings -> Import secret keys".
Caution: Make sure the key is not protected by a password, or remove the password beforehand.

If you don't have a key or don't even know you would need one - don't worry: Delta Chat generates keys as needed, you don't have to hit a button for it.

### Je n'arrive pas à importer ma clé PGP existante dans Delta Chat.

L'origine la plus probable de ce problème est que votre clé est chiffrée ou requiert un mot de passe, ou les deux. Ce type de clés n'est pas géré par Delta Chat. Vous pouvez tenter de retirer le chiffrement et le mot de passe puis réessayer l'importation. 

Another common error is having the wrong file ending.
Use the ASCII armored format and an `.asc` file ending.

Delta Chat gère les formats de clé privée OpenPGP les plus communs, néanmoins il
 est peu probable que les clés privées générées par toutes les sources soient prises en charge. Mais l'objectif principal de Delta Chat n'est pas là. En pratique, la majorité des nouveaux utilisateurs ne possèdent pas de clés de chiffrement avant d'utiliser Delta Chat.
Néanmoins, nous essayons de gérer les clés privées d'autant de sources que possible.

La méthode pour retirer le mot de passe de la clé privée dépend du logiciel que vous utilisez pour gérer vos clés GPG. Avec Enigmail, vous pouvez définir votre mot de passe en laissant le champ vide dans la fenêtre de Gestion des Clés. Avec GnuPG, vous pouvez le définir [avec la ligne de commande](https://github.com/deltachat/deltachat-android/issues/98#issuecomment-378383429).
Pour les autres programmes, vous devriez pouvoir trouver la solution en ligne.

## Multi-client {#multiclient}

### Puis-je utiliser Delta Chat sur plusieurs appareils en même temps?

Oui. Delta Chat 1.36 comes with a new, experimental function for using the same account on different devices:

- Make sure both devices are on the same Wi-Fi or network

- Sur le premier appareil, allez dans **Paramètres → Ajouter un deuxième appareil**, déverrouillez l'écran si nécessaire, et patientez un peu jusqu'à ce qu'un code QR s'affiche.

- Sur le deuxième appareil, [installez Delta Chat](https://get.delta.chat).

- Sur le deuxième appareil, ouvrez Delta Chat, sélectionnez **Ajouter comme deuxième appareil**, et scannez le code QR du premier appareil.

- Le transfert devrait commencer quelques secondes après et, pendant l'opération, les deux appareils affichent l'**état d'avancement**.
  Patientez jusqu'à ce que le transfert soit terminé sur les deux appareils.

Contrairement à de nombreuses autres messageries, une fois le transfert terminé, les deux **appareils sont complètement indépendants**.
L'un n'a pas besoin de l'autre pour pouvoir fonctionner.


### Dépannage

- Vérifier à nouveau que les deux appareils sont sur **le même réseau ou le même Wi-Fi**.

- Il se peut que votre système dispose d'un "pare-feu personnalisé",
  source bien connue de dysfonctionnements (en particulier sur Windows).
  **Désactivez le pare-feu personnalisé** sur chaque appareil pour Delta Chat et réessayez.

- Assurez-vous de disposer d'un **espace de stockage suffisant** sur l'appareil de destination.

- Une fois que le transfert a commencé, assurez-vous que les appareils **restent actifs** et ne se mettent pas en veille.
  Ne quittez pas Delta Chat !
  (Nous faisons de notre mieux pour que l'application fonctionne en arrière-plan, mais les [systèmes ont une fâcheuse tendance à tuer les applis](https://dontkillmyapp.com).)

- Si Delta Chat est **déjà connecté** sur l'appareil de destination.
  Vous pouvez utiliser plusieurs comptes par appareil : [ajoutez un nouveau compte](#multiple-accounts).

- Si les problèmes persistent, ou si vous **ne pouvez pas scanner de code QR**,  essayez la méthode de **transfert manuel** décrite ci-dessous.


### Manual Transfer {#backup}

Recourez à cette méthode uniquement si les instructions ci-dessus pour "Ajouter un deuxième appareil" ont échoué.

- On the old device, go to "Settings -> Chats and media -> Export Backup". Enter your
  screen unlock PIN, pattern, or password. Then you can click on "Start
  Backup". This saves the backup file to your device. Now you have to transfer
  it to the other device somehow.
- On the new device, on the login screen, instead of logging into your email
  account, choose "Import Backup". After import, your conversations, encryption
  keys, and media should be copied to the new device.
  - **If you use iOS:** and you encounter difficulties, maybe
    [this guide](https://support.delta.chat/t/import-backup-to-ios/1628) will
    help you.
- You are now synchronized, and can use both devices for sending and receiving
  end-to-end encrypted messages with your communication partners.

### Le lancement d'un client Web Delta Chat est-il prévu ?

- Il n'y a pas de plans immédiats mais quelques idées préliminaires.
- Il y a 2-3 façons d'introduire un client Web Delta Chat, mais toutes représentent
 un travail conséquent. Pour l'instant, nous nous concentrons à sortir des versions stables dans tous les magasins d'applications (Google Play/iOS/Windows/macOS/centre de paquets Linux) en tant qu'applications natives.
- Si vous avez besoin d'un client Web parce que vous n'êtes pas autorisé à installer des logiciels sur l'ordinateur sur lequel vous travaillez, vous pouvez utiliser le Client Portable pour bureaux Windows ou l'AppImage pour Linux. Vous pouvez les trouver sur 
[get.delta.chat](https://get.delta.chat).


### Quel est l'intérêt du paramètre “M'envoyer une copie”? 

Envoyer une copie de vos messages à vous-même garantit que vous recevez vos propres
 messages sur tous les appareils. Si vous avez de multiples appareils et que vous ne l'activez pas, vous voyez seulement les messages des autres personnes et les messages que vous avez envoyé depuis l'appareil en cours.

La copie est envoyée dans la Boîte de réception puis déplacée dans le dossier DeltaChat; elle n'est pas mise dans le dossier “Envoyés”. Delta Chat ne téléverse jamais quelque chose dans le dossier Envoyés car ça signifierait de le téléverser deux fois (une fois via SMTP, puis une fois dans le dossier Envoyés via IMAP).

Le paramètre par défaut pour l'envoi à soi-même est "Non".

### Pourquoi puis-je choisir de regarder le dossier “Envoyés”? 

La seule raison de regarder le dossier Envoyés est si vous utilisez un autre programme de courriel (tel que Thunderbird) en parallèle de votre application Delta Chat, et que vous voulez que votre client de messagerie participe aux discussions.

Cependant, nous recommandons d'utiliser le client de bureau Delta Chat; vous pouvez le télécharger sur [get.delta.chat](https://get.delta.chat). L'option de regarder le dossier “Envoyés” pourrait disparaître dans le futur. Elle a été introduite à une époque où il n'y avait pas de client de bureau Delta Chat disponible sur toutes les plateformes.

### Pourquoi puis-je choisir de ne pas regarder le dossier Delta Chat? 

Certaines personnes utilisent Delta Chat comme un client de messagerie normal, et veulent utiliser la Boîte de réception pour leurs mails au lieu d'utiliser le dossier DeltaChat. Si vous désactivez “Surveiller le dossier DeltaChat”, vous devriez aussi désactiver “déplacer les messages de discussions dans DeltaChat”.
Sinon, la suppression de messages dans une configuration multi-appareils pourrait ne pas marcher correctement.


## webxdc apps {#webxdc}

In Delta Chat, you can share [webxdc apps](https://webxdc.org), attachments with an `.xdc` file
extension. They can do very different things, and make Delta Chat a truly
extendable messenger.


### How private are webxdc apps?

- webxdc apps can not send data to the Internet, or download anything.
- A webxdc app can only exchange data within a Delta Chat chat, with its
  copies on the devices of your chat partners. Other than that, it's completely
  isolated from the Internet.
- The privacy a webxdc app offers is the privacy of your chat - as long as you
  trust the people you chat with, you can trust the webxdc app as well.
- This also means: it can be a privacy risk to open webxdc apps in chats where
  you don't trust the members - as you know it from e-mail attachments, where 
  you only open attachments from senders you trust, and not from spammers.


### Where can I get webxdc apps?

- In general, anyone can share webxdc apps with each
  other without restrictions.
- You can [send 'hi' to xstore@testrun.org](https://delta.chat/en/2023-08-11-xstore)
  to see an experimental webxdc appstore.
  All of the apps are open source and for free.
- Many people write their own webxdc apps and post them to [the Delta Chat
  forum](https://support.delta.chat/c/webxdc/20).


### How can I create my own webxdc apps?

- webxdc apps are just zip files containing html, css, and javascript code.
- You can extend the [Hello World example app](https://github.com/webxdc/hello)
  to get started.
- All else you need to know is written in the
  [documentation](https://docs.webxdc.org/).
- If you have question, you can ask others with experience in the [Delta Chat
  Forum](https://support.delta.chat/c/webxdc/20).


## Fonctionnalités expérimentales

We are very grateful for feedback on these features - do you want to share
your ideas? Join the [Forum](https://support.delta.chat) to contribute. 
You may conveniently login via Delta Chat and a QR code scan,
another rather stable experiment we run on the side (sic!).

### Comment passer des appels audio/vidéo avec Delta Chat ?

- To turn on audio/video calls, go to the "experimental features" section in
  the advanced settings and choose a "Video Chat Instance". 
- When you invite others to a video chat, it is opened in your browser/app at
  once. The others receive an e-mail with a link to the video chat. 
  This way, it is also compatible if your chat partners don't use Delta Chat.
- Note that there is no ring tone on the other side, and your chat partners
  will not get interrupted by a video chat invite.
- You can use any video chat service which allows joining by link. Just add the
  link in the settings.
- For example, to use the flagship Jitsi Meet instance, you could enter
  `https://meet.jit.si/$ROOM`. The `$ROOM` variable will be a random value;
  this way, you will have a new random jitsi room every time you call someone.


### Que sont les listes de diffusion et comment les utiliser ?

- Une liste de diffusion vous permet d'envoyer un message à plusieurs destinataires en même temps sans qu'ils puissent se voir mutuellement. Vous recevez leurs réponses respectives dans les discussions privées que vous avez avec chacun d'eux.
- Concrètement, c'est un courriel avec plusieurs destinataires en copie cachée.
- Vous pouvez activer cette option dans la section "Fonctionnalités expérimentales" des paramètres avancés. Vous pourrez ensuite créer une liste de diffusion à partir du bouton "Nouvelle discussion".
- Si vous utilisez plusieurs appareils, veuillez noter qu'il n'est pas possible, pour l'instant, de synchroniser les listes de diffusion.
- Les messages envoyés à des listes de diffusion ne sont pas chiffrés, parce que le chiffrement romprait l'anonymat puisque tous les destinataires pourraient alors voir qui d'autre a reçu le message.
  (Mais envoyer des courriels individuels à tout le monde serait encore pire à cause de la consommation du réseau requise et des limites d'envoi).


### Comment partager ma géolocalisation avec mes contacts ?

- Vous pouvez activer l'envoi de la géolocalisation à la demande dans la section "Fonctionnalités expérimentales" des paramètres avancés.
- Pour partager votre position dans une discussion, allez dans "Ajouter une pièce jointe" et sélectionnez "Position". Vous pouvez alors choisir la durée pendant laquelle vous voulez partager votre position avec les membres de la discussion, de 5 minutes à 6 heures.
- Quand vous vous déplacez, vos contacts voient votre position sur une carte dans la discussion.
- Vous devez activer cette fonctionnalité dans les paramètres avancés pour pouvoir voir la carte et la position de vos contacts.
- Cette fonctionnalité ne partage votre position avec personne d'autre que les membres de la discussion. *Cependant,* pour que la carte s'affiche, les tuiles de carte sont téléchargées depuis mapbox.com, donc si vous *visualisez* la carte, une requête pour afficher une zone spécifique est envoyée à mapbox.com. Si cela constitue un risque pour la protection de votre vie privée, cette fonctionnalité n'est probablement pas faite pour vous. Nous nous efforçons de trouver une alternative décentralisée à Mapbox.
- Sur l'application de bureau, votre système d'exploitation ne peut généralement pas déterminer votre position. À la place, vous pouvez faire un clic droit sur la carte pour décrire votre position, qui sera ensuite envoyée dans la discussion en tant que message, tout en apparaissant sur la carte.


### Que protège réellement le chiffrement expérimental de base de données ?

- À l'heure actuelle, le chiffrement de la base de données est encore expérimental. Mieux vaut ne pas vous y fier pour la protection de vos données et activer aussi le chiffrement votre système d'exploitation si vous le pouvez.
- Le chiffrement de base de données ne permet pas encore de chiffrer les blobs, seulement les lignes et les colonnes de la base. Cela signifie grosso modo que vos messages sont bien protégés, mais pas les pièces jointes.
- Sur iOS et Android, les clefs de chiffrements sont stockées dans le trousseau système. Par conséquent, le chiffrement est aussi fiable que le système d'exploitation dont il dépend.
- Comme il n'existe aucun moyen standardisé de stocker les clefs de chiffrement sur les différentes plateformes disponibles, le chiffrement de la base de données n'est pas encore disponible pour le client bureau de Delta Chat.


### Pourquoi peut-on choisir de ne consulter que le dossier Delta Chat ?

Il s'agit d'un paramètre expérimental à destination des personnes qui expérimentent avec des règles côté serveur. Tous les fournisseurs ne le prennent pas en charge, mais certains permettent de déplacer tous les courriels avec un en-tête "Chat-Version" dans le dossier DeltaChat. Normalement, cette action est réalisé par l'application Delta Chat.

Activer l'option "Ne consulter que le dossier Delta Chat" est intéressant si vous avez **à la fois** :

- activé une règle côté serveur pour déplacer tous les messages avec un en-tête "Chat-Version" dans le dossier Delta Chat ;
- modifié le paramètre "Voir les courriels classiques" pour "Non, seulement les discussions".

Si ces deux conditions sont remplies, Delta Chat n'a pas besoin de surveiller la boîte de réception, seulement le dossier Delta Chat.


### Comment changer mon compte pour une adresse courriel différente ?

1. Change your address in “Settings - Password and Account” and
   enter the password of your new account (and if necessary, server settings).
   You will get an information notice about the fact that you are moving to a new address. 
   An additional notice will also show up in your "Device messages" chat. 

2. If possible, let your old e-mail provider forward all messages to your new address.

3. Tell your contacts that you changed your address. 
   Writing to guaranteed end-to-end encrypted chats and groups,
   will make them notice your move automatically 
   and they will continue chatting with you using your new address. 

Note that Delta Chat will not retrieve messages anymore from your old e-mail provider.
If you didn't configure your e-mail provider to forward messages (step 2.) 
only those contacts to whom you sent a message in a guaranteed end-to-end encrypted chat
will send messages to your new address. 

To learn more about this the details behind this, [read our blogpost on
it](https://delta.chat/en/2022-09-14-aeap).


## Divers

### Est-ce que Delta Chat fonctionne avec _mon_ fournisseur de courriel ? 

- Il y a de bonnes chances que oui :)
Cependant, il faut activer des options spéciales pour que cela fonctionne correctement avec certains fournisseurs... Voir [la liste des fournisseurs](https://providers.delta.chat).


### Je veux administrer mon propre serveur courriel pour Delta Chat : que me conseillez-vous ?

- La plupart des serveurs courriel fonctionneront très bien. Mais nous conseillons de combiner mailcow et mailadm, ainsi que nous le décrivons [sur notre blog](https://delta.chat/en/2023-01-27-upcoming-mail-server-workshops).
- Vous trouverez un [guide d'installation sur notre site internet](serverguide).


### Si Delta Chat se base sur le courrier électronique, est-ce vraiment une messagerie _instantanée_? 

- L'envoi et la réception de messages prennent généralement quelques secondes. Il arrive parfois que cela prenne plus de temps, mais c'est aussi le cas avec n'importe quelle autre messagerie.
- La messagerie instantanée est rapide quand les deux parties utilisent activement l'application. Elle peut devenir plus lente si l'application fonctionne en arrière-plan.
- La réception de messages peut alors prendre plusieurs minutes, car Android et iOS empêchent souvent Delta Chat de fonctionner en arrière-plan et ne le réveillent qu'occasionnellement. Ce délai artificiel est généralement pire sur iOS que sur Android.
- Cependant, le fait qu'Android et iOS tuent les applications fonctionnant en arrière-plan constitue un problème pour de nombreuses applications reconnues.
Pour plus d'informations, voir [dontkillmyapp.com](https://dontkillmyapp.com/).


### Delta Chat est-il compatible avec Protonmail / Tutanota / Criptext ?

- Yes and No.
- No, you can not use your Protonmail, Tutanota, or Criptext account with Delta
  Chat; they do not offer receiving mails via IMAP.
- In any case you can use Delta Chat to send Messages to people who use
  Protonmail, Tutanota, or Criptext. Those messages will not be end-to-end
  encrypted, though. The end-to-end encryption those providers offer is not
  compatible with [Autocrypt](https://autocrypt.org/), the standard Delta Chat
  uses.
- Delta Chat can end-to-end-encrypt through any e-mail provider with any
  [Autocrypt-enabled e-mail app](https://autocrypt.org/dev-status.html).


### Les détails techniques m'intéressent. Pouvez-vous m'en dire plus ?

- Consultez les [standards utilisés dans Delta Chat]({% include standards-url %}).

### Est-ce qu'un audit indépendant des failles de sécurité a été réalisé sur Delta Chat ? {#security-audits}

Quatre audits indépendants ont été réalisés sur le projet Delta Chat ces dernières années :

- En 2019, [Include Security](https://includesecurity.com) a analysé les bibliothèques [PGP](https://github.com/rpgp/rpgp) et
[RSA](https://github.com/RustCrypto/RSA) de Delta Chat.
Aucune faille critique n'a été trouvée, mais deux failles sévères ont été identifiées et immédiatement réparées par nos soins.
Une faille de gravité moyenne ainsi que quelques failles de gravité moindre ont également été découvertes, sans qu'il soit toutefois possible de les exploiter dans le fonctionnement de Delta Chat.
Nous en avons néanmoins réparées certaines depuis le rapport d'audit.
Le rapport complet [est consultable ici](../assets/blog/2019-first-security-review.pdf).

- En 2020, [Include Security](https://includesecurity.com) a analysé les [bibliothèques principales](https://github.com/deltachat/deltachat-core-rust/) Rust de Delta Chat, ainsi que ses bibliothèques [IMAP](https://github.com/async-email/async-imap), [SMTP](https://github.com/async-email/async-smtp) et [TLS](https://github.com/async-email/async-native-tls).
Aucun problème grave ou critique n'a été découvert.
Le rapport a tout de même révélé quelques vulnérabilités de gravité moyenne, qui ne représentent pas une menace en elles-mêmes pour les utilisateurs et les utilisatrices de Delta Chat, car elles dépendent de l'environnement dans lequel Delta Chat est utilisé.
Pour des raison de compatibilité et de facilité d'utilisation, nous ne pouvons pas les pallier toutes et avons préféré fournir des préconisations de sécurité aux personnes exposées.
Le rapport complet [est consultable ici](../assets/blog/2020-second-security-review.pdf).

- Début 2023, [Cure53](https://cure53.de) a analysé le chiffrement d'acheminement des connexions réseau de Delta Chat et testé une configuration de serveur de courriel reproductible, telle que [recommandée sur ce site](serverguide).
Vous trouverez plus d'informations sur cet audit [sur notre blog](https://delta.chat/en/2023-03-27-third-independent-security-audit) ou dans [le rapport complet ici](../assets/blog/MER-01-report.pdf).

- Beginning 2023, we fixed security and privacy issues with the "web
  apps shared in a chat" feature, related to failures of sandboxing
  especially with Chromium. We subsequently got an independent security
  audit from Cure53 and all issues found were fixed in the 1.36 app series released in April 2023.
  See [here for the full background story on end-to-end security in the web](https://delta.chat/en/2023-05-22-webxdc-security).


### Comment est financé le développement de Delta Chat ?

Delta Chat ne reçoit par de fonds en capital-risque, n'est pas endetté et ne subit aucune pression pour générer de gros profits ou vendre ses utilisateurs et utilisatrices - en même temps que leurs amis et leur famille - à des annonceurs (ou pire). 
Nous préférons utiliser des fonds provenant d'institutions publiques, jusqu'à présent basées en Europe ou aux États-Unis, pour soutenir nos efforts de développement d'un système de messagerie diversifié et décentralisé, basé sur les contributions de la communauté du libre et de l'open-source.

Jusqu'à présent, le développement de Delta Chat a été financé par les sources suivantes :

- The [NEXTLEAP](https://nextleap.eu) EU project funded the research
  and implementation of verified groups and setup contact protocols
  in 2017 and 2018 and also helped to integrate end-to-end Encryption
  through [Autocrypt](https://autocrypt.org).

- L'association [Open Technology Fund](https://opentechfund.org) nous a octroyé une première subvention en 2018/2019 (de 200.000$ environ), grâce à laquelle nous avons pu apporter des améliorations majeures à l'application Android et publier une première version Beta de l'application de bureau. Elle nous a aussi permis d'ancrer notre recherche UX de développement de fonctionnalités dans des contextes de droits humains.   
À ce sujet, vous pouvez consulter notre rapport en anglais ["Needfinding and UX report"](https://delta.chat/en/2019-07-19-uxreport).
La seconde subvention de 2019/2020 (environ 300.000$) nous a permis de publier des version iOS de Delta Chat, de convertir notre bibliothèque principale en Rust et de créer de nouvelles fonctionnalités pour toutes les plateformes.  

- The [NLnet foundation](https://nlnet.nl/) granted in 2019/2020 EUR 46K for
  completing Rust/Python bindings and instigating a Chat-bot eco-system. 

- En 2021, nous avons reçu un financement européen supplémentaire pour deux initiatives de Next Generation Internet : 97.000€ pour la création d'un [annuaire de la portabilité des fournisseurs de courriel](https://dapsi.ngi.eu/hall-of-fame/eppd/) (ou EPPD pour "e-mail provider portability directory"), et environ 90.000€ pour le développement du [portage des adresses courriel](https://nlnet.nl/project/EmailPorting/) (ou AEAP pour "email address porting"). Ces deux projets ont aussi permis une meilleure prise en charge de la fonctionnalité multi-compte, un QR code de contact plus performant et de nombreuses améliorations concernant la gestion des réseaux et les configurations de groupe sur toutes les plateformes.

- Entre la fin de l'année 2021 et mars 2023, nous avons bénéficié d'un fonds *Internet Freedom* (pour la "liberté d'internet", de 500.000$) du Bureau of Democracy, Human Rights and Labor (DRL) des États-Unis. 
Cet argent est venu soutenir nos deux objectifs de longue date ; à savoir améliorer la compatibilité de Delta Chat pour le rendre utilisable plus facilement avec un large éventail de serveurs de courriel dans le monde entier, et en améliorer la résistance et la sécurité dans les régions où les coupures internet et la censure d'internet sont monnaie courante.

- Début 2023, nous avons été acceptés dans le programme Entrust de Next Generation Internet (NGI) pour nos projets d'applications privées décentralisées. 
Le montant exact de la subvention reste à déterminer (autour de 100.000€). 
Ce financement nous permettra de continuer le développement des [appli webxdc partagées dans une discussion](https://webxdc.org). 

- Nous recevons parfois des dons ponctuels de la part de personnes privées. 
 En 2021 par exemple, une généreuse personne nous a envoyé 4000€ par virement bancaire, avec l'intitulé "continuez votre super travail de développement !". 💜 
 Nous utilisons l'argent de ces dons pour financer des rencontres entre développeurs et développeuses ou pour des dépenses ponctuelles difficiles à anticiper ou à rembourser avec des subventions publiques.
Recevoir plus de dons aide notre communauté de contributrices et contributeurs à devenir plus indépendante et à rester viable sur le long terme.

[Faire un don](donate){: .cta-button}

- Dernier point, mais certainement pas des moindres : quelques personnes passionnées et expertes ont apporté, et apportent toujours, leur contribution bénévole au développement de Delta Chat sans contrepartie financière - ou seulement de petites sommes. Sans leur énergie, Delta Chat n'en serait pas là aujourd'hui... et de très loin.

Les financements mentionnés précédemment sont gérés principalement par merlinux GmbH à Fribourg (Allemagne) et redistribués à plus d'une douzaine de contributeurs et contributrices du monde entier.

N'hésitez pas à consulter les [Canaux de contribution à Delta Chat Contribution](contribute) pour en savoir plus sur les différentes manières de contribuer, financières ou non.  
