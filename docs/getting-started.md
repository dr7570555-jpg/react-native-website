video 
id: environment-setup
title: Get Started with React Native
hide_table_of_contents: true
---

import PlatformSupport from '@site/src/theme/PlatformSupport';
import BoxLink from '@site/src/theme/BoxLink';

**React Native allows developers who know React to create native apps.** At the same time, native developers can use React Native to gain parity between native platforms by writing common features once.

We believe that the best way to experience React Native is through a **Framework**, a toolbox with all the necessary APIs to let you build production ready apps.

You can also use React Native without a Framework, however we’ve found that most developers benefit from using a React Native Framework like [Expo](https://expo.dev). Expo provides features like file-based routing, high-quality universal libraries, and the ability to write plugins that modify native code without having to manage native files.

<details>
<summary>Can I use React Native without a Framework?</summary>

Yes. You can use React Native without a Framework. **However, if you’re building a new app with React Native, we recommend using a Framework.**

In short, you’ll be able to spend time writing your app instead of writing an entire Framework yourself in addition to your app.

The React Native community has spent years refining approaches to navigation, accessing native APIs, dealing with native dependencies, and more. Most apps need these core features. A React Native Framework provides them from the start of your app.

Without a Framework, you’ll either have to write your own solutions to implement core features, or you’ll have to piece together a collection of pre-existing libraries to create a skeleton of a Framework. This takes real work, both when starting your app, then later when maintaining it.

If your app has unusual constraints that are not served well by a Framework, or you prefer to solve these problems yourself, you can make a React Native app without a Framework using Android Studio, Xcode. If you’re interested in this path, learn how to [set up your environment](set-up-your-environment) and how to [get started without a framework](getting-started-without-a-framework).

</details>

## Start a new React Native project with Expo

<PlatformSupport platforms={['android', 'ios', 'tv', 'web']} />

Expo is a production-grade React Native Framework. Expo provides developer tooling that makes developing apps easier, such as file-based routing, a standard library of native modules, and much more.

Expo's Framework is free and open source, with an active community on [GitHub](https://github.com/expo) and [Discord](https://chat.expo.dev). The Expo team works in close collaboration with the React Native team at Meta to bring the latest React Native features to the Expo SDK.

The team at Expo also provides Expo Application Services (EAS), an optional set of services that complements Expo, the Framework, in each step of the development process.

To create a new Expo project, run the following in your terminal:

```shell
npx create-expo-app@latest
```

Once you’ve created your app, check out the rest of Expo’s getting started guide to start developing your app.

<BoxLink href="https://docs.expo.dev/get-started/set-up-your-environment">Continue with Expo</BoxLink>

.css
.js
1
<html><head> 
2
  <meta charset="UTF-8"> 
3
  <meta name="viewport" content="width=device-width, initial-scale=1"> 
4
  <title>Premium Scientific Calculator with Theme Toggle</title> 
5
  <link rel="stylesheet" href="Caculator.css" type="text/css" media="all"> 
6
 </head> 
7
 <body class="dark"> 
8
  <div class="calculator"> 
9
   <div class="theme-toggle-container"> <button id="theme-toggle" class="theme-toggle-button" aria-label="Toggle light/dark mode"> Switch to Light Mode </button> 
10
   </div> 
11
   <div class="display" id="display">
12
    0
13
   </div> 
14
   <div class="buttons"> <button data-action="all-clear">AC</button> <button data-action="clear-last">C</button> <button data-action="parenthesis">(</button> <button data-action="parenthesis">)</button> <button data-number="7">7</button> <button data-number="8">8</button> <button data-number="9">9</button> <button data-action="operator">÷</button> <button data-number="4">4</button> <button data-number="5">5</button> <button data-number="6">6</button> <button data-action="operator">×</button> <button data-number="1">1</button> <button data-number="2">2</button> <button data-number="3">3</button> <button data-action="operator">-</button> <button data-number="0">0</button> <button data-action="decimal">.</button> <button data-action="operator">+</button> <button class="button-equal" data-action="equals">=</button> 
15
   </div> 
16
  </div> 
17
  <script src="Caculator.js"></script> 
18
 
19
</body></html>  
.html
.css
.js
1
<html><head>
2
  
3
 </head>
4
 <body>   
5
  <meta charset="UTF-8"> 
6
  <title>I LOVE You 💖 x500</title> 
7
  <style>
8
    body {
9
      background-color: #fff0f5;
10
      font-family: 'Comic Sans MS', cursive, sans-serif;
11
      display: flex;
12
      flex-wrap: wrap;
13
      justify-content: center;
14
      align-items: center;
15
      padding: 30px;
16
    }
17

18
    .love {
19
      color: #ff1493;
20
      background: #ffe4e1;
21
      border-radius: 10px;
22
      padding: 10px 15px;
23
      margin: 5px;
24
      font-size: 20px;
25
      box-shadow: 2px 2px 5px rgba(255, 105, 180, 0.3);
26
      animation: pop 1s ease-in-out infinite alternate;
27
    }
28

29
    @keyframes pop {
30
      from { transform: scale(1); }
31
      to { transform: scale(1.1); }
32
    }
33
  </style>   
34
  <script>
35
    const message = "I LOVE You 💖";
36
    for (let i = 0; i < 500; i++) {
37
      const span = document.createElement('span');
38
      span.className = 'love';
39
      span.textContent = message;
40
      document.body.appendChild(span);
41
    }
42
  </script>       
43
  
44
 
45
</body></html>  
.html
.css
.js
1
<html><head></head> 
2
 <body> 
3
  <h1> Hello </h1> 
4
  <div>
5
    This is a html example from Dcoder, 
6
   <br> have fun. :) 
7
  </div> 
8
 
9

10

11
    <meta charset="UTF-8">
12
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
13
    <title>YouTube Watch Time</title>
14
    <link rel="stylesheet" href="styles.css">
15

16

17
    <div class="container">
18
        <h1>YouTube Watch Time</h1>
19
        <button id="getStartedButton">Get Started</button>
20
        
21
        <!-- Video Section (hidden by default) -->
22
        <div id="videoSection" class="video-section">
23
            <div class="video-container">
24
                <iframe id="video1" width="560" height="315" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen=""></iframe>
25
            </div>
26
            <div class="video-container">
27
                <iframe id="video2" width="560" height="315" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen=""></iframe>
28
            </div>
29
            <div class="video-container">
30
                <iframe id="video3" width="560" height="315" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen=""></iframe>
31
            </div>
32
            <div class="video-container">
33
                <iframe id="video4" width="560" height="315" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen=""></iframe>
34
            </div>
35
            <div class="video-container">
36
                <iframe id="video5" width="560" height="315" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen=""></iframe>
37
            </div>
38
        </div>
39
    </div>
40

41
    <script src="script.js"></script>
42

43

44
</body></html>
