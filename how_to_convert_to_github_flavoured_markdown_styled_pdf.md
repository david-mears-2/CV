NB: links internal to the md do not still work when in pdf.
 
1. Start python virtual environment:

```
python3 -m venv .venv
source .venv/bin/activate
```

2. Install grip

```
pip install grip
```

3. Render file with grip

```
grip README.md
```

4. Go to browser. Download the page as html. 
5. Copy github markdown from the file at https://raw.githubusercontent.com/sindresorhus/github-markdown-css/gh-pages/github-markdown-light.css, which I got from https://github.com/sindresorhus/github-markdown-css. Note I chose the light theme, not the default, which varies depending on the user’s current preference for light or dark system. Add this to the <style> tag in the html head. 
6. Remove link to octicons stylesheet from head. 
7. Add the below to the h3 containing the filename

```
style="display: none"
```

8. Host the html file in the browser. 
9. Print page as pdf from browser. Firefox settings:
    - Untick ‘print headers and footers’ 
    - Remove blank last page if blank.
