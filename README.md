[MY BLOG](https://jak2k.schwanenberg.name/) ▪️ FEDORA-LINUX-USER ▪️ ❤️ OPEN SOURCE ▪️ WANT PRIVACY

## Hi there 👋

- 🔭 I’m working on my website and a search engine.
- 🔧 I'm using **rust, typescript, vue,** nuxt, astro, vitesse. [More here](https://jak2k.schwanenberg.name)
- 🌱 I'm learning Elixir.
- 👯 I’m **looking to collaborate on your open source project** (just open an issue [here](https://github.com/jak2k/jak2k/issues)).
- 🤔 I’m looking for help with [tuxnest](https://github.com/jak2k/tuxnest).
- 💬 Ask me about *anything*!
- 📫 How to reach me: Just [open an issue](https://github.com/Jak2k/Jak2k/issues/new?assignees=&labels=contact&template=contact-me.md&title=Contact+Request) for contacting me (or send a Contact Request on Discord, where I'm called @Jak2k).
- 😄 Pronouns: he/him
- ⚡ Fun fact: My ears have bluetooth. I can listen to music with them and accept calls with them. I can also use them as a microphone.

## [My blog](https://jak2k.schwanenberg.name)

<!--START_SECTION:feed-->
- [Why you should use UnoCSS instead of Tailwind](https:&#x2F;&#x2F;jak2k.schwanenberg.name&#x2F;post&#x2F;unocss-tailwind&#x2F;) 
*In this post, I will explain why you should use UnoCSS instead of Tailwind.
What is Tailwind? (For those who don&#39;t know)
Tailwind is a utility-first CSS framework. It provides you with a set of utility classes that you can use to style your website. It is very popular and is used by many developers.
html

&lt;div class&#x3D;&quot;bg-red-500 text-white p-4 rounded-lg&quot;&gt;This is a card&lt;&#x2F;div&gt;


What is UnoCSS?
To understand what UnoCSS is, let me first explain WindiCSS. WindiCSS was a utility-first CSS framework like Tailwind. It was very similar to Tailwind, but it used just-in-time compilation to reduce the size of the CSS file and the build time.
Tailwind adopted this feature too and WindiCSS got discontinued. UnoCSS is the spiritual successor of WindiCSS. It is much more customizable than Tailwind and has a lot of features that Tailwind doesn&#39;t have.
Some of the features of UnoCSS are:
Presets, like preset-wind which is similar to Tailwind
Dark mode
User-defined shortcuts: btn instead of bg-red-500 border-solid border-1 border-black rounded-full
Extractors: For example, attributify lets you write bg-red-500 text-3xl instead of class&#x3D;&quot;bg-red-500 text-3xl&quot;
Interactive Docs: You can quickly look up a class or a css property
And many more
html

&lt;div bg-red-500 text-white p-4 rounded-lg&gt;This is a card&lt;&#x2F;div&gt;


How can I try it out?
Documentation
Playground
Integrate with your framework
GitHub*
- [I switched from React to Vue](https:&#x2F;&#x2F;jak2k.schwanenberg.name&#x2F;post&#x2F;switch-react-vue&#x2F;) 
*I enjoyed using React. I really liked it. But then I tried Vue and nuxt. I almost cried, for real. Developing with Vue is so much easier. React is legacy code. Here is why.
SFCs are awesome
In a Vue-file you don&#39;t need to do weird stuff with .map() or conditional expressions in JSX placeholders. For conditional rendering you can just use the v-if and v-for html attributes. It&#39;s so much easier to read and understand. Oh, and I don&#39;t have weird issues with missing brackets anymore. Else-if is also much easier to do.
vue

&lt;template&gt;
  &lt;div&gt;
    &lt;h1 v-if&#x3D;&quot;age &gt;&#x3D; 18&quot;&gt;Major&lt;&#x2F;h1&gt;
    &lt;h1 v-else-if&#x3D;&quot;age &gt;&#x3D; 13&quot;&gt;Teenager&lt;&#x2F;h1&gt;
    &lt;h1 v-else&gt;Child&lt;&#x2F;h1&gt;
  &lt;&#x2F;div&gt;
&lt;&#x2F;template&gt;


and
vue

&lt;template&gt;
  &lt;div&gt;
    &lt;h1 v-for&#x3D;&quot;item in items&quot; :key&#x3D;&quot;item.id&quot;&gt;&lt;&#x2F;h1&gt;
  &lt;&#x2F;div&gt;
&lt;&#x2F;template&gt;


instead of
jsx

&lt;div&gt;
  {age &gt;&#x3D; 18 ? &lt;h1&gt;Major&lt;&#x2F;h1&gt; : age &gt;&#x3D; 13 ? &lt;h1&gt;Teenager&lt;&#x2F;h1&gt; : &lt;h1&gt;Child&lt;&#x2F;h1&gt;}
&lt;&#x2F;div&gt;


and
jsx

&lt;div&gt;
  {items.map((item) &#x3D;&gt; (
    &lt;h1 key&#x3D;{item.id}&gt;{item.name}&lt;&#x2F;h1&gt;
  ))}
&lt;&#x2F;div&gt;


Vue has an awesome ecosystem
Don&#39;t get me wrong, React has a great ecosystem too. But Vue has a lot of well thought and well designed libraries. For example, pinia is much more fun than redux and nuxt has a devtool that for itself is worth switching to Vue.
VueUse
VueUse is a collection of useful composition functions (like hooks in React). It&#39;s a great collection of functions that you can use in your Vue project. In react you would need to install a lot of different libraries to get the same functionality.
vue

&lt;script setup lang&#x3D;&quot;ts&quot;&gt;
import { useMouse, useWindowSize } from &quot;@vueuse&#x2F;core&quot;;

const { x, y } &#x3D; useMouse();
const { width, height } &#x3D; useWindowSize();
&lt;&#x2F;script&gt;
&lt;template&gt;
  &lt;div&gt;
    &lt;p&gt;Mouse position: , &lt;&#x2F;p&gt;
    &lt;p&gt;Window size: x&lt;&#x2F;p&gt;
  &lt;&#x2F;div&gt;
&lt;&#x2F;template&gt;


Pinia
Pinia is a state management library for Vue. It&#39;s much easier to use than Redux and it&#39;s much more fun. It&#39;s also much easier to understand. It also integrates very well with the nuxt devtools.
Statemanagement in a Vue component
vue

&lt;script setup lang&#x3D;&quot;ts&quot;&gt;
const counter &#x3D; ref(0);
&lt;&#x2F;script&gt;
&lt;template&gt;
  &lt;div&gt;
    &lt;p&gt;Counter: &lt;&#x2F;p&gt;
    &lt;button @click&#x3D;&quot;counter++&quot;&gt;Increment&lt;&#x2F;button&gt;
  &lt;&#x2F;div&gt;
&lt;&#x2F;template&gt;


Statemanagement with Pinia
typescript

import { defineStore } from &quot;pinia&quot;;

export const useCounterStore &#x3D; defineStore(&quot;counter&quot;, () &#x3D;&gt; {
  const counter &#x3D; ref(0);

  function increment() {
    counter.value++;
  }
  return { counter, increment };
});



vue

&lt;script setup lang&#x3D;&quot;ts&quot;&gt;
import { useCounterStore } from &quot;~&#x2F;store&#x2F;counter&quot;;

const counterStore &#x3D; useCounterStore();
&lt;&#x2F;script&gt;
&lt;template&gt;
  &lt;div&gt;
    &lt;p&gt;Counter: &lt;&#x2F;p&gt;
    &lt;button @click&#x3D;&quot;counterStore.increment()&quot;&gt;Increment&lt;&#x2F;button&gt;
  &lt;&#x2F;div&gt;
&lt;&#x2F;template&gt;


As you can see, state management with Pinia is like state management in a Vue component. It&#39;s much easier to understand and much easier to use.
Nuxt
Nuxt is for Vue what Next.js is for React. It makes it very easy to create a static site or a server side rendered site. It also lets you create api endpoints, but also ships with a powerful database abstraction called nitro stores. You can also edit them in the nuxt devtools.
Nuxt devtools
The nuxt devtools are awesome. You can inspect everything. Here is an overview:
Components: You can see all components that are currently rendered. You can also see the props and the state of the component.
Pinia Stores: You can see all stores and their state. You can also edit the state.
Routes: You can see all routes and their params.
API: You can see all api endpoints and their params. You can also fill data in the params and send a request.
Nitro Stores You can inspect the data in the nitro stores and edit it.
Timeline You can see all events that happened in the app. You can also see the time it took to render a component.
The killer feature is, that you can add modules from inside the devtools. For example you can add tailwind or unocss (read a comparison here) with two clicks. They will also integrate with the devtools.
Vite
Yes, vite was originally made for Vue. It&#39;s much faster than webpack and it&#39;s much easier to configure. It also has a lot of plugins. For example, you can add a plugin to get a fork of the nuxt devtools in vite.
Vue has better state management
I already talked about pinia, but you can also store state locally in a component. When showcasing pinia I also showed how to that. Here a small revision:
vue

&lt;script setup lang&#x3D;&quot;ts&quot;&gt;
const counter &#x3D; ref(0);
const complexUserObject &#x3D; reactive({ name: &quot;John&quot;, age: 18 });
&lt;&#x2F;script&gt;
&lt;template&gt;
  &lt;div&gt;
    &lt;p&gt;Counter: &lt;&#x2F;p&gt;
    &lt;button @click&#x3D;&quot;counter++&quot;&gt;Increment&lt;&#x2F;button&gt;
    &lt;p&gt;User: , &lt;&#x2F;p&gt;
    &lt;button @click&#x3D;&quot;complexUserObject.age++&quot;&gt;Increment age&lt;&#x2F;button&gt;
  &lt;&#x2F;div&gt;
&lt;&#x2F;template&gt;



The demo has been removed because it don&#39;t use Vue on this website anymore. Read more
ref is used for primitive values (like numbers, strings, booleans)
reactive is used for objects and arrays (including nested objects and arrays)
From a ref you can get the value with .value. This is done automatically in the template.
Vue has two-way binding
In Vue you can bind a value to an input and the input will update the value. This much more intuitive than in React. In React you need to use useState and onChange to achieve the same result.
vue

&lt;script setup lang&#x3D;&quot;ts&quot;&gt;
const name &#x3D; ref(&quot;&quot;);
&lt;&#x2F;script&gt;
&lt;template&gt;
  &lt;div&gt;
    &lt;input v-model&#x3D;&quot;name&quot; &#x2F;&gt;
    &lt;p&gt;Hello &lt;&#x2F;p&gt;
  &lt;&#x2F;div&gt;
&lt;&#x2F;template&gt;



The demo has been removed because it don&#39;t use Vue on this website anymore. Read more
Why React is legacy code
It&#39;s super old. It&#39;s like the iPhone, which was the first smartphone. It was great, but now there are better alternatives. React is the same. It was great, but now there are better alternatives. Vue 3.0 is super modern and it&#39;s much easier to use.
It&#39;s not intuitive. You trap in many state management issues and you need to use a lot of libraries to get the same functionality as in Vue.
It uses an old technology. Other frameworks like Vue and Svelte use JS proxies for state management. React uses a setter function. This is much more verbose and much more complicated to use.
It&#39;s owned by Facebook. Originally, it was an internal tool for their needs. Vue is owned by a community.
React is verbose:
React
jsx

import { useState } from &quot;react&quot;; &#x2F;&#x2F; You have to import

export default function Counter() {
  &#x2F;&#x2F; You have to export and define a function
  const [counter, setCounter] &#x3D; useState(0); &#x2F;&#x2F; what a monster for such simple like a reactive variable

  return (
    &lt;div&gt;
      &lt;p&gt;Counter: {counter}&lt;&#x2F;p&gt;
      &lt;button
        onClick&#x3D;{() &#x3D;&gt;
          &#x2F;&#x2F; A function for such a simple thing? And a second one for setting the state correctly?
          setCounter((c) &#x3D;&gt; c + 1)
        }
      &gt;
        Increment
      &lt;&#x2F;button&gt;
    &lt;&#x2F;div&gt;
  );
}


Vue
vue

&lt;script setup lang&#x3D;&quot;ts&quot;&gt;
const counter &#x3D; ref(0);
&lt;&#x2F;script&gt;

&lt;template&gt;
  &lt;div&gt;
    &lt;p&gt;Counter: &lt;&#x2F;p&gt;
    &lt;button @click&#x3D;&quot;counter++&quot;&gt;Increment&lt;&#x2F;button&gt;
  &lt;&#x2F;div&gt;
&lt;&#x2F;template&gt;


Another React example
jsx

&#x2F;&#x2F; I just wanted a simple banner!
export default function Banner() {
  return (
    &lt;div&gt;
      &lt;h1&gt;My awesome website&lt;&#x2F;h1&gt;
      &lt;p&gt;It&#39;s awesome&lt;&#x2F;p&gt;
    &lt;&#x2F;div&gt;
  );
}


Another Vue example
vue

&lt;template&gt;
  &lt;div&gt;
    &lt;h1&gt;My awesome website&lt;&#x2F;h1&gt;
    &lt;p&gt;It&#39;s awesome&lt;&#x2F;p&gt;
  &lt;&#x2F;div&gt;
&lt;&#x2F;template&gt;


Conclusion
Vue is much easier to use than React. It&#39;s also much more intuitive. It&#39;s also much more fun to use. I switched from React to Vue and I don&#39;t regret it. I will never go back to React. Vue and other libraries like Svelte or qwik are the future. React is legacy code.*
- [How to write a webapp in Rust](https:&#x2F;&#x2F;jak2k.schwanenberg.name&#x2F;post&#x2F;rust-webapp&#x2F;) 
*You could write a webapp in Rust, but why should you do that? And how? This post tries to answer most of your questions. If I missed something, please let me know in the comments.
Why should you write a webapp in Rust?
Rust is safe. When it compiles, it works. No more unhandled exceptions or null pointer exceptions.
Rust is fast. It&#39;s as fast as C++ and C, but with a much nicer syntax.
Rust is modern. It has a great package manager, a great build system, and a great community.
Rust is cross-platform. It runs on every OS and on the web.
Rust is everything. It is low-level with no-cost abstractions, but it is also high-level with a great standard library and high-level abstractions.
Rust is helpful. It has a great compiler that helps you write better code.
How to write a webapp in Rust?
To write a frontend in Rust, you could write functions in rust, compile them to WebAssembly, and then use them in JavaScript, or you could use a framework like Yew. We will use Yew in this tutorial. It has an approach similar to React, but it is written in Rust and much more modern than grandpa React.
Prerequisites
Rust - Of course, you need Rust to write Rust code.
rustup target add wasm32-unknown-unknown - This command installs the WebAssembly target for Rust.
cargo install --locked trunk - This command installs the Trunk build tool for Rust.
Create a new project
To create a new project, run cargo generate --git https:&#x2F;&#x2F;github.com&#x2F;yewstack&#x2F;yew-trunk-minimal-template. This command creates a new project from the yew-trunk-minimal-template. It is a minimal template for Yew and Trunk.
The alternative is to create a new project from scratch.
Ok, how does it work?
Look at this code. I added a few comments to explain what&#39;s going on.
rust

use yew::prelude::*; &#x2F;&#x2F; Import things you will need quite often.

#[function_component] &#x2F;&#x2F; Declare a function component. It works like a React functional component.
fn App() -&gt; Html {
    let counter &#x3D; use_state(|| 0); &#x2F;&#x2F; this looks like React hooks, right? It is more like a Preact signal, but don&#39;t mind.
    let onclick &#x3D; {
        let counter &#x3D; counter.clone(); &#x2F;&#x2F; Take the value
        move |_| {
            let value &#x3D; *counter + 1; &#x2F;&#x2F; Increment it
            counter.set(value); &#x2F;&#x2F; And set it!
        }
    };

    html! { &#x2F;&#x2F; This is valid rust, checked by the compiler. Magic!
        &lt;div&gt;
            &lt;button {onclick}&gt;{ &quot;+1&quot; }&lt;&#x2F;button&gt;
            &lt;p&gt;{ *counter }&lt;&#x2F;p&gt;
        &lt;&#x2F;div&gt;
    }
}

fn main() {
    yew::Renderer::&lt;App&gt;::new().render(); &#x2F;&#x2F; And render it!
}


Wow, that was easy, right? But how do you compile it? Run trunk serve to compile it and serve it on http:&#x2F;&#x2F;localhost:8080.
Can we do even better? Yes, we can!
Rust provides powerful enums. We can use them to create messages, that are similar to redux actions.
rust

use js_sys::Date;
&#x2F;&#x2F; ...

#[derive(Clone, Copy, Debug)] &#x2F;&#x2F; Automagicly add some functionality to the enum
enum Msg {
    Increment, &#x2F;&#x2F; One of the cases of the enum
    Decrement,
}

struct App { &#x2F;&#x2F; The model of the app
    counter: u64,
}

impl Component for App { &#x2F;&#x2F; This time it&#39;s not functional
    type Message &#x3D; Msg; &#x2F;&#x2F; The type of the messages
    type Properties &#x3D; (); &#x2F;&#x2F; We have no props

    fn create(_ctx: &amp;Context&lt;Self&gt;) -&gt; Self { &#x2F;&#x2F; Create the model
        Self { counter: 0 }
    }

    fn update(&amp;mut self, _ctx: &amp;Context&lt;Self&gt;, msg: Self::Message) -&gt; bool {
        match msg { &#x2F;&#x2F; Every case of the enum MUST be handled
            Msg::Increment &#x3D;&gt; {
                self.value +&#x3D; 1;
                true &#x2F;&#x2F; Return true to cause the displayed change to update
            }
            Msg::Decrement &#x3D;&gt; {
                self.value -&#x3D; 1;
                true
            }
        }
    }

    fn view(&amp;self, ctx: &amp;Context&lt;Self&gt;) -&gt; Html {
        html! {
            &lt;div&gt;
                &#x2F;&#x2F; We can set classes
                &lt;div class&#x3D;&quot;panel&quot;&gt;
                    &#x2F;&#x2F; A button to send the Increment message
                    &lt;button class&#x3D;&quot;button&quot; onclick&#x3D;{ctx.link().callback(|_| Msg::Increment)}&gt;
                        { &quot;+1&quot; }
                    &lt;&#x2F;button&gt;

                    &#x2F;&#x2F; A button to send the Decrement message
                    &lt;button onclick&#x3D;{ctx.link().callback(|_| Msg::Decrement)}&gt;
                        { &quot;-1&quot; }
                    &lt;&#x2F;button&gt;

                    &#x2F;&#x2F; A button to send two Increment messages
                    &lt;button onclick&#x3D;{ctx.link().batch_callback(|_| vec![Msg::Increment, Msg::Increment])}&gt;
                        { &quot;+1, +1&quot; }
                    &lt;&#x2F;button&gt;

                &lt;&#x2F;div&gt;

                &#x2F;&#x2F; Display the current value of the counter
                &lt;p class&#x3D;&quot;counter&quot;&gt;
                    { self.value }
                &lt;&#x2F;p&gt;

                &#x2F;&#x2F; Display the current date and time the page was rendered
                &lt;p class&#x3D;&quot;footer&quot;&gt;
                    { &quot;Rendered: &quot; }
                    { String::from(Date::new_0().to_string()) }
                &lt;&#x2F;p&gt;
            &lt;&#x2F;div&gt;
        }
    }
}

&#x2F;&#x2F; ...


Ok, let&#39;s recap:
We created a new enum called Msg with two cases: Increment and Decrement.
We created a new struct called App with a field called counter.
We implemented the Component trait for App so that we can use it as a component.
We implemented the create method to create a new instance of App.
We implemented the update method to handle messages.
We implemented the view method to render the component.
This looks like a react class component, right? But it is much better and powerful. Think of it as a redux reducer and a view function in one.
Can I use it in production?
For small side projects, yes. For big critical projects, maybe wait a bit. Yew is still in development, but it is already quite great.
More resources
Yew - The official website of Yew.
Examples - Examples of Yew.
Playground - A playground for Yew. (You should run your code locally, the playground can be a bit slow.)
Trunk - The official website of Trunk.
Rust - The official website of Rust.
Rust book - The official book of Rust.
Rust by example - Rust by example.*
- [Performance is Climate Protection](https:&#x2F;&#x2F;jak2k.schwanenberg.name&#x2F;post&#x2F;performance-climate-protection&#x2F;) 
*Website performance is climate protection. Every bit of data that is transferred over the internet consumes energy. What can you do to reduce your website&#39;s carbon footprint and what did I do to reduce mine?
The Problem
Most websites load lots of JavaScript. Most of this isn&#39;t really needed. That means that the browser has to download and execute lots of code has no real benefit for the user. This is a waste of energy. The more energy is wasted, the more CO2 is emitted. This is bad for the climate.
Another problem are huge images. Most images can&#39;t even be seen in full resolution on most screens.
The Solution
The solution is to reduce the amount of data that is transferred over the internet. This can be done by reducing the amount of JavaScript that is loaded and by reducing the size of images.
My Blog
I used nuxt on this blog. After the inital load, nuxt hydrates the page. This means that lots of JavaScript is loaded to render the exact same page that was already rendered on the server. This is a waste of energy. I switched to Astro. Astro is a static site generator. This means that the page is rendered on the server and then served as a static file. No JavaScript is needed to render the page. This saves lots of energy.
But even in Astro I made changes later. Initially I had enabled view-transitions. They looked really cool, but they also required JavaScript. I disabled them. Now my blog doesn&#39;t use any JavaScript at all. Just for interactive posts like nuxt vs astro I use JavaScript.
What you can do
Use a static site generator like Astro when possible
Reduce the amount of JavaScript that is loaded
Reduce the size of images or avoid them completely (like I did on this blog)
Use a green hoster
Enable compression (gzip, brotli)
Disable JavaScript in your browser (There is NoScript for Firefox. In Chrom(e&#x2F;ium) you can disable JavaScript in the site settings).
Use an adblocker. Ads are just unnecessary :-) (I use uBlock Origin which is available for all major browsers)*
- [Nuxt vs. Astro - Interactive decision helper](https:&#x2F;&#x2F;jak2k.schwanenberg.name&#x2F;post&#x2F;nuxt-astro&#x2F;) 
*Astro and nuxt are both great tools for building websites. But which one should you use? This is an interactive post to help you decide. I will explain the differences between the two and then ask you a few questions to help you decide which one is right for you. At the end, I will give you a recommendation based on your answers.
This is an interactive post. To see the questions and get a recommendation, please enable JavaScript.
Rendering
Astro is a static site generator. This means that it generates all of the HTML, CSS, and JavaScript for your website at build time. This is great for performance because it means that your website will load faster than if it was rendered on the server or client. But it also means that your website will not be able to update in real-time. To update your website, you will need to rebuild it. In astro you can also add interactive islands to your website. These are small pieces of JavaScript that can be used to add interactivity to your website. You can use these to add real-time updates to your website, but they will update the entire page.
Nuxt is a full-stack framework for vue. (Read why I switched to vue) This means that it can render your website on the server or client. This result in good performance, but astro is still faster. If your data updates often, then you should use nuxt, as it provides many tools to work with dynamic data.

Content
Astro is great for rendering markdown-based content from its powerful content directory. You can use this to create a blog, documentation, or any other type of content. You can also use data from an api. For that there are plugins available. Astro also makes it quite easy to generate a sitemap and rss feed.
Nuxt is not to great for content. You can do it too, but for example you can&#39;t use a content directory and generate a rss feed for it. Nuxt is better for dynamic data from an api. But when you use an api it provides you with many tools to work with it.

Development tools.
Astro provides quite solid development tools. It has a built-in dev server with hot reloading. If you want to add an integration you just have to run one command.
Nuxt has an aswesome in-browser devtools. You can see all your stores, components, routes and more. You can also use the dev server with hot reloading. If you want to add an integration you just select it in the devtools and it will be added to your project. These devtools are really awesome and make developing with nuxt a lot easier. You can also throw away postman, because nuxt has a built-in api explorer.

UI Frameworks
Astro has support for everything from A like angular to q like qwik. You can use any ui framework you want. You can also use astro components. These are components that are built with astro and are statically rendered. Components from other frameworks can be rendered on both the server and client.
Nuxt only supports vue. This is also great because you can use the vue ecosystem and you can mix your components. In astro you can&#39;t embed a react component in a vue component. In nuxt all your components are vue.

Performance
As I said, astro is statically rendered. This means that it is very fast. It also has a very small bundle size.
In nuxt you usually use server-side rendering. This means that it is not as fast as astro and has a larger bundle size. There is also lots of code running on the client, which can slow down your website. Nuxt also supports static site generation, but it is not as good as astro and you lose the ability to use dynamic data on that page. That may be fine for a landing page, but not for an entire website.

Conclusion
Based on your answers, I recommend that you use . It is a great tool for building websites and has many features that will make your life easier. You may also change your answers and see if you get a different result.
Aggregata wrote a nice introduction on how to get started with Astro.
Nuxt has a great getting started guide.
Based on your answers, I can&#39;t decide which one is better for you. You may also change your answers and see if you get a different result.
You haven&#39;t answered the questions yet. Please answer them to get a recommendation.*
<!--END_SECTION:feed-->

<!--[![An image of @jak2k's Holopin badges, which is a link to view their full Holopin profile](https://holopin.me/jak2k)](https://holopin.io/@jak2k)-->
