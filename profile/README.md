<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->




<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/Commu-net">
    <img src="./assets/Communet-b_0tT9y4.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Communet</h3>

  <p align="center" >
    The open source bulk mailing utility for all your needs
    <br />
    <br />
    <br />
    <a href="https://job-radar-frontend.vercel.app/">Liv link</a>
    <a href="https://www.canva.com/design/DAGAffZePfQ/EVEkFAsayl-9iU5-8A9PEw/edit?utm_content=DAGAffZePfQ&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton">Presentation </a>
    <a href="https://www.youtube.com/watch?v=HaZUgfIjxb4">View Demo</a>
    ·
    <a href="https://github.com/JobRadar-ai/JobRadarFrontend">Report Bug</a>
    ·
    <a href="https://github.com/JobRadar-ai/JobRadarFrontend">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      About The Project
      <ul>
        <li>Built With</li>
      </ul>
    </li>
    <li>Usage</li>
    <li>Contributing</li>
    <li>License</li>
    <li>Developers</li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About  

<img src="./assets/home_page.png" alt="Logo" width="800" height="auto">

Communet is a cutting-edge open source platform dedicated to automating and enhancing outreach efforts for businesses, marketers, and individuals alike. With a focus on automation, personalization, and scalability, Communet offers a comprehensive suite of tools to streamline emails and facilitate communication with target audiences empowering users with intuitive solutions that optimize time efficiency and drive meaningful engagement.

Here's why you shoudld consider using communet:
* Your time is precious, and to optimize it, you write and we handle the email sending process for you.
* You can manage your receipients at your convinence .
* Last but not the least you can add personalization to your mail to keep it unique to everyone.






### Built With

These are some of the utilities frameworks languages and tools that we used to build the platform.

<div>
  <img src="./assets/react.png" height="80px">
  <img src="./assets/typescript.png" height="80px">
  <img src="./assets/javascript.png" height="80px">
  <img src="./assets/redux.png" height="80px">
  <img src="./assets/shadcn.png" height="80px">
  <img src="./assets/css.webp" height="80px">
  <img src="./assets/taliwind.png" height="80px">
  <img src="./assets/zod.png" height="80px">
  <img src="./assets/lottie.png" height="80px">


  <img src="./assets/vercel.png" height="80px">
  <img src="./assets/vite.png" height="80px">
  <img src="./assets/node.png" height="80px">
  <img src="./assets/express.png" height="80px">
  <img src="./assets/mongo.png" height="80px">
  <img src="./assets/python.png" height="80px">
  <img src="./assets/nginx.png" height="80px">
  <img src="./assets/aws.png" height="80px">
  <img src="./assets/gcp.png" height="80px">




</div>

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

Clone the repo and navigate to the  ```Mailer_frontend``` path and install all the dependencies
* Installing dependencies
  ```sh
  npm install 
  ```

* Run the app
  ```sh
   npm run dev
   ```

* navigate to ```localhost:5173``` to visit the locally set up project

<!-- USAGE EXAMPLES -->
## Usage

Here are some simple steps, following which you can use th platform at it's full potential

### 1 Visit the website of communet 
 <img src="./assets/home_page.png">

### 2 Read the documentation at resources page to get started 
 <img src="./assets/documentation_page.png">

 ### 3 Login to communet using Google
 <img src="./assets/login_page.png">

 ### 4 Navigate to dashboard 
 <img src="./assets/dashboard_page.png">

 ### 5 Add profile
 1. you can add profile by manual entry
 <img src="./assets/create_profile.png">
 2. you can also add profiles by excel files
 <img src="./assets/import_profile_from_excel.png">
 3. you can also add profiles usig our profile scraper extension 
  <img src="./assets/get_profile_from_extension.png">

 ### 6 Select the profiles to send mail to 
 <img src="./assets/select_profile.png">

 ### 7 compose mail and send to all selected profiles at once
 <img src="./assets/compose_mail.png">

 ### 8 Edit and delete profiles
  1. Edit the profile using actions for the profile 
