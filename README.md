# Demande d'appel — élèves Skool d'Anthony Sirius

Site à part de la page de vente. Une seule page (`index.html`, CSS et JS dedans,
sans build), à la charte d'Anthony (noir, blanc, rouge #AE0000, Anton + Poppins
en local).

Plus de calendrier depuis le 12/11/2026 : un formulaire (prénom, nom, e-mail,
numéro WhatsApp). Le lead tombe dans les **Leads du jour** de l'équipe Base44 du
CRM (`~/CRM Sirius`), avec `offre = 'skool'` : le CRM lui met la pastille rouge
« Skool », le sales applique la trame Skool (SQL `CRM Sirius/supabase/26-leads-skool.sql`).

Message après l'envoi, selon l'heure de Paris (réglage `NUIT` en tête du script) :
- de 9 h à 23 h : un membre de l'équipe appelle dans les minutes à suivre ;
- de 23 h à 9 h : un membre de l'équipe appelle dès demain matin.
Dans les deux cas : ne pas prendre l'abonnement Base44 avant l'appel.

Les anciens liens perso (`/<code>`) affichent le même formulaire.
`?ref=xxx` (ou `?src=xxx`) est gardé dans `source`.

En local : `python3 -m http.server 8195` puis http://localhost:8195/.
