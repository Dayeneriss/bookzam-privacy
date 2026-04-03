# Politique de confidentialite — BookZam

Derniere mise a jour : 3 avril 2026

BookZam respecte votre vie privee. Cette politique explique quelles donnees sont collectees, comment elles sont utilisees, et quels sont vos droits.

## 1. Donnees collectees

### 1.1 Donnees de compte
- Adresse e-mail et nom (lors de la creation de compte)
- Identifiant de connexion via Google Sign-In ou Sign in with Apple
- Photo de profil (si fournie via Google ou Apple)

### 1.2 Donnees de bibliotheque
- Historique des livres scannes, recherches et ajoutes
- Coordonnees geographiques associees a chaque scan (latitude, longitude, ville, pays), si vous avez autorise la localisation. Ces donnees sont stockees dans votre profil sur nos serveurs (Cloud Firestore) et servent a alimenter votre carte des decouvertes.
- Favoris, notes personnelles, statuts de lecture
- Progression de lecture et objectifs
- Defis de lecture et badges obtenus

### 1.3 Donnees d'ecoute (audiobooks)
- Sessions d'ecoute (debut, fin, duree, vitesse de lecture)
- Progression par chapitre et par audiobook
- Retours post-ecoute (feedback d'abandon ou de fin)

### 1.4 Donnees sociales
- Profil public : pseudo, niveau de lecture, genres preferes, nombre de livres, badges
- Activite partagee : livres ajoutes, defis completes, badges obtenus
- Messages dans les clubs de lecture

### 1.5 Donnees liees a l'IA
Lorsque vous utilisez les fonctionnalites d'intelligence artificielle (recherche par humeur, recherche par citation, ADN Litteraire, chat Livre Oublie, quiz, recommandations), les textes que vous saisissez ainsi que le contexte de votre bibliotheque sont envoyes aux serveurs de Google (Gemini) pour traitement. Aucune image de couverture n'est envoyee pour la reconnaissance de texte (OCR), qui est effectuee entierement sur votre appareil.

### 1.6 Donnees techniques
- Modele d'appareil, version du systeme d'exploitation, version de l'application
- Logs de crash anonymes (traces d'erreur, sans donnees personnelles)
- Evenements d'utilisation anonymises (ecrans visites, fonctionnalites utilisees)
- Proprietes utilisateur anonymisees transmises a Firebase Analytics : plateforme (Android/iOS/Web), source d'installation (Google Play, App Store...), type de compte (anonyme, gratuit, premium), anciennete d'installation, nombre de sessions, nombre de livres, fonctionnalites decouvertes, niveau d'engagement
- Compteurs d'utilisation locaux (nombre de scans, recherches IA, quiz, etc.) stockes sur votre appareil et synchronises periodiquement
- Jeton de notification push (FCM token)

### 1.7 Donnees de localisation
- Position geographique (uniquement si vous l'autorisez), utilisee pour :
  - **Carte des decouvertes** : les coordonnees GPS (latitude, longitude) et la localisation inverse (ville, pays) sont enregistrees avec chaque scan de livre dans votre profil Firestore. Vous pouvez supprimer cet historique dans Parametres > Effacer l'historique.
  - **Liens d'achat** : votre pays est detecte pour vous rediriger vers la boutique Amazon correspondante. Le code pays est mis en cache localement sur votre appareil (SharedPreferences), mais n'est pas envoye a nos serveurs.
- Vous pouvez revoquer l'acces a la localisation a tout moment dans les reglages de votre telephone. L'application continuera de fonctionner normalement sans cette permission.

### 1.8 Donnees multimedia
- Acces a la camera (pour scanner des couvertures de livres et des etageres)
- Acces aux photos (pour selectionner des images de livres)
- Acces au microphone (pour la recherche vocale)
- Ces donnees sont traitees localement ou transmises temporairement pour la reconnaissance. Elles ne sont pas stockees sur nos serveurs.

## 2. Utilisation des donnees

- Fournir les fonctionnalites principales de l'application (bibliotheque, recherche, recommandations, audiobooks, quiz, clubs de lecture)
- Personnaliser votre experience (recommandations IA, ADN Litteraire, profil de lecture)
- Gerer votre abonnement Premium
- Afficher des publicites pertinentes (pour les utilisateurs gratuits uniquement)
- Ameliorer l'application (statistiques d'usage anonymisees, correction de bugs)
- Envoyer des notifications de rappel et de progression (desactivables dans les parametres)
- Proposer des liens d'achat vers Amazon via des liens affilies (programme Amazon Associates, tag `bookzam0cf-21`). BookZam percoit une commission sur les achats effectues via ces liens. Aucune donnee personnelle n'est transmise a Amazon par BookZam ; seule votre localisation (pays) est utilisee localement pour vous orienter vers la bonne boutique Amazon.
- **Aucune donnee n'est vendue a des tiers**

## 3. Services tiers

BookZam utilise les services tiers suivants :

| Service | Finalite | Donnees transmises |
|---------|----------|--------------------|
| **Firebase Authentication** | Connexion securisee | Email, nom, identifiant de connexion |
| **Cloud Firestore** | Stockage des donnees | Bibliotheque, profil, progression |
| **Firebase Analytics** | Statistiques d'usage | Evenements anonymises, proprietes utilisateur |
| **Firebase Crashlytics** | Rapports de crash | Traces d'erreur, infos appareil |
| **Firebase Cloud Messaging** | Notifications push | Jeton FCM |
| **Firebase Remote Config** | Configuration dynamique | Aucune donnee personnelle |
| **Firebase App Check** | Protection anti-fraude | Attestation d'appareil |
| **Google Generative AI (Gemini)** | Fonctionnalites IA | Textes de recherche, contexte bibliotheque |
| **RevenueCat** | Gestion des abonnements | Identifiant utilisateur, statut d'abonnement |
| **Google AdMob** | Publicites | Identifiant publicitaire (GAID/IDFA) |
| **Google Books API** | Recherche de livres | Termes de recherche (titre, auteur, ISBN) |
| **Open Library** | Recherche de livres | Termes de recherche |
| **Library of Congress** | Recherche de livres (fallback) | Termes de recherche |
| **LibriVox** | Audiobooks gratuits | Titre, auteur |
| **Google ML Kit** | OCR (sur l'appareil) | Aucune — traitement local uniquement |

En cas d'activation de tests comparatifs (shadow testing), vos requetes IA peuvent egalement etre traitees par Anthropic (Claude) en parallele de Gemini.

## 4. Stockage et securite

- Les donnees sont stockees sur **Google Firebase** (infrastructure securisee, chiffrement en transit et au repos)
- Les donnees locales (cache, preferences) sont stockees sur votre appareil via SharedPreferences et sqflite (non chiffrees)
- Les images capturees par la camera sont stockees temporairement sur votre appareil et ne sont pas envoyees a nos serveurs (sauf pour l'analyse d'etagere via Gemini Vision, le cas echeant)

## 5. Publicites

- Les utilisateurs **gratuits** voient des bannieres publicitaires fournies par Google AdMob
- Les utilisateurs peuvent regarder des **publicites recompensees** (rewarded ads) pour obtenir des recherches IA supplementaires
- Les utilisateurs **Premium** ne voient aucune publicite
- Google AdMob peut collecter des identifiants publicitaires (GAID sur Android, IDFA sur iOS) pour personnaliser les annonces
- Sur iOS, une demande de consentement (App Tracking Transparency) vous sera presentee avant toute collecte d'identifiant publicitaire

## 6. Notifications

- BookZam peut envoyer des notifications push pour les rappels de lecture, les series de lecture, les defis, les recommandations et les mises a jour
- Vous pouvez desactiver chaque categorie de notification individuellement dans les parametres de l'application
- Vous pouvez vous desabonner completement des notifications a tout moment

## 7. Profil public et donnees sociales

- Certaines informations de votre profil sont visibles par les autres utilisateurs : pseudo, niveau de lecture, genres preferes, nombre de livres, badges
- Le fil d'activite (livres ajoutes, defis completes, badges) est visible par tous les utilisateurs connectes
- Les messages de clubs de lecture sont visibles par les membres du club
- Vous pouvez controler la visibilite de votre profil dans les parametres

## 8. Droits des utilisateurs

Conformement au RGPD et aux lois applicables, vous pouvez :
- **Acceder** a vos donnees personnelles
- **Rectifier** vos informations
- **Supprimer** votre compte et toutes vos donnees — disponible directement dans l'application (Parametres > Compte > Supprimer mon compte)
- **Exporter** vos donnees — disponible directement dans l'application (Parametres > Compte > Exporter mes donnees) au format JSON
- **Retirer votre consentement** pour les notifications et la localisation via les parametres de l'application

Pour exercer ces droits, vous pouvez utiliser les fonctionnalites integrees a l'application ou nous contacter a **contact@bookzam.io**

## 9. Conservation des donnees

- Les donnees de votre compte sont conservees tant que votre compte est actif
- En cas de suppression de compte, vos donnees sont effacees sous 30 jours
- Les logs de crash sont conserves 90 jours
- Les evenements analytics sont conserves selon la politique de retention de Firebase (14 mois par defaut)

## 10. Enfants

BookZam n'est pas destine aux enfants de moins de 13 ans. Nous ne collectons pas sciemment de donnees personnelles d'enfants. Si vous etes parent et pensez que votre enfant nous a fourni des donnees, contactez-nous a contact@bookzam.io.

## 11. Modifications

BookZam peut mettre a jour cette politique. En cas de changement majeur, nous vous en informerons via l'application ou par e-mail. La date de derniere mise a jour est indiquee en haut de ce document.

## 12. Contact

Pour toute question ou demande concernant vos donnees :
- Email : **contact@bookzam.io**
- Vous pouvez egalement utiliser la fonctionnalite de feedback dans l'application (Parametres > Feedback)
