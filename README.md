# Camp Mamo Demos

Welcome to the **Camp Mamo Demos** repository!  
This repo is the single place where participants in **Camp Mamo**—Celestia's hackathon preparation program—can find, pull, and explore every example project used throughout the course.

---

## 📚 What is this repo?
Camp Mamo spans many topics and hands-on sessions. To keep things organised we host each demo or reference implementation in its **own standalone Git repository**.  
This repo is therefore an **anchor / index**: every top-level folder here points to another repository that holds the actual demo code.

We keep these external repos as **Git submodules** so that you can:
1. fetch everything with a single clone command;
2. stay in sync with upstream fixes and improvements;
3. avoid inflating the size of this meta-repo.

If the term *submodule* is new to you—don't worry, the commands you need are listed below.

---

## 🚀 Quick start
```bash
# Clone *and* pull all submodules in one go
$ git clone --recurse-submodules git@github.com:celestiaorg/campmamo-demos.git

# If you already cloned without the flag, run:
$ git submodule update --init --recursive
```
Each sub-folder now contains a fully-functional project ready for you to open, build, and hack on.

---

## 🗂️ Repository layout
```
campmamo-demos/
├── dojo-demo/            # ↳ https://github.com/gbarros/dojo-demo (submodule)
├── chopin-demo/          # placeholder – upcoming demo
├── initia-demo/          # placeholder – upcoming demo
├── livy-demo/            # placeholder – upcoming demo
├── rollkit-demo/         # placeholder – upcoming demo
└── LICENSE               # licence information for this index repo
```
> The exact list will grow as the course progresses. Check back often or run `git pull --recurse-submodules` to stay up-to-date.

---

## 🤝 Contributing & adding new demos
1. Fork this repo and create a new branch.
2. Add the external demo as a submodule:
   ```bash
   git submodule add <demo-repo-git-url> <folder-name>
   ```
3. Commit and push your changes, then open a pull request.  
   Remember to include a short description of the demo and a link to its documentation in the PR body.

Please keep new demos small and focused—participants should be able to clone everything quickly.

---

## 📄 Licence
The content of **this** repo is licensed under the **Apache License 2.0** (see `LICENSE`).  
Each submodule keeps its own licence; make sure you comply with it when re-using code.

---

## 🙋 Need help?
If you hit any issues, open an [issue](https://github.com/celestiaorg/campmamo-demos/issues) or post in the Camp Mamo Discord. We're happy to help!

Happy hacking! 🚀 