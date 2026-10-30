# Réservation d'un appel — équipe Skool d'Anthony Sirius

Site à part de la page de vente : on y réserve un appel avec l'équipe Skool.
Une seule page (`index.html`, CSS et JS dedans, sans build), à la charte
d'Anthony (noir, blanc, rouge #AE0000, Anton + Poppins en local).

- **La racine** = le lien de l'équipe, le même pour tous les setters : tous
  les créneaux où au moins un setter Skool est libre (leurs dispos du CRM),
  et l'appel va au setter libre à l'heure choisie.
- `/<code>` ne montre qu'un setter (`staff.rdv_code`, ex. `/mathis`).

La page lit et écrit dans le Supabase d'Anthony (`mmpazpnzkmianenkfyiv`, le
même que la page de vente et `~/CRM Sirius`) par deux fonctions publiques,
`rdv_calendrier` et `rdv_reserver` (`CRM Sirius/supabase/02` et `03`). Le lead
arrive dans l'équipe Skool, onglet **Rendez-vous** du setter.

En local : `python3 -m http.server 8195` puis http://localhost:8195/.
Aperçu avec de faux créneaux : vider `SUPABASE_URL` et ouvrir `/?apercu`.
