# Exercise 1: Start a new project folder & Terminal Basics

1. Let's get started with a new project folder:

    - On your MacOS / Windows Desktop, create a new folder called `vibeprojects` (no spaces).

2. Open the new folder in your Terminal / Console:

    - Right click on the new folder and select:
        - MacOS: `services` > `New Terminal at Folder`
        - Windows: `TBC`

3. Figure out what's the path of this folder.

    - MacOS: Type `pwd`
    - Windows: Type `cd`

    Take note of this path.

4. To open this folder in [VSCode](https://code.visualstudio.com/), type: `code .`

    > Tip: Can refer to this [page](https://code.visualstudio.com/docs/configure/command-line?referrer=vsc-search#_launching-from-command-line) on how to add the `code` CLI to your Terminal.

5. You can also use the [Integrated Terminal](https://code.visualstudio.com/docs/terminal/getting-started) in VSCode.

    - From the VSCode menu bar, select: `View` > `Terminal`

6. Do try out some of the Terminal / Console commands below.

## Terminal Commands (Linux and MacOS)

Command | Example | Description
------- | ------- | -----------
`pwd` |  | Present working directory - the folder where you are operating from.
`ls` | `ls -al` | List files in the present directory. <br> `-a` - Include directory entries whose names begin with a dot (‘.’). <br> `-l` - (The lowercase letter “ell”.) List files in the long format.
`cd` | `cd exercises` | Change Directory. The example includes the directory name you want to switch to. <br> To change to the parent directory, use `cd ..` where the 2 `..` refers to the parent folder.
`mkdir` | `mkdir app1` | Creates the folder.
`rm` | `rm badfile.txt`<br> `rm -r badfolder` | To permanently delete a file or directory. To remove a folder, `rm -r <folder_name>`. Be careful as this is a permanent operation.

Anytime you are not sure about how to use a Terminal command, add `--help` to the command to see some helpful tips.

## Windows Console Commands

Command | Example | Description
------- | ------- | -----------
`cd` |  | Present working directory - the folder where you are operating from.
`dir` | `dir` | List files in the present directory. <br> `-a` - Include directory entries whose names begin with a dot (‘.’). <br> `-l` - (The lowercase letter “ell”.) List files in the long format.
`cd` | `cd exercises` | Change Directory. The example includes the directory name you want to switch to. <br> To change to the parent directory, use `cd ..` where the 2 `..` refers to the parent folder.
`mkdir` | `mkdir app1` | Creates the folder.
`del` | `del badfile.txt` | To permanently delete a file. Be careful as this is a permanent operation.
`rmdir` | `rmdir badfolder` | To permanently delete a folder. Be careful as this is a permanent operation.
