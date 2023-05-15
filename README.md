**Postman + newman + github actions**
## Project description
- This project contains integration tests created in Postman, based on a simple store template.
- It also includes a GitHub action to run the `petstore.collection.json` on GitHub pages.

## Technologies Used
- Node.js
- Newman
- newman-reporter-htmlextra
- Postman

## Project set up

To set up the project, follow these steps:

1. Clone the project `git clone https://github.com/AvatarasS/Postman_ghActions.git`
2. Install Node.js dependencies: `npm i` 

## Running Postman Tests
 To run `store.collection.json` in Postman:
1. Start the local testing server: `npm run tern-on-api`
2. Import `store.collection.json` into Postman
3. Click the `Runner`
4. Drag one of the folders from the `store collection` into the `RUN ORDER` field
5. Press the `Run store` button

## Running Newman Tests
- To run the collection through the command line
 `newman run {{name}}.collection.json`
- To create a new report in the ./docs directory 
 `newman run {{name}}.collection.json -r htmlextra --reporter-htmlextra-export results/index.html`

## GitHub Pages:

To view the generated HTML report for  `petstore.collection.json`:
- Go to the [report](https://avatarass.github.io/Postman_ghActions/) on GitHub pages.
