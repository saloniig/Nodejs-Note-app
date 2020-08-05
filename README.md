# Note-App

A Command line note app based on node.js

# Requirements

-   Node.js
-   yargs
-   chalk

# Installation

Clone this repository to your local computer and follow the steps below:

$ cd notes-app
$ npm install
## Instructions

The entry point of this app is  **app.js**. Run the script in the format  `node app.js [command] [options]`. The commands that are currently supported are:

-   `add`
    -   Adds a note.
    -   Parameters need are  `--title`  and  `--body`.
    -   Example:  `node app.js add --title="title goes here" --body="body goes here"`
-   `list`
    -   All the notes are listed.
    -   No parameters are needed.
    -   Example:  `node app.js list`
-   `read`
    -   Reads a note.
    -   Parameter need is  `--title`.
    -   Example:  `node app.js read --title="title goes here"`.
-   `remove`
    -   Removes a note.
    -   Parameter need is  `--title`.
    -   Example:  `node app.js remove --title="title goes here"`.
-   Show help: You can pass  `help`  argument to see all the commands with their description.

```
  $ node app.js --help
  app.js [command]

  Commands:
    app.js add     Add new note
    app.js list    List all Notes
    app.js read    Read a note
    app.js remove  Remove a note

  Options:
    --version  Show version number                                       [boolean]
    --help     Show help                                                 [boolean]

```

You can also get details of an individual command

```
$ node app.js add help
app.js add

add new note

Options:
  --version    Show version number                                     [boolean]
  --help       Show help                                               [boolean]
  --title      Title of Note                                          [required]
  --body       Body of Note                                           [required]

```
### Remarks

-   You can also use  `-t`  instead of  `--title`  and  `-b`  instead of  `--body`.
-   `node app.js --help`  gives you all available commands and options.
-   All the dependencies are listed in  `package.json`.
