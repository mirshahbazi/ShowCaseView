# ShowCaseView


##demo
<table sytle="border: 0px;">
<tr>
<td><img width="200px" src="https://github.com/corerzhang/ShowCaseView/raw/master/screenshot/showcase.gif" /></td>
</tr>
</table>

##use
```java
         View guideView = LayoutInflater.from(this).inflate(R.layout.showcase_content_one, null, false);
         View target = findViewById(R.id.target_one);
         ShowCaseView showCaseView = new ShowCaseView.Builder(MainActivity.this)
                        .setLayoutController(new LayoutController(guideView))
                        .setShape(new CircleShape(this))
                        .build(target);
        
        showCaseView.show(this);
        showCaseView.hide();
        
```

## Support for expansion

###Extends the style of the highlighted area
>setShape(IShape shape)

###Expand layout control
>setLayoutController(ILayoutController layoutController)

###Expand the display and hide the animation
>setAnimationController(IAnimationController animationController)

Add it in your root build.gradle at the end of repositories:
```
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```

Step 2. Add the dependency

```
dependencies {
	        compile 'com.github.mirshahbazi:ShowCaseView:-SNAPSHOT'
	}
```

## Edit By MAM :)
