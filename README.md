# Sistemi i Takimeve me Mjeke duke perdorur MERN stack

Ky projekt eshte nje aplikacion web full-stack i ndertuar duke perdorur teknologjine MERN (MongoDB, Express.js, React.js dhe Node.js) per te ofruar nje sistem efikas dhe miqesor per perdoruesin ne menaxhimin e takimeve me mjeke. Pacientet mund te kerkojne mjeke sipas specialitetit, vendndodhjes ose disponueshmerise, te rezervojne takime, te shohin historikun e tyre te takimeve dhe te menaxhojne informacionin e profilit te tyre. Mjeket mund te menaxhojne oraret e tyre, te shohin informacionin e pacienteve dhe te perditesojne statusin e takimeve.

## Teknologjite

- **Front-end:** React.js
- **Back-end:** Express.js, Node.js
- **Baza e te dhenave:** MongoDB
- **Varesi te tjera:** Axios, Redux, Moment, Ant Design, Bootstrap

## Instalimi dhe Konfigurimi

1. Klononi projektin:

   ```bash
   git clone https://github.com/Omega-me/projekti_web
   ```

2. Instaloni varesite:

   ```bash
   bun install (prferohet per shkak te shpejtesise qe ofron)
   # ose
   npm install
   # ose
   yarn install
   ```

3. Krijoni nje file `.env` ne root folder dhe vendosni variablat e meposhtme:

   ```env
   PORT=8080
   NODE_MODE=development
   MONGO_URL=linku_i_bazes_se_te_dhenave_mogodb
   JWT_SECRET=kodi_secret_i_jwt
   ```

4. Nisni aplikacionin ne menyre zhvillimi:
   ```bash
   bun dev (preferohet starton ne te njejten kohe serverin dhe klientin)
   # ose
   npm run dev
    # ose
   yarn dev
   ```

## Karakteristikat Kryesore dhe perdorimi

- Regjistrimi
- Regjistrimi dhe menaxhimi i profilit per mjeket
- Kerkim dhe rezervim takimesh
- Anulim dhe riplanifikim i takimeve
- Historik i takimeve dhe njoftime per perdoruesit
- Autentifikim dhe autorizim i sigurt
- Dizajn i pergjegjshem dhe i lehte per perdorim

1. Hapni aplikacionin ne shfletuesin tuaj ne:

   ```
   http://localhost:3000
   ```

2. Regjistrohuni me email dhe password, dhe nese sistemi nuk ka nje admin, per tu bere admin duhet ndryshuar vete ne databaze **isAdmin:true**,

3. Cdo perdorues qe rregjistorhet eshte i rregjistruar si **pacient** si fillim, dhe pacienti mund te aplikoje per tu bere **mjek** pastaj nese eshte i interesuar te jete i rregjistruar si mjek i cili aprovohet ose refuzohet nga admini,

4. **Pacienti** mund te skeduloje takime me mjekte te ndryshem qe i shfaqen nga sistemi dhe eshte **mjeku** qe aprovon ose refuzon takimin

5. **mjeku** mund te shikoje te gjitha takimet qe nje **klientet** kan kerkuar dhe approvoje ose refuzoje na varesi te ngarkeses qe mund te kete

6. **Pacienti** ndjek ecurine e takimit te skeduluar nese eshte aprovuar apo refuzuar.

7. **Admini** mund te shikoje listen e **mjekeve** ku mund te heq te drejten per te qene mjek ne plateforme, te aprovoje kerkesen per tu bere mjek nese ka marre nje kerkese

8. **Admini** mund te shikoje listen e te gjithe pordoruesve ku perfshihen **pacientet** dhe **mjeket** dhe mund tju bllokoje aksesin ne sistem nese thyhen rregullat e percaktuara.

## Test accounts

- Admin email:admin@gmail.com password:12345678
- Doctor 1 email:doctor1@gmail.com password:12345678
- Doctor 2 email:doctor2@gmail.com password:12345678
- Doctor 3 email:doctor3@gmail.com password:12345678
- Pacent 1 email:pacient1@gmail.com password:12345678
- Pacent 2 email:pacient2@gmail.com password:12345678
- Pacent 3 email:pacient3@gmail.com password:12345678
- Pacent 4 email:pacient4@gmail.com password:12345678
