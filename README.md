# React application using giflow and automate task with Github actions

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

## Branches in this repo

### `Main`

### `gh-pages`

gh-pages is used as a release branch

### `Developer`

### `Feature/<name>`

## tags format
- v1.1 &rarr first feature
- v1.2 &rarr second feature

## Workflows

All of the new worflows are stored in the root of the project in the next path: ./github/worflows

This are the workflow for the next project

### `Deploy`

This workflow is use to deploy the application into github pages. Will install of node dependencies, build source code. The test that are running are just an echo to show a message

For any events like PUSH or PULL REQUEST in the branch MAIN.

### `pull_request_dev`

For any push or pull request in the branch DEVELOP will run a echo to show a message that a test is running. Take the branch MAIN as a destination and the branch that make a push or pull request.

### `pull_request_dev`

Performs the same functionality as " pull_request_dev ". The only difference is that it will only trigger when a push event happens in any of the future branchs.

Pull request to the DEVELOP branch.

## Flow of the project

when a new feature is in development it should be developed in a new feature branch with the format. Then push all the changes in the repository. A workflow will be trigger to create a pull request. If the pull request is accepted and the changes is merged in DEVELOP another workflow will be trigger to create a pull request to add the changes in MAIN to release the new feautre 









