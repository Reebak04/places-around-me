# Places Around Me

## AIM:

To develop a website to display details about the places around my house.

## Design Steps:

### Step 1:
Open up a terminal in your preffered location, and start a django project using djang-admin startproject Next setup an app inside the project folder using django-admin startapp.

### Step 2:

Once Created ,link your app to the project by adding it in the list of apps in settings.py file located inside the project folder. Add access to your host in allowed host setting and add static folders path to your settings.py file.

### Step 3:

Create a static folder and template folder and add all your required files for the project - Images .etc in your static folder. In the Template folder add your html files required for the pages.

### Step 4:

Head to the views.py in your app folder and create required functions to render a particular page or template when requested by the client. Next go to the urls.py and route the correct view functions to each particular request as needed.

### Step 5:

Next start the server from the projects main directory using python3 manage.py runserver 0:. Now the pages can be accessed from all the routed addresses in urls.py.

## Code:
### map.html
```html
<!DOCTYPE html>
<html>
    <head>
        <title>
            Image Map
        </title>
    </head>
    <body >
        <h1 align="center" >
            <font color="red" >
                    AMBATTUR PARADISE
            </font>   
        </h1>
        <h3 align="center">
        <font color="blue">
            TEJUSVE KABEER.F(212222100054)
        </font>
            
        </h3>
        <center>
            <img src="/static/image/map.png" usemap="#image-map">
            <map name="image-map">
            <area  alt="" title="Rakki Theatre" href="rakki.html" shape="rect" coords="410,87,460,137" style="outline:none;" target="_self"     />
            <area  alt="" title="Ambattur OT Bus Stand" href="bus.html" shape="rect" coords="759,477,809,527" style="outline:none;" target="_self"     />
            <area  alt="" title="Grace Super Market" href="sm.html" shape="rect" coords="1258,598,1308,648" style="outline:none;" target="_self"     />
            <area  alt="" title="Temple" href="temp.html" shape="rect" coords="398,324,448,374" style="outline:none;" target="_self"     />
            <area  alt="" title="Aacini.MAT.HR.SEC.School" href="schl.html" shape="rect" coords="1070,143,1120,193" style="outline:none;" target="_self"     />
            <area shape="rect" coords="1449,894,1451,896" alt="Image Map" style="outline:none;" title="Image Map" href="https://www.image-maps.com/" />
            </map>
        </center>
        <p align="center">
            <font color="maroon"  face="Comic Sans MS" >
                This Image Map shows various locations around my home.<br>
                Click the location and get information about it.
            </font>
        </p>


    </body>
</html>
```
### temp.html
```html
<!DOCTYPE html>
<html>
    <head>
        <title>TEMPLE</title>
    </head>
    <body bgcolor="green">
        <h1 align='center'>TEMPLE</h1>
        <center>
          <img src ="/static/image/temp.png"  height="300" width="600" align="center" >
        </center>
        <p style="font-size: 24px">
            Temple is a place of positivity,where we redeem ourselves just by venting out our emotions to the GOD.
            A temple is a religious building that's meant for worshipping or praying. Hindu temples are typically 
            devoted to one specific god. While temples tend to be associated with non-Christian religions like Islam,
             Judaism, and Buddhism, some sects of Orthodox Christianity worship in temples as well.
        </p>
    </body>

</html>
```
### bus.html
```html
<!DOCTYPE html>
<html>
    <head>
        <title>BS</title>
    </head>
    <body bgcolor="pink">
        <h1 align='center'>BUS STAND</h1>
        <center>
          <img src ="/static/image/bs.png"  height="300" width="600" align="center" >
        </center>
        <p style="font-size: 24px">
        A bus stand, also called a bus bay, or bus stance, is a designated parking location where a bus 
        or coach waits out of service between scheduled public transport services.'Bus stand' is also often 
        an alternative name for specific bus stops inside a bus station.In the simplest case, a bus turnout type 
        of bus  stop is extended, and buses can lay over away from the stop if necessary. In locations where buses 
        cannot emain stationary for long, nearby but separate bus stands may be provided where other bus parking is 
        not conveniently located. 
        </p>
    </body>

</html>
```
### rakki.html
```html
<!DOCTYPE html>
<html>
    <head>
        <title>THEATRE</title>
    </head>
    <body bgcolor="orange">
        <h1 align='center'>RAKKI THEATRE</h1>
        <center>
          <img src ="/static/image/rakki.png"  height="300" width="600" align="center" >
        </center>
        <p style="font-size: 24px">
        Theatre is the only place without any partiality,where all kind of people will sit together and the movie completely.
        It is the place filled with emotions of all kind.Some will assume themselves as actors and starting having fake scenarios
        in their mind.It is the place where the creativity and imagination of one individual will be encouraged and welcomed by
        the world.Each movie is directed with different social message to spread awareness to the people.This is the perfect media
        for spreading awareness to the people by their favourite actor.Though some people don't listen to their parents they 
        will listen to their favourite actor.

        </p>
    </body>

</html>
```
### sm.html
```html
<!DOCTYPE html>
<html>
    <head>
        <title>SM</title>
    </head>
    <body bgcolor="yellow">
        <h1 align='center'>SUPER MARKET</h1>
        <center>
          <img src ="/static/image/sm.png"  height="300" width="600" align="center" >
        </center>
        <p style="font-size: 24px">
        Super market is super place where will be no clock to restrict our shopping time.That place has a lot of items which attracts
        the customers.Especially the kids are attracted very much by chocolates and toys which are being set up at the entrance
        by the business mind.It is a place which reduces our work because this place a collection of products so we don't need to 
        go to different shop for buying different things.super market is a pazhamudhircholai and supermarket which deals all kind
        of fruits and vegetables with all home needs.But now people using online supermarket rather than shopping directly in the
        supermarket
        </p>
    </body>

</html>
```
### schl.html
```html
<!DOCTYPE html>
<html>
    <head>
        <title>SCHOOL</title>
    </head>
    <body bgcolor="blue">
        <h1 align='center'>SCHOOL</h1>
        <center>
          <img src ="/static/image/schl.png"  height="300" width="600" align="center" >
        </center>
        <p style="font-size: 24px">
            School is a word with a mixture of emotions.At this place we would have spent nearly quarter of our life.This
            is the place where we make and correct our mistakes.No matter how mischief we are,the Teachers will mold us into 
            the best shape and make us grow matured with enough experience.The knowledge and experience gained at this place
            will be forever. 
        </p>
    </body>

</html>
```
## Output:

### Serveroutput
![so](https://user-images.githubusercontent.com/118364993/234471518-306f258b-a44c-4320-a10f-2b44f922f405.png)

### Clientoutput
![map](https://user-images.githubusercontent.com/118364993/234471654-7b725744-04f0-4aa8-aa48-cc5ce3f6559b.png)

![bs](https://user-images.githubusercontent.com/118364993/234471666-fc7c1ade-f72f-4e9b-aed7-e13d1ee637c3.png)

![rakki](https://user-images.githubusercontent.com/118364993/234471674-de59acd2-0179-497d-8d16-ebc024e4f10d.png)

![schl](https://user-images.githubusercontent.com/118364993/234471682-b302f10b-6b7c-455a-aede-095575008ea6.png)

![sm](https://user-images.githubusercontent.com/118364993/234471686-568c2168-d5c9-4f86-92c1-70c5b17bbcf1.png)

![temp](https://user-images.githubusercontent.com/118364993/234471702-fc3772cc-6d4a-4ab7-90d1-8c0d4503e543.png)

## Result:
Thus the code has been executed successfully.
