# Deploying Applications

**1.** What is the package.json file used for?

<!-- enter you answer in the space below -->

```
To record important metadata about a project which is required before publishing to NPM, and also defines functional attributes of a project that npm uses to install dependencies, run scripts, and identify the entry point to our package. *Note, this was not covered in the prior readings nor covered in class this week so I am doing my best to answer using google. I might recommend syncing these quizzes with the material that is actually being covered.
```

**2.** At what level of your project do you need package.json when deploying your application? Why?

<!-- enter you answer in the space below -->

```
It is housed in the root directory of the project because it holds important information about the project, like the project name, description, and functional metadata like the package version number, and a list of dependencies required by the application. *Note, this was not covered in the prior readings nor covered in class this week so I am doing my best to answer using google. I might recommend syncing these quizzes with the material that is actually being covered.
```

**3.** What command will ensure that your Vue code is compiled properly for deployment?

<!-- enter you answer in the space below -->

```
npm run build? *Note, this was not covered in the prior readings nor covered in class this week so I am doing my best to answer using google. I might recommend syncing these quizzes with the material that is actually being covered.
```

**4.** **\_\_\_** are used to provide your application with specific data based on it's environment. For example: connections strings, private keys or port. Fill in the blank.

<!-- enter you answer in the space below -->

```
.env
```

**5.** What are the two ways to view the logs from your Heroku app.

<!-- enter you answer in the space below -->

```
The Heroku CLI, the dashboard, your logging add-on, or in your log drain. *Note, this was not covered in the prior readings nor covered in class this week so I am doing my best to answer using google. I might recommend syncing these quizzes with the material that is actually being covered.
```

**6.** How do you update an app already deployed on Heroku?

<!-- enter you answer in the space below -->

```
1. Download & install Heroku CLI
2. Clone your repository
3. Make your changes
4. Deploy your changes
5. Switch default branch from master to main
6. Delete the old branch locally
7. Reset the GIT repository hosted on the Heroku
8. Redeploy the application
*Note, this was not covered in the prior readings nor covered in class this week so I am doing my best to answer using google. I might recommend syncing these quizzes with the material that is actually being covered.
```

**7.** Why is branching important to version control?

<!-- enter you answer in the space below -->

```
Branching allows teams of developers to collaborate inside of one central code base. When a developer creates a branch, the version control system creates a copy of the code base at that point in time. Changes to the branch don't affect other developers on the team. *Note, this was not covered in the prior readings nor covered in class this week so I am doing my best to answer using google. I might recommend syncing these quizzes with the material that is actually being covered.
```

**8.** When should code review happen?

<!-- enter you answer in the space below -->

```
Code reviews should happen after the automated checks have completed successfully, but before the code merges to the repository's mainline branch.
```

**9.** What is the term used to define combining two branches?

<!-- enter you answer in the space below -->

```
Merging.
```
