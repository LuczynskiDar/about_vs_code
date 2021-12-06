# Extension API

VS Code is built with *extensibility in mind*. Almost every part of VS Code can be customized and enhanced through the **[Extension API](https://code.visualstudio.com/api)**. In fact, many core features of VS Code are built as extensions and use the same Extension API.

Extensions can be found in extension marketplace and major thing about it is that it’s not limited to just code. There are custom debuggers, code linters, ssh-terminals, prettifies, and DevOps pipeline connections.

<!-- Notes -->

inj-note:

---

## Extension API Templates

The extension scaffolding is done by a kickstarter, **[Yoeman](https://yeoman.io/)** running on `node.js`.

![extensions1][extensions1] <!-- .element: width="60%" height="auto" class="stretch"  -->

[extensions1]: ../../images/extensions1.png "Yoeman"

To start the extension development you need to run VS Code Extension Generator, then follow the api documentation.

```bash
npm install -g yo generator-code
```

<!-- Notes -->

inj-note:

---

## Markdowns

Install bolded extensions:
<!-- .element: class="left-orient" -->

1. **Markdown All in One**,
2. **Markdownlint**,
3. **Markdown Preview Enhanced**,
4. Markdown PDF

**Preview the markdown** by clicking on the preview icon on the right side.
<!-- .element: class="left-orient" -->
In the terminal, write below:
<!-- .element: class="left-orient" -->

```bash
# make sure that you are in the project folder
git add .
git commit -m "markdown manifest"
```

inj-note:

Pokazać tylko output z markdown w zakładce

---

## Capl extension

Run git bash terminal in VS Code and type following:
<!-- .element: class="left-orient" -->

```bash
    git branch capl
    git checkout capl
    git branch
```

1. **Capl**
   - code highlight, autocompletion and snippets.

Copy reference `capl` file to project folder. Open file and see the first line: `/*@!Encoding:1250*/`.
Click on bottom ribbon at `UTF-8->Reopen with Encoding-1250>`. Observe if encoding's changed.
In the file editor write `testcase`, press tab. See the snippets (`Ctrl+Space`). Go to the terminal and run following:

```bash
    git add .
    git commit -m "capl file commit"
    git checkout master
    git branch
```

---

## VS Code Built-ins

Visual Studio Code has integrated source control management (SCM) and includes Git support in-the-box.
However it can be improved with couple of extensions.

**Git Extensions. Hint:** Try `@popular git` in extensions search window.
<!-- .element: class="left-orient" -->

1. **Git history**, highlights recent commits built into the editor
2. **Git lens**, shows commits, files history stashes
3. **Git Graph**, visualization of git repository
4. Gitignore

Using `Create new branch ...`, create **xml** branch.
<!-- .element: class="left-orient" -->

![git][git] <!-- .element: width="89%" height="auto" class="stretch" -->

[git]: ../../images/main_editor4.PNG "git popup"

---

#### XML Extensions

1. **XML Tools**,
2. **XML**, XML Language Support by Red Hat,
3. **Auto Rename Tag**,
4. **Auto Close Tag**

Copy **xml report** to *hands_on_code folder* and open in the editor. Open **Explorer's pane**, see: `Outline` and `XML Document`. In the `XML document` click on `@null`, then remove the comment in the editor and save. Press `Ctrl+p` and navigate through all symbols.

Add the **xml report** file to source control, write a message and commit.
<!-- .element: class="left-orient" -->

![commit][commit] <!-- .element: width="42%" height="auto" class="stretch" -->

[commit]: ../../images/main_editor5.PNG "git commit"

<!-- Notes -->
inj-note:

1. Create and switch to xml branch
2. Copy prerequisites xml report
3. Add to version control
4. Show the tree/remove comment in the bottom
5. Manipulate with tags
6. Checkin
7. Switch to master

---

### XML Extensions

#### Hands on
<!-- .element: class="left-orient" -->

1. Press `F1` and write `XML Tools: Evaluate XPath` choose: `XPath Query`, then write:

    ```xml
    <!-- write -->
    //testme
    //testmecase[@timestamp>1005]/testmestep/text()
    testme/info/info[name='number']/info/text()
    ```

    Observe *Output: [XPath](https://www.w3schools.com/xml/xpath_syntax.asp) Results* window.
    <!-- .element: class="left-orient" -->

2. Create new tag, see if the closure was created. Rename `<testme>` to `<mytestme>`, see the closing tag changes.
<!-- .element: class="left-orient" -->

---

#### VS Code Built-ins

Emmet snippets and expansion is built right into Visual Studio Code. **[Emmet](https://emmet.io/)** is a web-developer’s toolkit that improves HTML/XML & CSS workflow. To see VS Code built in extensions press `Ctrl+Shift+x` and type `@builtin`.

![emmet][emmet] <!-- .element: width="48%" height="auto" class="stretch"  style="float: right;" -->

[emmet]: ../../images/emmet.gif "Emmet"

Make new file **issues.xml**. In the file press `Ctrl+Space` and choose `Insert XML declaration`, then `Tab`. Under the declaration paste in following and press `Tab`:

```html
<!-- checkout emmet in action -->
head>issue*2>(id#Iss_Test_Name_0x00*3+IssueDet[no="Ticket-" ticket_stat="New" sw="xx.xx.xx"]{Title: My test title })
```

Add **issues.xml** file to source control, write a message and commit. Checkout branch from *xml* to *master*.

<!-- Notes -->
inj-note:
<!-- Insert XML declaration -->

<sop>
    <po>
        ban>tan[reg="" testrun="yes"]{testing changes on the way}*5  
    </po>
</sop>

---

## Visual Extensions

Install bolded extensions:
<!-- .element: class="left-orient" -->

1. **Guides**,
    - Guides › Active: Width > 1 -> 5 (Active indentation guides rendering width)
2. Bracket Pair Colorizer,
3. **Bracket Pair Colorizer 2**,
4. Rainbow indent,
5. Prettier,
6. **Material Icon Theme**,
7. vscode-icons,
8. Better comments,
9. Code spell checker
  
<!-- Notes -->

inj-note:

Only install and describe plugins.

---

## Interactive features

1. Live Server
   - used to trace changes during a web app development.
2. **Live Share Extension Pack**
   - ad hoc collaboration with your partner on the same code without the need to sync code or to configure the same development tools, settings, or environment. It gives an access to remote collaboration session up to 30 people.

Paste the URL into a browser's address or join live share collaboration session in your VS Code. Log into the live share session, use your MS or Github account. Paste in yours **personal row** from info's table in `manifest.md` into collaborative **attendance table**.  

<!-- Notes -->

inj-note:

1. Live Server - show how the presentation works,
2. Live Share Extension Pack - get a part of each person table as a confirmation of presence

Live Share enables you to quickly collaborate with a friend, classmate, or professor

---

## Handy Extensions

1. Visual Studio IntelliCode, code auto completion,
2. Kite AutoComplete, code auto completion,
3. Tabnine, intellisense, code auto completion,
4. Bookmarks,
5. .run, Code Runner,
6. Project Manager,
7. settings sync, VS Code settings export to Github Gist
8. Code Spell Checker

<!-- Notes -->

inj-note:

Powiedzieć tylko kilka słów

---

## Other, Python extensions

1. Python, basic VS plugin,
2. Jupyter,
3. Python preview, debug without running the code (static eval),
4. Arepl for python, evaluates code during typing,
5. Python extension pack,
6. Python docstring generator, generates pydocs,
7. Github copilot, generates code based on syntax/phrase,
8. Python indent, indentation

---

## Other, C# extensions

1. C#,
2. C# Extensions,
3. C# XML Documentation Comments,
4. Auto-Using for C#

---

## Other, html css js

1. Html tag wrap,
2. SVG Viewer,
3. Css peek,
4. Html css support,
5. Es6 snippets,
6. Debugger for chrome,
7. Path Intellisense
