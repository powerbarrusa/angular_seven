# Unit 02:  Building more pages

## Using the scaffolder to create more components

Angular has a generator that will scaffold new components for us.
We will create three new pages.  Name them whatever you'd like.

I'm going to create a navigation component, and then 4 pages for some regions in Westeros.

cd into the *app* folder, then

do either
```
ng generate component nav  
```
or
```
ng g c nav
```

(the second one is a shortcut)

now look at your folder structure:

![](nav_is_new.png)

Next, I'll create a home page:

```
ng generate home
```



Lastly, I will generate my 4 pages:

```
ng generate component braavos  
```

```
ng generate component dorne  
```

```
ng generate component winterfell  
```

```
ng generate component essos  
```


By examining all of these generated components, you can see that they all share the same structure.

Now that we've got a ton of pages, let's go back to our app.component.html page.


## inserting the nav component

The app.commponent.html page can be used as a container to pull in all of the other pages.
This is why it has, by default, the

```
<router-outlet></router-outlet>
 ```
tags are there.

router outlet is a component that will pull in whichever page has been served up by our router, which we will configure soon.

Since the *nav* will exist on every page, it goes directly on the app.component.html page.

When we click on a link in the nav, whichever page is clicked on should appear in the <router-outlet> component.
