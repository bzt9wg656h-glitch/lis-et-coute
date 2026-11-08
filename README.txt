CLAIRLIRE — prototype de recherche, pas encore validé pour le TFE.

Pour tester : déposer les fichiers du dossier à la racine d'un nouveau dépôt GitHub public, activer Settings > Pages > Deploy from branch > main / root, puis ouvrir l'URL HTTPS sur Safari iPad et Chrome Android. Ne pas ouvrir en file:// : le stockage et certaines bibliothèques peuvent ne pas fonctionner.

Fonctions : catégories personnalisées avec emoji, documents séparés par appareil, stockage IndexedDB, export/restauration JSON, photo originale, PDF original, OCR français Tesseract.js, lecture française Web Speech API, double surlignage approximatif sur les documents.

LIMITES IMPORTANTES :
- La lecture mot par mot dépend des événements onboundary du moteur vocal. Safari/iPad peut ne pas les transmettre : dans ce cas le surlignage reste sur le premier mot. Ce prototype ne garantit donc PAS le suivi fiable de NaturalReader.
- Les coordonnées des mots PDF sont approximatives (polices, tableaux, plusieurs colonnes) ; OCR sur photos/PDF peut être imprécis et l'ordre de lecture erroné.
- L'OCR français, PDF.js et Tesseract.js sont chargés par Internet (CDN). L'OCR peut être lent sur tablette. Un PDF multipage long peut utiliser beaucoup de mémoire.
- La voix dépend du navigateur/appareil et peut être moins naturelle que NaturalReader.
- Le stockage local peut être effacé par l'utilisateur ou le système. Utiliser Sauvegarder régulièrement et conserver le fichier JSON ailleurs.
- Ne pas importer de documents contenant des données personnelles sensibles pendant les essais sans vérifier les règles de confidentialité du terrain de stage.
- Pas de validation sur appareils physiques effectuée. Tester avant toute utilisation avec des participants.
