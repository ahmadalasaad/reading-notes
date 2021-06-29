# Forms

**Why Forms?**

The best known form on the web is probably 
the search box that sits right in the middle of 
Google's homepage.

* Form Structure
```
<form action="http://www.example.com/subscribe.php" 
method="get">
<p>This is where the form controls will appear.
 </p>
</form>
```
* Text Input
```
<form action="http://www.example.com/login.php">
<p>Username:
 <input type="text" name="username" size="15" 
 maxlength="30" />
</p>
</form>
```

* assword Input

```
<form action="http://www.example.com/login.php">
<p>Username:
 <input type="text" name="username" size="15" 
 maxlength="30" />
</p>
<p>Password:
 <input type="password" name="password" size="15" 
 maxlength="30" />
</p>
</form>
```

* Text Area

```
<form action="http://www.example.com/comments.php">
<p>What did you think of this gig?</p>
 <textarea name="comments" cols="20" rows="4">Enter 
 your comments...</textarea>
</form>
```

* Radio Button

```
<form action="http://www.example.com/profile.php">
<p>Please select your favorite genre:
 <br />
 <input type="radio" name="genre" value="rock" 
 checked="checked" /> Rock
 <input type="radio" name="genre" value="pop" /> 
 Pop
 <input type="radio" name="genre" value="jazz" /> 
 Jazz
</p>
</form>
```
* Checkbox

```
form action="http://www.example.com/profile.php">
<p>Please select your favorite music service(s):
 <br />
 <input type="checkbox" name="service" 
 value="itunes" checked="checked" /> iTunes
 <input type="checkbox" name="service" 
 value="lastfm" /> Last.fm
 <input type="checkbox" name="service" 
 value="spotify" /> Spotify
</p>
</form>
```

* Drop Down List Box

```
<form action="http://www.example.com/profile.php">
<p>What device do you listen to music on?</p>
<select name="devices">
 <option value="ipod">iPod</option>
 <option value="radio">Radio</option>
 <option value="computer">Computer</option>
 </select>
</form>
```
* Multiple Select Box

```
<form action="http://www.example.com/profile.php">
<p>Do you play any of the following instruments? 
 (You can select more than one option by holding 
 down control on a PC or command key on a Mac 
 while selecting different options.)</p>
<select name="instruments" size="3" 
 multiple="multiple">
 <option value="guitar" selected="selected">
 Guitar</option>
 <option value="drums">Drums</option>
 <option value="keyboard" 
 selected="selected">Keyboard</option>
 <option value="bass">Bass</option>
</select>
</form>

```

* File Input Box

```
<form action="http://www.example.com/upload.php"
method="post">
<p>Upload your song in MP3 format:</p>
<input type="file" name="user-song" /><br />
<input type="submit" value="Upload" />
</form
```

* Submit Button
```
<form action="http://www.example.com/subscribe.php">
<p>Subscribe to our email list:</p>
<input type="text" name="email" />
<input type="submit" name="subscribe" 
 value="Subscribe" />
</form>
```

# Lists, Tables & Forms

* Bullet Point Styles

```
<h1>The Complete Poems</h1>
<h2>Emily Dickinson</h2>
<ol>
<li>Life</li>
<li>Nature</li>
<li>Love</li>
<li>Time and Eternity</li>
<li>The Single Hound</li>
</ol>

```

* Images for Bullets

```
<h1>Index of Translated Poems</h1>
<h2>Arthur Rimbaud</h2>
<ul>
<li>Ophelia</li>
<li>To Music</li>
<li>A Dream for Winter</li>
<li>Vowels</li>
<li>The Drunken Boat</li>
</ul>
```

# Events

* DIFFERENT EVENT TYPES

UIEVENTS

| **EVENT** | **DESCRIPTION** |
| ----------------- | ------------- |
|load | Web page has finished loading  |
| unload | Web page is unloading (usually because a new page was requested)  |
| error | Browser encounters a JavaScript error or an asset doesn't exist  |
| resize| Browser window has been resized  |
| scroll |User has scrolled up or down the page  |

KEYBOARD EVENTS

| **EVENT** | **DESCRIPTION** |
| ----------------- | ------------- |
|keydown|User first presses a key (repeats while key is depressed)  |
| keyup | User releases a key  |
| keypress | Character is being inserted (repeats while key is depressed)t  |

MOUSE EVENTS 

| **EVENT** | **DESCRIPTION** |
| ----------------- | ------------- |
| click | User presses and releases a button over the same element |
| dbl click  | User presses and releases a button twice over the same element |
| moused own | User presses a mouse button while over an element |
| mouseup | User releases a mouse button while over an element  |
| mousemove | User moves the mouse (not on a touchscreen)  |
| mouseover |User moves the mouse over an element (not on a touchscreen)  |
| mouseout |User moves the mouse off an element (not on a touchscreen)   |
