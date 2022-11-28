# light

Challenges I faced while completing this page and waht I found a solution.
I spent some time on self learning and iterating my codes on the following areas while programmin this web page:

1. The home and serach buttons (icons) on the navigation.

When I edited the codes of navigation at the first time, I found two things I didn't think about at that time. One is that I mistakenly regard the home page and search icon on the left and right sides of the navigation as a downloaded pictures, of course I can download them from the bootstrap logo website. However, I does not have to that. 
The solution I found out - Bootstrap icon. I need to add the link in the html between <head> tag or import into CSS file from our CDN. This information can be found in bootstrap official website. Then I can copy the icon font. Sometimes I will use the svg codes in my html file.
 
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css" integrity="sha384-Zenh87qX5JnK2Jl0vWa8Ck2rdkQ2Bzep5IDxbcnCeuOxjzrPF/et3URy9Bv1WTRi" crossorigin="anonymous">




2. How To Create a Breadcrumb Navigation
A breadcrumb navigation provide links back to each previous page the user navigated through, and shows the user's current location in a website.
Home / Pictures Summer /Italy

![image](https://user-images.githubusercontent.com/102950347/204208629-a7c239a7-3207-4f2c-8b1d-677ed38dc392.png)



Other tips:
-	The logic of creating bean crump navigation is display all the ul list in a flex / inline setting so they will shown in the same line. 
-	List-style: none to remove all bullet points before the list.
-	Text-decoration: none; remove all underline below the lists.
-	Add a “>” in the left side of each list.
  .breadcrumb ul li::before {    
    content: ">";
    margin-left: 6px; 
 }
-	Remove the “>” in the left side of the first list
  .breadcrumb ul li:first-child:before {    
     display: none;
}
-	:after / :before are there to allow you to add content either or after an element from within the CSS. – single colon
-	::after / ::before – double colons
Pseudo-elements - different concept !!
https://www.cnblogs.com/starof/p/4459991.html





3. The second thing is that I should have a macro perspective for the responsive webpage layout from the beginning, so as to avoid further revisions later.Finally, through w3school and bootstrap's explanation on navigation, coupled with repeated tests, I finally understood how to achieve the corresponding layout of small-sized screens by adding corresponding attruibutes in HTML only. Compared with the previous method of adding media query completely through css, this also greatly reduces the running speed of the browser.

There are some links I found helpful:

https://getbootstrap.com/docs/5.2/components/navbar/ 
 
https://www.cnblogs.com/zhangbao/p/6593121.html
 
https://bootstrapshuffle.com/cn/classes/navbar/navbar-toggler-icon
 
https://www.w3schools.com/bootstrap/bootstrap_navbar.asp 


The standard navigation format:
 
![image](https://user-images.githubusercontent.com/102950347/204208518-0c6da830-5200-4d18-9395-22e72bb635ea.png







 
