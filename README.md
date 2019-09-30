

# Cheese Festival - Tooling: GIT/npm/GULP group project
This is the group project for week 5 of the **Coding Fellowship** with **DevelopMe Summer 2019.**

The team:  [Sasha Lawrence](https://github.com/SashaLawrence)  [Oliver Siket](https://github.com/OliverSiket) [Paul](https://github.com/kitespin) 

## The brief
We were set an exercise to build a website using our knowledge of:

## **Tooling: Git & GitHub**

Collaborate in your team using the Gitflow workflow and git branches.

Discuss your working practice, and who will do what in terms of setting up and ongoing roles:

-   Tech lead / pull request reviewer (merging to development)
    
-   Release manager (merging to master)
    
-   Product owner (documenting new features)
    
-   Developers

## **npm and GULP**

 to implement and automate plug ins to handle:

 - compiling sass to CSS and minifying CSS,
 - JS combining and minification
 - html minification
 - to create bootstrap sass
 - 
We also used **gulp.series** to run gulp tasks in series e.g.

    gulp.task('styles', gulp.series('customsassfile', 'minify-css'))

We also had a gulp task that uses **gulp.watch** to watch for changes in SASS files and to combine and minify them:

    gulp.task('watch', function () {
    return  gulp.watch('src/scss/*.scss', gulp.series('styles'));
    });

## Getting Started

view the live website: [cheese festival](https://sashalawrence.github.io/cheese_festival/)
## Screenshots
![Screenshot 2019-09-30 at 22 28 23](https://user-images.githubusercontent.com/51890290/65921911-875ef100-e3db-11e9-9f92-6b669729d054.png)

![Screenshot 2019-09-30 at 22 28 32](https://user-images.githubusercontent.com/51890290/65922006-cb51f600-e3db-11e9-9470-3b2d9c442724.png)

![Screenshot 2019-09-30 at 22 29 01](https://user-images.githubusercontent.com/51890290/65922033-da38a880-e3db-11e9-81bf-91a97bde9f77.png)

## Skills Used
Gitflow, Branches GULP, npm, HTML, CSS, SASS, Bootstrap.

## In order to start work on our site:

### Clone the actual repository:

```
git clone git@github.com:sashalawrence/cheese_festival.git
```

### Check that you have node, npm and	gulp installed:

```
node -v
npm -v
gulp -v
```

### Follow the steps:

```
cd into the cloned repo
```
```
npm init --yes
```
## IMPORTANT NOTE

### Before any changes to your files create your own branch and checkout to it

#### As all the files set up by our team you only have to run 
```
gulp watch
```
#### and you ready to go!

## If any questions see your development team leader.

