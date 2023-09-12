# A Guide to your first open source contribution

This project aims to simplify and guide the way beginners make their first contribution. If you are looking to make your first contribution, follow the steps below.

## Requirements
Install [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) on your machine

## 1. Fork this repository
Fork this repository by clicking on the fork button on the top of this page. This will create a copy of this repository in your account.

<img width="300" src="https://github.com/Gerry-Aballa/initial-contribution/blob/main/assets/fork.png" alt="fork this repository" />

## 2. Clone the repository
Now clone the forked repository to your machine. Go to your GitHub account, open the forked repository, click on the code button and then click the _copy to clipboard_ icon.

<img width="300" src="https://github.com/Gerry-Aballa/initial-contribution/blob/main/assets/code_btn.png" alt="clone this repository" />

Open a terminal and run the following git command:
```
git clone "url you just copied"
```
Where "url you just copied" (without the quotation marks) is the url to this repository (your fork of this project). See the previous steps to obtain the url.

<img width="300" src="https://github.com/Gerry-Aballa/initial-contribution/blob/main/assets/copy_code.png" alt="copy this repository" />

For example:
```
git clone git@github.com:this-is-you/initial-contribution.git
```
where `this-is-you` is your GitHub username. Here you're copying the contents of the first-contributions repository on GitHub to your computer.


## 3. Create a branch
Change to the repository directory on your computer (if you are not already there):
```
cd initial-contribution
```
Now create a branch using the `git switch` command:
```
git switch -c your-new-branch-name
```

For example:
```
git switch -c add-automation-mantis
```


## 4. Make changes and commit the changes
Now open `Contributions.md` file in a text editor, add your name to it. Don't add it at the beginning or end of the file. Put it anywhere in between. Now, save the file.
If you go to the project directory and execute the command `git status`, you'll see there are changes.

Add those changes to the branch you just created using the `git add` command:
```
git add Contributions.md
```

Now commit those changes using the `git commit` command:
```
git commit -m "Add your-name to Contributions list"
```

replacing `your-name` with your name.


## 5. Push changes to github
Push your changes using the command `git push`:

```
git push -u origin your-branch-name
```

replacing `your-branch-name` with the name of the branch you created earlier.

<details>
<summary> <strong>If you get any errors while pushing, click here:</strong> </summary>

- ### Authentication Error
     <pre>remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
  remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
  fatal: Authentication failed for 'https://github.com/<your-username>/initial-contribution.git/'</pre>
  Go to [GitHub's tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) on generating and configuring an SSH key to your account.

</details>


## 6. Submit your changes for review

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

<img src="https://github.com/Gerry-Aballa/initial-contribution/blob/main/assets/create_pr.png" alt="submit the changes" />

Now submit the pull request.

<img src="https://github.com/Gerry-Aballa/initial-contribution/blob/main/assets/create_pr1.png" alt="create pull request" />

## What next
Soon I'll be merging all your changes into the main branch of this project. You will get a notification email once the changes have been merged.
You are allowed to delete the created branch.

<img src="https://github.com/Gerry-Aballa/initial-contribution/blob/main/assets/delete_branch.png" alt="delete the branch" />

Congrats! You just completed the standard _fork -> clone -> edit -> pull request_ workflow that you'll often encounter as a contributor!

### Tip!
Complete this twice to earn your first [Github badge](https://github.com/drknzz/GitHub-Achievements)
