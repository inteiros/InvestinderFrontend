# InvestinderFrontend

This repository contrains the Back-end and Front-end application from InvesTinder!

InvesTinder is an open-source application developed in JavaScript using ReactJS by João Gabriel Eler Mendes and Victor Lomba to compete in a Hackaton.

This application lets investors connect easily with consultants or advisors, leting them match if they like each other's profile and then providing contact information.

InvesTinder is still on development, so many other features might be added later.

## Info

The back-end application was made using Node.js, and it contains the services that are used and it is responsible for the communication with the database.

The front-end was developed with the ReactJS framework.

## Usage

The Login page is the main page, while on it, you can navigate to the account creation page. Once the account is created, the application displays a toast indicating if the operation was a success or if there was an error, and if it was a success, the user is redirected to the main page where he can login.

Once the user is logged, a Json Web Token is created and saved in local storage, where it can remain for 1 day. It means that if the user closes the application and then reopen it later, he will be already logged in.

On the dashboard page, a card will be displayed with some info about the person on it. If the user is an investor, the person displayed will be either a consultant or an advisor, and the user will show up in their dashboard.

In this card, the information displayed is: the name, bio and interests/company name. The bio is used to get to know better about one's profile and personality.

The user can choose either to like or dislike the person that is in the card. In case the user disliked someone not on porpouse or regreted it, the person that was disliked is not blocked from the user, that means the person can be shown later on.

When liking a account, the account's id is stored on the 'likes' table of the user at the database, and in case the person in that account likes the user back, they will be stored in the 'matches' table, and they will get authorization to see each others contact information.

After they get this authorization, the contact information will be displayed on the 'matches' page, and then they can use the number and e-mail displayed to contact each other and do proper business.

This way, the application eases the customers capitation, the acknowledgement of the investor's risk profile and lets less experienced people enter in the finance fields, expanding its area.
