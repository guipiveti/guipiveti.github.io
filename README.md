
## :computer: Creating your own portfolio

1. Manually create a new repository called `your-github-username`.github.io at GitHub:

2. Clone the `code` branch of `guipiveti/guipiveti.guithub.com` by using the following command:

```  bash
git clone -b code https://github.com/guipiveti/guipiveti.github.io.git
```

3. Edit the `homepage` declaration in **`package.json`** to:

```"homepage": "https://your-github-username.github.io"```

4. Edit the **username, default_name and linkedinUrl constants** in ```src/pages/Portfolio/index.js``` .

5. Run:

```bash
npm install
```

6. Edit the remote URL:

```bash
git remote rm origin

git remote add origin https://github.com/<your-github-username>/<your-github-usernam>.github.io.git
```

7. Deploy your portfolio:

```bash

npm run deploy

```

8. Your portfolio should be available in minutes by acessing https://`your-github-username`.github.io

9. **Optional** To save the your edited version of the react app save it into a non-master branch ( In the example I will save it into "code" branch).
```bash
git checkout -b code
git add .
git commit -m "Code commit"
git push origin code
```