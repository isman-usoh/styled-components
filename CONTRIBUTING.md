Thanks for giving this a read! We're always open to your contributions to styled-components.
This document will get you started on how to contribute and things you should know.
So please give it a thorough read.

Please also give the code of conduct a read.

## How do I contribute code?

1. Find some issue you're interested in, or a feature that you'd like to tackle.
  Also make sure that no one else is already working on it. We don't want you to be
  disappointed.

2. Fork, then clone: `git clone https://github.com/YOUR_USERNAME/styled-components.git`

3. Create a branch with a meaningful name for the issue: `git checkout -b fix-something`

4. Make your changes and commit: `git add` and `git commit`

5. Make sure that the tests still pass: `npm test` and `npm run flow` (for the type checks)

6. Push your branch: `git push -u origin your-branch-name`

7. Submit a pull request to the upstream styled-components repository.

8. Choose a descriptive title and describe your changes briefly.

9. Wait for a maintainer to review your PR, make changes if it's being recommended, and get it merged.

10. Perform a celebratory dance! :dancer:

## How do I set up the project?

Run `npm install` and edit code in the `src/` folder. It's luckily very simple! :wink:

## How do I verify and test my changes?

To make development process easier, you could use a sandbox provided in this repo.
To use the sandbox, follow these steps:

1. Go to sandbox folder: `cd sandbox`

2. Install all the dependencies: `yarn install` or `npm install`

3. Run `yarn start` or `npm start` to start sandbox server

Now you should have the sandbox running on `localhost:3000`

Sandbox supports client-side and server-side rendering.

You can use an interactive editor, powered by [`react-live`](https://react-live.philpl.com/), to
test your changes. But if you want more control, you can edit the sandbox itseft:

- Root `<App>` componens is located at `styled-components/sandbox/src/App.js` file

- Client-side entry point is at `styled-components/sandbox/src/browser.js`

- Server-side entry point is at `styled-components/sandbox/src/server.js`

In the sandbox source, `styled-components` is an alias to `styled-components/src` folder,
so you can edit the source directly and dev-server will handle rebuilding the source and
livereloading your sandbox after the build is done.

When you commit our pre-commit hook will run, which executes `lint-staged`. It will run
the linter automatically and warn you, if the code you've written doesn't comply with our
code style.
