# HW1 - Exercise 3.2: Curve plotting in Python: A refresher

Although the plot function is designed primarily for plotting standard xy graphs, it can be adapted for other kinds of plotting as well.

a) Using pyplot, make a plot of the so-called deltoid curve, which is defined parametrically by the equations, x = 2 cos(θ) + cos(2θ) and y = 2 sin(θ) − sin(2θ), where 0 ≤ θ < 2π. 
To do this, take a set of values of θ between zero and 2π, and calculate x and y for each from the equations above, then plot y as a function of x.

b)  Taking this approach a step further, one can make a polar plot r = f(θ) for some function f by calculating r for a range of values of θ and then converting r and θ to Cartesian coordinates using the standard equations x = r cos θ, y = r sin θ. Use this method to make a plot of the Galilean spiral, $$r=θ^2 $$ for 0 ≤ θ ≤ 10π.

c)  Using the same method, make a polar plot of “Fey’s function” in the range 0 ≤ θ ≤ 24π.
$$r = e^{\cos{\theta}} - 2 \cos{4 \theta} + \sin^5{\frac{\theta}{12}} $$ 

Put all 3 plots in one figure with labels making it clear which plot is which. If you're doing this with an ipython notebook, you can have the figure display inline. Otherwise, save the figure as a png or pdf file, and include it in your clone of this repository.


![image](https://github.com/user-attachments/assets/4a6e750f-acde-455a-876f-d6274c09d316)


The [repository](https://github.com/CUNY-CompMethods-2024/Homework1) for the assignment is public. Unfortunately, Github does not directly allow the creation of private forks for public repositories. To create a private fork, you can duplicate the repo as documented [here](https://help.github.com/articles/duplicating-a-repository/) and an example description [here](https://gist.github.com/0xjac/85097472043b697ab57ba1b1c7530274)

To clone this assignment, the commands are as follows:

 1. Create a bare clone of the repository.
    (This is temporary and will be removed so just do it wherever.)
    ```bash
    git clone --bare https://github.com/CUNY-CompMethods-2024/Homework1.git
    ```

 2. [Create a new private repository on Github](https://help.github.com/articles/creating-a-new-repository/) and name it `Homework1`.
    > If you are unable to create a private repo, you can request unlimited private repos as a studant by getting
    > the [student pack](https://education.github.com/pack) from Github.

 3. Mirror-push your bare clone to your new `Homework1` repository.
    > Replace `<your_username>` with your actual Github username in the url below.
    
    ```bash
    cd Homework1.git
    git push --mirror git@github.com:<your_username>/Homework1.git
    ```

 4. Remove the temporary local repository you created in step 1.
    ```bash
    cd ..
    rm -rf Homework1.git
    ```
    
 5. You can now clone your `Homework1` repository on your machine (in my case in the `code` folder).
    ```bash
    cd ~/code
    git clone git@github.com:<your_username>/Homework1.git
    ```
   
 6. (OPTIONAL) If you want, add the original repo as remote to fetch (potential) future changes.
    Make sure you also disable push on the remote (as you are not allowed to push to it anyway).
    ```bash
    git remote add upstream https://github.com/CUNY-CompMethods-2024/Homework1.git
    git remote set-url --push upstream DISABLE
    ```
    You can list all your remotes with `git remote -v`. You should see:
    ```
    origin	git@github.com:<your_username>/Homework1.git (fetch)
    origin	git@github.com:<your_username>/Homework1.git (push)
    upstream	git@github.com:usi-systems/Homework1.git (fetch)
    upstream	DISABLE (push)
    ```
    > When you push, do so on `origin` with `git push origin`.
   
    > When you want to pull changes from `upstream` you can just fetch the remote and rebase on top of your work.
    ```bash
      git fetch upstream
      git rebase upstream/master
      ```
      And solve the conflicts if any
