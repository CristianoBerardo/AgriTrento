<div align="center">
  <img src="./Deliverables/Logo/AgriTrentoSlogan.svg" alt="Logo di AgriTrento" width="400">
  <p> 
   <div align="center">
      <strong><a href="https://agritrento-rhzf.onrender.com/home">AgriTrento</a></strong> a web platform that facilitates the ordering and sale of fruit and vegetables from the Trento farmers' market, encouraging the consumption of local, seasonal produce and fostering sustainable practices that respect our local area.
   </div>
</div>

<br><br>

# Prerequisiti

- [Node.js](https://nodejs.org/en/) v20.17.0
- [npm](https://www.npmjs.com/) v10.8.2


# Instructions for local execution

1. Make sure you have installed Node and npm. You can verify this by running the following command in your terminal:

   ```bash
   node -v
   npm -v
   ```

1. Clone the repository
1. Enter the project folder and install the necessary modules from the terminal:

   ```bash
   npm run install:all
   ```

1. Create a MongoDB database

1. Create a Firebase database
   
1. Add the `.env` file in "/backend/":

   ```bash
   PORT=3000
   MONGODB_URI=mongodb+srv://...
   JWT_SECRET=JWT_SECRET
   ```

1. Add the file `serviceAccountKey.json` in "/backend/config/". To find it connect to [console.firebase.google.com](https://console.firebase.google.com/) > Project > Settings ⚙️ > Service account > Generate a new private key 
   
   This will download a JSON file. Copy the file's contents and paste them into the file `serviceAccountKey.json`. The file should look like this:

   ```json
       {
         "type": "...",

         "project_id": "...",

         "private_key_id": "...",,

         "private_key": "...",

         "client_email":  "...",

         "client_id":  "...",

         "auth_uri":  "...",

         "token_uri":  "...",

         "auth_provider_x509_cert_url":  "...",

         "client_x509_cert_url":  "...",

         "universe_domain":  "..."
     }

   ```

2. Run the follow command on your terminal

   ```bash
   npm run dev
   ```

3. Check the terminal and open this link [http://localhost:5173/](http://localhost:5173/) on your preferred browser to see the web-application

<br>

# Deployment diagram


<div align="center">
  <img src="./Deliverables/fourth-deliverable/img/DiagrammaAgriTrento.drawio.svg" alt="Diagramma del deployment">
  <p>AgriTrento's deployment diagram</p>
</div>
