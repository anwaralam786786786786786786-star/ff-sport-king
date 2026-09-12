BIHAR FF SPORT - Firebase Connected (Google Login)

This version connects the user app to Firebase Authentication and Firestore.

Enabled in the app:
- Email/Password login and signup
- Continue with Google (mobile-friendly redirect flow)
- Automatic users/{UID} profile creation
- Role=User and Coins=0 for new user profiles

Firebase project: bihar-ff-sport
Hosting site: bihar-ff-sport

Deploy from this project folder:
firebase login
firebase use bihar-ff-sport
firebase deploy --only hosting

Important:
- Google provider must be enabled in Firebase Authentication and a support email selected.
- Do not trust a client-side Role field for admin access in production. Use secure backend/custom claims and Firestore rules.
- Do not credit wallet coins from client-side payment claims alone. Use server-side payment verification/webhooks.
- Google sign-in uses Firebase Authentication; the app never receives or stores the user's Google password.
