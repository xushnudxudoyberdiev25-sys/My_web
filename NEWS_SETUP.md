Kaizen Online News setup

The HTML is already prepared for Firebase Authentication + Firestore + Storage.

Open Firebase Console and create a project.

Add a Web App to the project.

Copy the Firebase Web App config.

In Вставленный код(3).html, find FIREBASE_CONFIG and replace all YOUR_... values.

Set FIREBASE_ADMIN_EMAIL to the admin email address.

Firebase Authentication -> Sign-in method -> enable Email/Password.

Authentication -> Users -> add the admin user using that email and the password you want to type in the existing Admin login screen.

Create a Cloud Firestore database.

Create a Storage bucket.

Replace ADMIN_EMAIL in FIREBASE_RULES.txt with the admin email and paste the Firestore rules into Firestore Rules and the Storage rules into Storage Rules.

Upload the updated HTML to the GitHub Pages repository.

The existing Admin username remains Xushnud_. The password is no longer hard-coded in the HTML; it is checked by Firebase Authentication.

Guests can read published news. Only the Firebase admin email can create, update, or delete news.
