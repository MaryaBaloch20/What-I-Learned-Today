## Introduction Screens using Flutter

![Intro_Screen Image](../images/introduction_screen.jpg)

### Pageview Widget
In this section I'll discuss about pageview widget.
Pageview widget is a widget that allows you to swipe between pages.
Using Pageview widget you can create a scrollable list of pages.
Here is an example of pageview widget that I created:
```
 PageView(
            onPageChanged: (index) {
              setState(() {
                onLastPage = (index == 3);
              });
            },
            controller: _controller,
            children: const [
              LogoScreen(),
              IntroScreen1(),
              IntroScreen2(),
              IntroScreen3(),
            ],
          ), 
```
Here inside the Pageview I've included four screens, which are the children of the Pageview and a controller.
I have also included a function that will be called when the page changes. This function will change the state of the onLastPage variable, when index is 3, the app will change the onLastPage variable to true.

### PageController
PageController is a class that allows you to control the current page of a PageView widget.
You can use the PageController to control the page of a PageView widget.
Here is an example of PageController:
``` final PageController _controller = PageController(); ```
Here I've created a PageController variable called _controller, And I used this _controller in some places in the code. I've used this _controller in the Pageview widget, and in the onPageChanged function, and in the onTap function.

```
GestureDetector(
                          onTap: () {
                            _controller.nextPage(
                                duration: const Duration(milliseconds: 500),
                                curve: Curves.easeIn);
                          },
                          child: const Text(
                            "Next",
                          )),
```
Here in the above code snipper I've used the nextPage function of the PageController to change the page to the next page.


```
GestureDetector(
                      onTap: () {
                        _controller.jumpToPage(3);
                      },
                      child: const Text("Skip")),
```
Here in the above code snippet I've used the jumpToPage function of the PageController to change the page to the third page, which is the last page.