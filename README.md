## Passageway Web

#### Getting started

1. Copy the project to your local machine:  
`git clone https://github.com/Passageway/PassagewayWeb.git passageway-web`
2. `cd passageway-web`
3. Allow access to the following scripts: `chmod u+x init/deploy init/ubuntu_prepare init/deploy`
4. Run `init/ubuntu_prepare`
5. Once complete, run `firebase login` and `firebase add --project <passageway-project-id>`
6. From there, run `firebase open` to run locally, or run `init/deploy` to deploy to the Firebase hosting instance


#### Futher Reference
* [Firebase hosting quickstart][firebase_qs]
* [Polymer CLI][polymer_cli]


[firebase_qs]: https://firebase.google.com/docs/hosting/quickstart
[polymer_cli]: https://www.polymer-project.org/1.0/docs/tools/polymer-cli
