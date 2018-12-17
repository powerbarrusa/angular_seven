# Unit 02:  Creating more components

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

Now that we've
