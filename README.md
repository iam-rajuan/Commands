<!-- ## Git Commands -->
<h1 align="center">Git Commands</h1>


### Checking Status

- **Check git status**
  ```sh
  git status
  ```
  ```sh
  git status
  ```
  ```sh
  git status
  ```
  ```sh
  git status
  ```








  
  **Example:**
  After modifying a file (`index.js`), run `git status` to check its state before adding it to staging.

### Adding Files to Staging Area

- **Add one file to staging area**
  ```sh
  git add <filename>
  ```
  **Example:**
  ```sh
  git add index.js
  ```
  This adds `index.js` to the staging area.

- **Add all files to staging area**
  ```sh
  git add -A
  git add --a
  git add .
  ```
  **Example:**
  ```sh
  git add .
  ```
  This adds all modified and new files in the repository to staging.

### Committing Changes

- **Perform a Git commit**
  ```sh
  git commit -m "Commit message"
  ```
  **Example:**
  ```sh
  git commit -m "Added new feature to homepage"
  ```

- **Direct commit without staging**
  ```sh
  git commit -a -m "Commit message"
  ```
  **Example:**
  ```sh
  git commit -a -m "Updated styles in CSS files"
  ```

### Checking and Comparing Changes

- **Checkout one file**
  ```sh
  git checkout <filename>
  ```
  **Example:**
  ```sh
  git checkout index.js
  ```
  Restores `index.js` to the last committed state.

- **Checkout all files from the last commit**
  ```sh
  git checkout -f
  ```

- **Check recent activities (last 2 commits with changes)**
  ```sh
  git log -p -2
  ```

- **Compare working tree to staging area**
  ```sh
  git diff
  ```

- **Compare last commit to staging area**
  ```sh
  git diff --staged
  ```

### Removing Files

- **Delete from staging area to untracked**
  ```sh
  git rm --cached <filename>
  ```
  **Example:**
  ```sh
  git rm --cached config.json
  ```
  This removes `config.json` from version control but keeps it locally.

- **Delete file completely**
  ```sh
  git rm <filename>
  ```
  **Example:**
  ```sh
  git rm old_script.js
  ```

- **Remove `node_modules` from Git and ignore it in future commits**
  ```sh
  git rm -r --cached node_modules
  echo "node_modules/" >> .gitignore
  git add .gitignore
  git commit -m "Removed node_modules and updated .gitignore"
  git push origin main
  ```
  **Example:**
  If you accidentally committed `node_modules`, this removes it and prevents future commits.

### Short Status View

- **Show short status**
  ```sh
  git status -s
  ```
  **Example:**
  Displays a compact version of `git status`, showing modified (`M`), new (`A`), and deleted (`D`) files.





### Remote Repository Setup

- **Set remote repository**
  ```sh
  git remote set-url origin git@github.com:iam-rajuan/WebDevelopmentProjects.git
  ```
  **Example:**
  If you change your GitHub repository URL, use this command to update it.

- **View remote repositories**
  ```sh
  git remote -v
  ```

### Pushing Changes to GitHub

- **Push to master branch**
  ```sh
  git push origin master
  ```
  **Example:**
  ```sh
  git push origin main
  ```
  Pushes changes to the `main` branch.

- **Push to a specific branch**
  ```sh
  git push origin branch1
  ```

- **Set upstream and push**
  ```sh
  git push -u origin master
  ```

- **Push using the set upstream**
  ```sh
  git push
  ```

 
<br><br>
<!-- # Ignoring `package-lock.json` and `node_modules` in Git  -->
<h2 align="center">Ignoring `package-lock.json` and `node_modules` in Git </h2>

### 1. Modify `.gitignore` in Your Repository  
To ignore `package-lock.json` and `node_modules/` from all folders inside a specific repository, add the following lines to the `.gitignore` file at the root of your project:  

```gitignore
**/package-lock.json
**/node_modules/
```  

This ensures that `package-lock.json` and all `node_modules/` folders are ignored throughout the repository.  

### 2. Use a Global `.gitignore` (For All Repositories)  
To ignore `package-lock.json` and `node_modules/` in all your Git repositories, follow these steps:  

```sh
git config --global core.excludesfile ~/.gitignore_global
```  

Then, edit `~/.gitignore_global` and add:  

```gitignore
**/package-lock.json
**/node_modules/
```  

### 3. Remove Already Tracked `package-lock.json` and `node_modules/` Files  
If `package-lock.json` and `node_modules/` have already been committed, remove them from tracking:  

```sh
git rm --cached **/package-lock.json
git rm -r --cached **/node_modules/
git commit -m "Removed package-lock.json and node_modules from tracking"
git push origin main  # or your current branch
```  


  






<br><br>
<!-- # SSH Key Setup -->
<h2 align="center">SSH Key Setup</h2>

- **Configure Username & email**
  ```sh
  git config --global user.name "Md Rajuan Hossen"
  ```
  ```sh
  git config --global user.email "rajuan.official@gmail.com"
  ```
  
- **Generate SSH key**
  ```sh
  ssh-keygen -t rsa -b 4096 -C "rajuan.official@.com"
  ```

