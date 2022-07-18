## Gradient Color Background With Image in Front

### Gradient

Here is the code:
```
Container(
                height: MediaQuery.of(context).size.height * 0.3,
                width: MediaQuery.of(context).size.width,
                decoration: BoxDecoration(
                  gradient: LinearGradient(
                    begin: Alignment.topCenter,
                    end: Alignment.bottomCenter,
                    colors: [
                      myGreen,
                      bgColor_zeroOpacity,
                    ],
                  ),
                  image: const DecorationImage(
                    image: AssetImage("assets/images/logo.png"),
                    fit: BoxFit.fitWidth,
                  ),
                ),
              ),
```
here in the above code snippet I've used a container and inside the container I've used the BoxDecoration widget to add a gradient color to the container and I've added an image to the container.
I've defined height as 0.3 of the screen height, and width as the screen width.