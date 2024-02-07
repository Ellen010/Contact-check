# Contact-check
//Java basics
const contacts = [
  {
    firstName: "Andrew",
    lastName: "Bowes",
    cellphone: "8504506978",
    likes: ["Sports", "Pizza", "Traveling"],
  },
  {
    firstName: "Melissa",
    lastName: "Knowles",
    cellphone: "7204563879",
    likes: ["Cosmo", "Mountaines", "Yoga"],
  },
  {
    firstName: "Scott",
    lastName: "Roberts",
    cellphone: "5783204569",
    likes: ["Real estate", "Guitar", "Cars"],
  },
  {
    firstName: "Larsa",
    lastName: "Marshalls",
    cellphone: "2560057865",
    likes: ["Dancing", "Traveling"],
  },
];

function findContact(name, feature) {
  // Finds the contact
  for (let i = 0; i < contacts.length; i++) {
    if (contacts[i].firstName === name) {
      // Checks the contact features
      if (contacts[i].hasOwnFeature(feature)) {
        return contacts[i][feature]; // Returns the features
      } else {
        return "No such feature";
      }
    }
  }

  // If the loop completes without finding the contact, return "Contact doesn't present"
  return "No such contact";
}