- **Start SSH agent**
  ```sh
  eval $(ssh-agent -s)
  ```

- **Add SSH key to agent**
  ```sh
  ssh-add ~/.ssh/id_rsa
  ```

- **View SSH public key**
  ```sh
  cat ~/.ssh/id_rsa.pub
  ```
- Copy the txt "ssh-rsa ... @.com" and set up your key.

---



  

<br><br><br><br><br><hr>
<h1 align="center">Terminal Modify & Download Manager</h1>
<!-- https://zimfw.sh/ -->

## Terminal commands
- **install softwares**
  ```sh
  sudo dpkg -i ***
  ```
## Terminal Mod

- **ubuntu**
  ```sh
  https://zimfw.sh/
  ```
- **Windows Terminal Admin**
  ```sh
  Powershell 7+
  winget install --id Microsoft.Powershell
  ```
## IDM 
  - **IDM Crack**
  ```sh
  iex(irm is.gd/idm_reset)
  ```
---


<br><br><br><br><br><hr>
<!-- # VS Code Shortcuts -->
<h1 align="center">VS Code Shortcuts</h1>

  
## Terminal Command

- **Go back to user location**
```sh
cd
```
- **Go back Previous location like backward**
```sh
cd -
```
- **Change C: to D:**
```sh
D: 
```
- **Previous Directory**
```sh
cd ..
```
- **Close Terminal and Open Existing Directory**
```sh
code -r <dirname> 
code -r ExpressJS 
```
---







<!-- # Installed Extensions -->
<br><br>
<h1 align="center">Installed Extensions Details</h1>


Below is a list of all the extensions installed in Visual Studio Code:

## General Extensions
- **Error Lens**: Improve highlighting of errors, warnings, and other language diagnostics.
- **JavaScript and TypeScript Nightly**: Enables TypeScript@next to power VS Code's built-in JavaScript and TypeScript support.
- **Auto Rename Tag**: Auto rename paired HTML/XML tags.
- **Code Runner**: Run code snippets for multiple languages including C, C++, Java, JS, PHP, Python, and more.
- **Dracula Theme Official**: A dark theme for many editors, shells, and more.
- **Material Icon Theme**: Material Design Icons for Visual Studio Code.
- **SynthWave '84**: A Synthwave-inspired color theme.
- **vscode-icons**: Icons for Visual Studio Code.
- **Jellyfish Theme**: A theme for your code editor.
- **GitHub Theme**: GitHub theme for VS Code.

## C/C++ Development
- **C/C++**: C/C++ IntelliSense, debugging, and code browsing.
- **C/C++ Extension Pack**: Popular extensions for C++ development.
- **C/C++ Themes**: UI Themes for C/C++ extension.
- **CMake**: CMake language support for Visual Studio Code.
- **CMake Tools**: Extended CMake support in Visual Studio Code.

## Java Development
- **Debugger for Java**: A lightweight Java debugger for Visual Studio Code.
- **Extension Pack for Java**: Popular extensions for Java development.
- **Gradle for Java**: Manage Gradle projects and run Gradle tasks.
- **Language Support for Java(TM) by Red Hat**: Java linting, IntelliSense, formatting, and more.
- **Maven for Java**: Manage Maven projects and execute goals.
- **Project Manager for Java**: Manage Java projects in Visual Studio Code.
- **Test Runner for Java**: Run and debug JUnit or TestNG test cases.

## PHP Development
- **PHP**: All-in-One PHP support including IntelliSense, Debug, Formatter, and more.
- **PHP Intelephense**: PHP code intelligence for Visual Studio Code.
- **PHP Profiler**: Support for PHP (Xdebug) profiling files.
- **PHP Server**: Serve your project with PHP.
- **IntelliPHP - AI Autocomplete for PHP**: AI-assisted development for PHP.

## Web Development
- **Tailwind CSS IntelliSense**: Intelligent Tailwind CSS tooling for VS Code.
- **Live Server**: Launch a development local server with live reload feature.
- **Live Preview**: Hosts a local server for previewing webpages.
- **Prettier - Code formatter**: Code formatter using Prettier.

## React/Redux/GraphQL Development
- **ES7 React/Redux/GraphQL/React-Native snippets**: Simple extensions for React, Redux, and GraphQL in JS/TS with ES7 syntax.
- **ES7+ React/Redux/React-Native snippets**: Extensions for React, React-Native, and Redux in JS/TS with ES7+ syntax.

## AI-Assisted Development
- **IntelliCode**: AI-assisted development.
- **IntelliCode API Usage Examples**: See relevant code examples from GitHub for over 100K different APIs.

## Other Utilities
- **Composer**: All-in-One Composer integration for PHP.
- **JavaScript (ES6) code snippets**: Code snippets for JavaScript in ES6 syntax.

---



<!-- # Installed Extensions -->
<h1 align="center">Installed Extensions</h1>

<!-- Below is a list of all the extensions installed in Visual Studio Code: -->

## General Extensions
- **Improve highlighting of errors, warnings, and other language diagnostics**
```sh
Error Lens
```

