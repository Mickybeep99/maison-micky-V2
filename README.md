# Maison Micky V2
Prototype exécutable sans identifiants externes.

## Inclus
- UI responsive bleu/bordeaux/rouge
- catalogue et stock persistant (`data/db.json`)
- clients et commandes
- réservation/décrémentation du stock à la commande, restauration sur échec/annulation
- Wave direct (activé dès ajout de `WAVE_API_KEY`)
- Orange Money isolé derrière un connecteur configurable
- espèces à la livraison
- statuts paiement + préparation/livraison
- tableau de bord
- architecture notification WhatsApp Business avec aperçu avant connexion

## Lancer
`npm install` puis `npm start`, ouvrir http://localhost:3000

## À connecter pour la production
Wave Business/API + validation de signature webhook; identifiants/API marchand Orange Money; Meta WhatsApp Business; hébergement HTTPS et base PostgreSQL/Supabase. Le JSON local est adapté au prototype, pas à la production multi-utilisateur.
