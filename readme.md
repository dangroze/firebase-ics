npm i firebase-tools -g
put this inside the '~/.bash_profile' file
alias firebase="`npm config get prefix`/bin/firebase"
firebase init hosting
create firebase project on https://console.firebase.google.com
firebase use --add
index.html - delete the style in head and everything in body and add <script src="app.js">
touch public/app.js
document.addEventListener("DOMContentLoaded", event => {
  const app = firebase.app();
  console.log(app)
})