- **Enables TypeScript@next to power VS Code's built-in JavaScript and TypeScript support**
```sh
JavaScript and TypeScript Nightly
```
- **Auto rename paired HTML/XML tags**
```sh
Auto Rename Tag
```
- **Run code snippets for multiple languages including C, C++, Java, JS, PHP, Python, and more**
```sh
Code Runner
```
- **A dark theme for many editors, shells, and more**
```sh
Dracula Theme Official
```
- **Material Design Icons for Visual Studio Code**
```sh
Material Icon Theme
```
- **A Synthwave-inspired color theme**
```sh
SynthWave '84
```
- **Icons for Visual Studio Code**
```sh
vscode-icons
```
- **A theme for your code editor**
```sh
Jellyfish Theme
```
- **GitHub theme for VS Code**
```sh
GitHub Theme
```

## C/C++ Development
- **C/C++ IntelliSense, debugging, and code browsing**
```sh
C/C++
```
- **Popular extensions for C++ development**
```sh
C/C++ Extension Pack
```
- **UI Themes for C/C++ extension**
```sh
C/C++ Themes
```
- **CMake language support for Visual Studio Code**
```sh
CMake
```
- **Extended CMake support in Visual Studio Code**
```sh
CMake Tools
```

## Java Development
- **A lightweight Java debugger for Visual Studio Code**
```sh
Debugger for Java
```
- **Popular extensions for Java development**
```sh
Extension Pack for Java
```
- **Manage Gradle projects and run Gradle tasks**
```sh
Gradle for Java
```
- **Java linting, IntelliSense, formatting, and more**
```sh
Language Support for Java(TM) by Red Hat
```
- **Manage Maven projects and execute goals**
```sh
Maven for Java
```
- **Manage Java projects in Visual Studio Code**
```sh
Project Manager for Java
```
- **Run and debug JUnit or TestNG test cases**
```sh
Test Runner for Java
```

## PHP Development
- **All-in-One PHP support including IntelliSense, Debug, Formatter, and more**
```sh
PHP
```
- **PHP code intelligence for Visual Studio Code**
```sh
PHP Intelephense
```
- **Support for PHP (Xdebug) profiling files**
```sh
PHP Profiler
```
- **Serve your project with PHP**
```sh
PHP Server
```
- **AI-assisted development for PHP**
```sh
IntelliPHP - AI Autocomplete for PHP
```

## Web Development
- **Intelligent Tailwind CSS tooling for VS Code**
```sh
Tailwind CSS IntelliSense
```
- **Launch a development local server with live reload feature**
```sh
Live Server
```
- **Hosts a local server for previewing webpages**
```sh
Live Preview
```
- **Code formatter using Prettier**
```sh
Prettier - Code formatter
```

## React/Redux/GraphQL Development
- **Simple extensions for React, Redux, and GraphQL in JS/TS with ES7 syntax**
```sh
ES7 React/Redux/GraphQL/React-Native snippets
```
- **Extensions for React, React-Native, and Redux in JS/TS with ES7+ syntax**
```sh
ES7+ React/Redux/React-Native snippets
```

## AI-Assisted Development
- **AI-assisted development**
```sh
IntelliCode
```
- **See relevant code examples from GitHub for over 100K different APIs**
```sh
IntelliCode API Usage Examples
```

## Other Utilities
- **All-in-One Composer integration for PHP**
```sh
Composer
```
- **Code snippets for JavaScript in ES6 syntax**
```sh
JavaScript (ES6) code snippets
```
```sh
JavaScript (ES6) code snippets
```

---



<br><br><br><br><br><hr>
<!-- # VS Code Shortcuts -->
<h1 align="center">Sublime Text</h1>

<h2 align="center">Installation & Code+Input+Output -> Setup & View</h2>

- **view**
```
alt+shift+3
view> Groups> Max Column 2
```

- **Code+Input+Output**
```
1. file.cpp 
2. inputf.in 
3. outputf.in 
```
- Setup C++
```
tools> build system> new build system>
save file naem as C++14.sublime-build 
```
<h2 align="center">Build System</h2>

- **C++14_windows-sublime-build** 
```
{
"cmd": ["g++.exe","-std=c++14", "${file}", "-o", "${file_base_name}.exe", "&&" , "${file_base_name}.exe<inputf.in>outputf.in"],
"selector":"source.cpp",
"shell":true,
"working_dir":"$file_path"
}
```
- **C++14_linux-sublime-build** 
```
{
"cmd" : ["g++ -std=c++14 $file_name -o $file_base_name && timeout 4s ./$file_base_name<inputf.in>outputf.in"], 
"selector" : "source.c",
"shell": true,
"working_dir" : "$file_path"
}
```
- **C++14_macos-sublime-build** 
```
{
  "cmd" : ["g++-10 $file_name -o $file_base_name && gtimeout 4s ./$file_base_name<inputf.in>outputf.in"], 
  "selector" : "source.c",
  "shell": true,
  "working_dir" : "$file_path"
}
```
```
save file with name "C++14" and tools> build system> C++14
```