<img src="./assets/Edit_profile.png">

 2. Delete the profile using actions for the profile 
<img src="./assets/delete_profile.png">




## Server local Installation

1. Clone the Repository ```bash git clone https://github.com/JobRadar-ai/JobradarBackend ```

2. Install nx globally ```bash npm i -g nx ```  

3. Build the containers for each Service. ```bash docker-compose up --build ```

4. User Endpoints 
  


## Endpoints

### Home
- **URL:** `/`
- **Method:** `GET`
- **Description:** Returns a link to the Google authentication route.

### Google Authentication
- **URL:** `/auth/google/`
- **Method:** `GET`
- **Description:** Initiates the Google authentication process. The scope of the authentication includes the user's profile, email, and the ability to compose Gmail messages. The access type is set to 'offline', and the approval prompt is set to 'force'.

### Google Authentication Callback
- **URL:** `/auth/google/callback/`
- **Method:** `GET`
- **Description:** Callback route for Google to call after authentication. If the authentication is successful, the user is redirected to the Google success route. If the authentication fails, the user is redirected to the Google failure route.

### Google Authentication Success
- **URL:** `/auth/google/success`
- **Method:** `GET`
- **Description:** Handles successful Google authentication. The user's email, name, sub, and id are returned as query parameters in a redirect to the client URL.

### Google Authentication Failure
- **URL:** `/auth/google/failure`
- **Method:** `GET`
- **Description:** Handles failed Google authentication. Returns an error message stating that the user is not authenticated.

### Logout
- **URL:** `/logout`
- **Method:** `GET`
- **Description:** Logs out the current user. If the user has an active session, the session is destroyed. The user is then logged out, and a success message is returned.

### Get User Data
- **URL:** `/getuser`
- **Method:** `GET`
- **Headers:** `Authorization: Bearer <token>`
- **Description:** Retrieves data for the current user. The user must be authenticated and provide a valid token in the Authorization header. If the user is found in the database, their data is returned. If the user is not found or not authenticated, an error message is returned.

5. Email Endpoints


## Base URL
The base URL for these endpoints is `http://localhost:/email`.

## Endpoints

### Send Mass Email with Attachments
- **URL:** `/send`
- **Method:** `POST`
- **Description:** Send mails with attachments.
- **Request Body:**
  - `emails`: Array of email addresses to send mails to.
  - `sender`: Email address of the sender.
  - `subject`: Subject of the email.
  - `text`: Body of the email.
  - Files to be attached.

### Manage Email
- **URL:** `/mail`
- **GET Method:** `GET`
- **Description:** Get all emails associated with a user.
- **Query Parameters:**
  - `userEmail`: Email address of the user.
- **POST Method:** `POST`
- **Description:** Add new email(s) to a user's account.
- **Request Body:**
  - `userId`: ID of the user.
  - `data`: Array of email objects containing the following fields:
    - `email`: Email address.
    - `currentDesignation`: Current designation (optional).
    - `name`: Name (optional).
    - `company`: Company (optional).
- **DELETE Method:** `DELETE`
- **Description:** Remove an email from a user's account.
- **Request Body:**
  - `userId`: ID of the user.
  - `_id`: ID of the email to remove.
- **PUT Method:** `PUT`
- **Description:** Update an existing email associated with a user.
- **Request Body:**
  - `userId`: ID of the user.
  - `data`: Object containing the following fields:
    - `_id`: ID of the email.
    - `email`: Email address.
    - `currentDesignation`: Current designation (optional).
    - `name`: Name (optional).
    - `company`: Company (optional).

### Store Mail
- **URL:** `/mail/store-mail`
- **Method:** `POST`
- **Description:** Store email(s) in a user's account.
- **Headers:** `Authorization: Bearer <token>`
- **Request Body:**
  - `emails`: Array of email addresses to store.





<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>





Project Link: [https://job-radar-frontend.vercel.app/](https://job-radar-frontend.vercel.app/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>






<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 

