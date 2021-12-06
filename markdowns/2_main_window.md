## Hands On

Prepare your working environment, run command console (press Win+R, type cmd):
<!-- .element: class="left-orient" -->

```bash
    # Go to your workspace
    cd <c:\your_workspace>
    # to make a dir
    mkdir hands_on_code
    # go to directory
    cd hands_on_code
    # initialize git repository
    git init
    # setup local git config
    # it's possible to setup global
    # git config --global
    git config user.name "<Your-Full-Name>"
    git config user.email "<your-email-address>"
    # checkout the VS Code API
    code --help
    # to run vs code type 
    code .
```
<!-- Notes -->
inj-note:

---

## Main window

![main_win1][main_win1] <!-- .element: width="91%" height="auto" class="stretch"  style="float: right;" -->

[main_win1]: ../../images/main_editor1.PNG "main window"

<!-- Notes -->
inj-note:

---

## Main window

![main_win2][main_win2] <!-- .element: width="91%" height="auto" class="stretch"  style="float: right;" -->

[main_win2]: ../../images/main_editor2.PNG "main window"

<!-- Notes -->
inj-note:

---

## Main window

![main_win3][main_win3] <!-- .element: width="91%" height="auto" class="stretch"  style="float: right;" -->

[main_win3]: ../../images/main_editor3.PNG "main window"

<!-- Notes -->
inj-note:

---


## Hands On

Create new file, `.gitignore` in the code explorer. Add below content in the file editor.
<!-- .element: class="left-orient" -->

```ini
    # Ignore .png files
    *.png
    # ignore .pdf files
    *.pdf
```

Open **bash**(git) **terminal in VS Code**. Make sure that you are in the project folder, write below:
<!-- .element: class="left-orient" -->

```bash
    git add .
    git commit -m "initial commit"
```

---

## Hands On

Create new file, `manifest.md` in the code explorer add following text to the file.
<!-- .element: class="left-orient" -->

```markdown
## Info
<!-- put cursor here -->
|Full name|Occupation|Group|Date|
|:--------|:--------:|:---:|---:|
|Darek Łuczyński|Tester|team|put_the_date_here|


## Manifest

I hereby consent to attend this meeting voluntarily, keep calm till the end of it. 
# About VS Code

Kraków, Poland, presented on put_the_date_here

## Team links

- [Confluence](https://www.atlassian.com/software/confluence)
- [Jira](https://www.atlassian.com/software/jira)

```
<!-- .element: width="100%" height="auto" class="stretch"   -->

Click in the middle of `<!-- put cursor here -->` and hit `Ctrl+Enter`. Modify the markdown using `Alt+LeftClick` on `put_the_date_here`, then change `Darek Łuczyński` to your full name. Select paragraph `# About VS Code` and line beneath, then move it to the top of the file.
