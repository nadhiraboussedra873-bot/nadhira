
## Code de vérification par e-mail à la connexion
La connexion envoie un code à 6 chiffres (Supabase Auth > e-mail OTP). Dans Supabase : Authentication > Email Templates > « Magic Link », ajoutez `{{ .Token }}` dans le message (ex. « Votre code : {{ .Token }} »). L'envoi d'e-mails par défaut de Supabase est très limité : configurez un SMTP personnalisé pour de vrais utilisateurs.
