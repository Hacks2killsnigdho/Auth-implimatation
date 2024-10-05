# Auth-implimatation
Adding additional profile information->
TWO ADDITIONAL INFORMATION CAN BE TO THE USER INFORMATION AS FOLLOWS:
1. Display Name
To add full name or any name for the purpose of displaying in the application.
2. Photo URL
To add the url of the photo that can be used as profile picture.


// Fetching the current user
const user = firebase.auth().currentUser;

// Fetching value from a html input fields with id
const displayName = document.getElementById("name").value;
const photoURL = document.getElementById("photo").value;

// Updating additional information
user.updateProfile({
  displayName,
  photoURL
})
